---
title: Adobe Workfront Planning 요청 제출
description: 누군가가 Adobe Workfront Planning의 레코드 유형 페이지에서 요청 양식에 대한 링크를 귀하에게 공유하면 요청을 추가하여 요청 양식과 연관된 레코드 유형에 대한 레코드를 생성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 99e26d4249162e46da1a73301e68bdf30436a81d
workflow-type: tm+mt
source-wordcount: '1871'
ht-degree: 1%

---

# Adobe Workfront Planning 요청을 제출하여 레코드 생성

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

작업 영역 관리자가 Adobe Workfront Planning에서 레코드 유형에 대한 요청 양식을 작성한 후 이 양식을 사용하여 해당 양식과 관련된 레코드 유형에 대한 레코드를 만들 요청을 제출할 수 있습니다.

다음 영역에서 Workfront Planning 요청을 제출할 수 있습니다.

* Workfront의 요청 영역에서
* 공유된 요청 양식에 대한 직접 링크에서.
* 레코드 유형 페이지에서 새 레코드를 추가하거나 요청할 때 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.

이 문서에서는 Workfront의 요청 영역 또는 공유 링크에서 레코드 유형에 새 레코드를 추가하도록 요청을 제출하는 방법에 대해 설명합니다.


Workfront 사용자와 외부 사용자는 Planning 레코드 유형에 요청을 제출하고 레코드를 생성할 수 있습니다. <!--double check on the external users-->

작업 영역 관리자가 요청 양식을 만들고 레코드 유형과 연결하는 방법에 대한 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>모든 Workfront 패키지 및 모든 Planning 패키지</p>
또는
<p>모든 워크플로우 패키지 및 모든 Planning 패키지</p>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>임의</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>Workfront 사용자인 경우 작업 공간 및 레코드 유형에 대한 이상의 권한을 봅니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

Workfront Planning 요청 양식에 요청을 제출하려면 먼저 다음 조건을 충족해야 합니다.

* Workfront Planning에는 다음이 있어야 합니다.

   * 작업 영역
   * 레코드 종류.
   * 레코드 유형과 연결된 요청 양식입니다.

     자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

* 액세스 가능한 방식으로 요청 양식을 공유해야 합니다. 다음과 같은 시나리오가 있습니다.

   * 내부적으로 작업 영역에 대한 보기 이상의 권한이 있는 사용자와 양식을 공유해야 합니다.

     Workfront 사용자는 링크에서 양식에 액세스하거나 Workfront의 요청 영역에서 요청 양식을 찾을 수 있습니다.

   * Workfront 계정이 없는 경우 양식에 대한 링크가 외부 사용자와 공유되었습니다.

     Workfront 사용자는 외부 사용자와 공유되는 링크에 액세스할 수도 있습니다.

* 양식에 대한 링크가 만료되지 않아야 합니다.

## Workfront Planning에 요청 제출에 대한 고려 사항

* 요청을 제출한 후에는 Workfront에서 요청을 편집할 수 없습니다.
* 제출된 각 요청은 사용하는 양식과 연결된 레코드 유형, 양식이 승인과 연결되지 않은 경우 또는 모든 승인자가 승인을 부여한 경우 레코드를 만듭니다.
* 요청 양식을 제출하여 생성된 레코드는 Workfront Planning에서 다른 방법을 통해 추가된 레코드와 구분할 수 없습니다.

  자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.
* 제출된 요청은 Workfront의 요청 영역에 표시됩니다.
* 제출된 Planning 요청은 새 요청 경험에서만 볼 수 있습니다. 레거시 요청 환경에서는 Planning 요청을 볼 수 없습니다.
* 특정 필드 유형이 요청 양식 또는 양식 제출 후 요청 세부 정보 페이지에 표시되는 방법에는 제한이 있습니다.

  자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Workfront의 요청 영역에서 Workfront Planning에 요청 제출

{{step1-to-requests}}

1. 화면 오른쪽 상단에서 **새 경험으로 전환** 설정을 사용하도록 설정합니다.
이 설정을 사용하면 Workfront Planning 요청 양식을 Workfront의 **요청** 영역에서 사용할 수 있습니다.

   >[!TIP]
   >
   >이 설정은 다음과 같은 경우에만 사용할 수 있습니다.
   >
   >* 귀사에서 Workfront Planning 패키지를 구매했습니다.
   >* Workfront 인스턴스가 Adobe 통합 경험에 온보딩됩니다.
   >* 하나 이상의 작업 영역을 볼 수 있는 액세스 권한이 있습니다.
   >

1. **제출하려는 요청** 막대를 클릭하여 요청 양식 목록을 엽니다.
1. 목록에서 요청 양식을 선택하거나 요청 양식 이름을 입력한 다음 목록에 표시될 때 선택합니다.

   창이 열리고 맨 위에 요청 양식 이름이 표시됩니다.
1. 요청 양식에서 사용할 수 있는 필드를 업데이트합니다. 빨간색 별표가 있는 필드는 필수입니다.
1. **제출을 클릭합니다**.

   요청 양식이 닫히고 **요청** 영역으로 돌아갑니다.

   양식이 제출되고 다음 사항이 발생합니다.

   * 요청 양식이 승인과 연결되어 있지 않은 경우, 요청은 Workfront 요청 영역 및 내 요청 위젯의 요청 목록에 추가되고 새 레코드는 해당 양식과 연결된 레코드 유형에 추가됩니다.

   * 요청 양식이 승인과 연결된 경우 요청이 Workfront 요청 영역 및 내 요청 위젯의 요청 목록에 추가됩니다. 새 레코드는 승인자가 승인한 후에만 레코드 유형 페이지에 추가됩니다.

     자세한 내용은 [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)를 참조하십시오.

   * 요청은 소유자, 승인자 및 작업 영역에 대해 최소 보기 권한이 있는 사람에게만 표시됩니다. Workfront 관리자는 시스템의 작업 영역에 제출된 모든 요청을 볼 수 있습니다.

   * 요청이 성공적으로 제출되었거나 검토를 위해 전송되었다는 인앱 및 이메일 알림을 받게 됩니다.
   * 요청 양식이 승인과 연결된 경우 승인자는 요청을 검토하고 승인하기 위한 인앱 및 이메일 알림을 수신합니다.

     >[!NOTE]
     >
     >이메일 및 인앱 알림은 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩될 때만 표시됩니다.
     >
     >이메일 확인 또는 승인 알림에 요청에 대한 링크가 있습니다.

1. (선택 사항) 확인 메시지에서 **요청 보기**&#x200B;를 클릭하여 요청을 열거나 **X** 아이콘을 클릭하여 확인을 닫습니다.
1. (선택 사항) 다음 중 하나를 수행합니다.

   * **필터**&#x200B;를 클릭하고 계획 탭에서 보려는 요청에 대한 조건을 추가하기 시작합니다.

     ![계획 요청 탭에서 필터 편집](assets/filters-editing-box-in-requests-planning-tab.png)

     다음 필드를 기준으로 필터링할 수 있습니다.

      * **Workspace**: 요청 양식과 연결된 작업 영역입니다.
      * **레코드 종류**: 요청 양식과 연결된 레코드 종류.
      * **시작 날짜**: 요청이 제출된 날짜입니다.
      * **요청 양식**: 요청을 제출하는 데 사용되는 요청 양식의 이름입니다.
      * **상태**: 요청의 상태입니다.
      * **입력한 사람**: 요청을 추가한 사용자의 이름입니다. Workfront 외부의 사용자가 요청을 추가한 경우 **입력한 사람** 필드에 `N/A`이(가) 표시됩니다.

        **And** 또는 **Or** 중 하나로 여러 필터를 연결할 수 있습니다.
필터 조건을 추가하면 요청 목록이 자동으로 필터링됩니다.

   * **열**&#x200B;을(를) 클릭하고 요청 목록에서 열을 숨기거나 표시하거나 다시 정렬하십시오.

     >[!TIP]
     >
     >열을 더 이상 추가할 수 없습니다.
     >
     >**제목** 필드를 표시할 수 없습니다.

     ![](assets/columns-editing-box-in-requests-planning-tab.png)


1. 목록에서 요청 이름을 클릭합니다.

   요청 세부 정보 페이지가 열립니다.

   ![댓글이 있는 요청 페이지](assets/new-request-page-with-comment.png)

1. (선택 사항) [주석] 영역에 주석을 입력합니다.
1. (조건부) 요청 양식이 승인과 연결되어 있지 않거나 요청이 승인된 경우 요청 이름을 클릭한 다음 **레코드** 필드의 레코드 이름을 클릭합니다.

   레코드의 페이지가 Workfront Planning에 열립니다.

   >[!TIP]
   >
   >* 레코드의 기본 필드가 요청 양식에서 업데이트되지 않으면 요청의 레코드 필드에 있는 레코드 이름이 **제목 없음**&#x200B;으로 표시됩니다.
   >
   >* 요청 양식이 승인과 연결된 경우 요청 페이지에서 레코드에 액세스하려면 승인을 받아야 합니다.

1. (선택 사항) **레코드 종류**&#x200B;의 이름을 클릭합니다.

   Workfront Planning에서 레코드 유형 페이지가 열립니다.

## 공유 링크에서 요청 양식으로 Workfront Planning에 요청 제출

1. Workfront Planning 레코드 유형에서 사용자와 공유되는 링크로 이동합니다.

1. 양식에서 사용할 수 있는 필드를 업데이트합니다. 별표가 있는 필드는 필수입니다.

   >[!TIP]
   >
   >   **제목** 필드를 사용할 수 있는 경우 요청이 제출된 후에는 Workfront Planning에 표시되지 않습니다.
   >
   >Workfront Planning의 레코드 유형에 추가될 때 새 레코드를 식별할 수 있도록 요청의 필드를 가능한 한 많이 업데이트하는 것이 좋습니다.

1. **제출을 클릭합니다**.

   양식이 제출되고 다음 사항이 발생합니다.

   * 요청 양식이 승인과 연결되어 있지 않은 경우, 요청은 Workfront 요청 영역 및 내 요청 위젯의 요청 목록에 추가되고 새 레코드는 해당 양식과 연결된 레코드 유형에 추가됩니다.

   * 요청 양식이 승인과 연결된 경우 요청이 Workfront 요청 영역 및 내 요청 위젯의 요청 목록에 추가됩니다. 새 레코드는 모든 승인자가 승인한 후에만 레코드 유형 페이지에 추가됩니다.

     자세한 내용은 [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)를 참조하십시오.

     >[!IMPORTANT]
     >
     >볼 수 있는 권한 이상이 있는 작업 영역에 사용자 또는 다른 사람이 제출한 요청만 볼 수 있습니다. Workfront 관리자는 시스템의 작업 영역에 제출된 모든 요청을 볼 수 있습니다. <!--ensure this is correct; asking team in slack-->

   * 요청이 성공적으로 제출되었거나 검토를 위해 전송되었다는 인앱 및 이메일 알림을 받게 됩니다.
   * 요청 양식이 승인과 연결된 경우 승인자는 요청을 검토하고 승인하기 위한 인앱 및 이메일 알림을 수신합니다.

     >[!NOTE]
     >
     >이메일 및 인앱 알림은 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩될 때만 표시됩니다.

   <!-- <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>-->

1. (선택 사항) Workfront에서 요청을 열려면 **요청 보기**&#x200B;를 클릭합니다.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (선택 사항) **기본 메뉴** > **요청** > **계획** 탭을 클릭하여 요청을 확인한 다음 요청 이름을 클릭합니다.

   요청 세부 정보 페이지가 열립니다.

   ![댓글이 있는 요청 페이지](assets/new-request-page-with-comment.png)



1. (선택 사항) [주석] 영역에 주석을 입력합니다.
1. (조건부) 요청 양식이 승인과 연결되어 있지 않거나 요청이 승인된 경우 요청 이름을 클릭한 다음 **레코드** 필드의 레코드 이름을 클릭합니다.

   레코드의 페이지가 Workfront Planning에 열립니다.

   >[!TIP]
   >
   >* 레코드 이름이 요청 양식에 추가되지 않은 경우 요청의 레코드 필드에 있는 레코드 이름이 **제목 없음**&#x200B;으로 표시됩니다.
   >
   >* 요청 양식이 승인과 연결된 경우 요청 페이지에서 레코드에 액세스하려면 승인을 받아야 합니다.

1. (선택 사항) **레코드 종류**&#x200B;의 이름을 클릭합니다.

   Workfront Planning에서 레코드 유형 페이지가 열립니다.

<div class="preview">

## 기존 요청을 복사하여 요청 만들기

Workfront의 요청 목록에서 요청을 복사한 다음 세부 사항을 편집하고 새 요청으로 제출할 수 있습니다.

새 요청 경험에서만 사용할 수 있습니다.

자세한 내용은 [요청 복사 및 제출](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)을 참조하십시오.

## 기존 초안에서 초안 및 요청 만들기

요청의 초안을 만든 다음 초안으로 돌아가 나중에 요청으로 제출할 수 있습니다.

새 요청 경험에서만 사용할 수 있습니다.

지침은 [초안에서 요청 만들기](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md)를 참조하십시오.

</div>


