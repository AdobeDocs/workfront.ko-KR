---
title: Adobe Workfront Planning 요청 제출
description: 누군가가 Adobe Workfront Planning의 레코드 유형 페이지에서 요청 양식에 대한 링크를 귀하에게 공유하면 요청을 추가하여 요청 양식과 연관된 레코드 유형에 대한 레코드를 생성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '2091'
ht-degree: 0%

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

  이 문서에서는 Workfront의 요청 영역 또는 공유 링크에서 레코드 유형에 새 레코드를 추가하도록 요청을 제출하는 방법에 대해 설명합니다.
* 레코드 유형 페이지에서 새 레코드를 추가하거나 요청할 때 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.

Workfront 사용자와 외부 사용자는 Planning 레코드 유형에 요청을 제출하고 레코드를 생성할 수 있습니다. <!--double check on the external users-->

작업 영역 관리자가 요청 양식을 만들고 레코드 유형과 연결하는 방법에 대한 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront 계획<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td>
   <td>
<p>다음 Workfront 플랜 중 하나:</p>
<ul><li>선택</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p>
   </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td>
   <td>
<p>임의 </p>  
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td>
   <td>
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>External, Contributor, Light 또는 Standard 라이센스</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <p>Workfront 사용자인 경우 작업 영역 <span class="preview"> 및 레코드 종류</span>에 대한 이상의 권한을 봅니다.</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront의 계획 영역에 액세스하려면 다음 레이아웃 템플릿 구성이 있어야 합니다. </p>
<ul>
<li><p>프로덕션 환경에서는 시스템 관리자를 포함한 모든 사용자를 Planning이 포함된 레이아웃 템플릿에 할당해야 합니다.</p></li>
<li><div class="preview">
<p> 미리보기 환경에서 Light 또는 기여자 라이선스가 있는 사용자에게 Planning이 포함된 레이아웃 템플릿을 할당해야 합니다.
   <p>표준 사용자 및 시스템 관리자에게는 기본적으로 계획 영역이 활성화되어 있습니다.</p></div></li></ul>

<p> 하지만 Workfront Planning에 요청을 제출하는 데 계획 영역에 액세스할 필요는 없습니다. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

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
* 제출된 요청은 Workfront의 요청 영역에 있는 제출됨 섹션의 계획 탭에 표시됩니다.
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

1. **새 요청**&#x200B;을 클릭합니다.

   ![통합 Workfront 및 Planning 카드가 있는 새 요청 상자](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   **새 요청** 상자가 열리고 다음 정보가 표시됩니다.

   * 가장 최근에 액세스한 6개의 Workfront 요청 대기열 및 Planning 요청 양식이 최근 섹션에 표시됩니다.
   * 50개의 추가 Workfront 요청 큐 및 Planning 요청 양식이 **모든 요청 양식** 섹션에 알파벳 순서로 표시됩니다. 기본적으로 표시되지 않는 요청 대기열을 검색할 수 있습니다.

1. 다음 중 하나를 수행하십시오.

   * 최근 또는 모든 요청 양식 섹션에서 Planning 요청 양식 중 하나에 대한 카드를 누릅니다
   * 검색 상자에 Planning 요청 양식 이름을 입력한 다음 목록에 표시될 때 카드를 클릭합니다.

   요청 양식이 열립니다.

1. 요청 양식에서 사용할 수 있는 필드를 업데이트합니다. 빨간색 별표가 있는 필드는 필수입니다.
1. **제출**&#x200B;을 클릭합니다.

   요청 양식이 닫히고 **요청** 영역으로 돌아갑니다.

   양식이 제출되고 다음 사항이 발생합니다.

   * 요청 양식이 승인과 연결되어 있지 않은 경우 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 요청이 추가되고 양식에 연결된 레코드 유형에 새 레코드가 추가됩니다.

   * 요청 양식이 승인과 연결된 경우 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 요청이 추가됩니다. 새 레코드는 모든 승인자가 승인한 후에만 레코드 유형 페이지에 추가됩니다.

     자세한 내용은 [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)를 참조하십시오.

     ![통합 워크플로 계획 탭에 대한 토글이 포함된 요청 영역](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >하나 이상의 작업 영역에 액세스할 수 있는 모든 사용자는 요청 영역에서 계획 탭을 볼 수 있습니다. 볼 수 있는 권한 이상이 있는 작업 영역에 사용자 또는 다른 사람이 제출한 요청만 볼 수 있습니다. Workfront 관리자는 시스템의 작업 영역에 제출된 모든 요청을 볼 수 있습니다.

   * 요청은 소유자, 승인자 및 작업 영역에 대해 최소 보기 권한이 있는 사람에게만 표시됩니다.

   * 요청이 성공적으로 제출되었거나 검토를 위해 전송되었다는 인앱 및 이메일 알림을 받게 됩니다.
   * 요청 양식이 승인과 연결된 경우 승인자는 요청을 검토하고 승인하기 위한 인앱 및 이메일 알림을 수신합니다.

     >[!NOTE]
     >
     >이메일 및 인앱 알림은 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩될 때만 표시됩니다.
     >
     >이메일 확인 또는 승인 알림에 요청에 대한 링크가 있습니다.

1. (선택 사항) 확인 메시지에서 **요청 보기**&#x200B;를 클릭하여 요청을 열거나 **X** 아이콘을 클릭하여 확인을 닫습니다.

1. (선택 사항) 요청을 보려면 **요청** 영역에서 **계획** 탭을 클릭합니다.
Planning 요청 양식에 제출된 보기 액세스 권한이 있는 모든 요청이 목록에 표시됩니다.
1. (선택 사항) 다음 중 하나를 수행합니다.

   <div class="preview">

   * **필터**&#x200B;를 클릭하고 계획 탭에서 보려는 요청에 대한 조건을 추가하기 시작합니다.

     ![계획 요청 탭에서 필터 편집](assets/filters-editing-box-in-requests-planning-tab.png)

     다음 필드를 기준으로 필터링할 수 있습니다.

      * **Workspace**: 요청 양식과 연결된 작업 영역입니다.
      * **레코드 종류**: 요청 양식과 연결된 레코드 종류.
      * **시작 날짜**: 요청이 제출된 날짜입니다.
      * **요청 양식**: 요청을 제출하는 데 사용되는 요청 양식의 이름입니다.
      * **상태**: 요청의 상태입니다.
      * **입력한 사람**: 요청을 추가한 사용자의 이름입니다. Workfront 외부의 사용자와 함께 요청을 추가한 경우 **입력한 사람** 필드에 `N/A`이(가) 표시됩니다.

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

   ![요청 세부 정보 페이지](assets/request-details-page.png)

   </div>


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

1. **제출**&#x200B;을 클릭합니다.

   양식이 제출되고 다음 사항이 발생합니다.

   * 요청 양식이 승인과 연결되어 있지 않은 경우 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 요청이 추가되고 양식에 연결된 레코드 유형에 새 레코드가 추가됩니다.

   * 요청 양식이 승인과 연결된 경우 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 요청이 추가됩니다. 새 레코드는 모든 승인자가 승인한 후에만 레코드 유형 페이지에 추가됩니다.

     자세한 내용은 [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)를 참조하십시오.

     ![요청의 계획 탭](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >하나 이상의 작업 영역에 액세스할 수 있는 모든 사용자는 요청 영역에서 계획 탭을 볼 수 있습니다. 볼 수 있는 권한 이상이 있는 작업 영역에 사용자 또는 다른 사람이 제출한 요청만 볼 수 있습니다. Workfront 관리자는 시스템의 작업 영역에 제출된 모든 요청을 볼 수 있습니다. <!--ensure this is correct; asking team in slack-->

   * 요청이 성공적으로 제출되었거나 검토를 위해 전송되었다는 인앱 및 이메일 알림을 받게 됩니다.
   * 요청 양식이 승인과 연결된 경우 승인자는 요청을 검토하고 승인하기 위한 인앱 및 이메일 알림을 수신합니다.

     >[!NOTE]
     >
     >이메일 및 인앱 알림은 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩될 때만 표시됩니다.

1. (선택 사항) Workfront에서 요청을 열려면 **요청 보기**&#x200B;를 클릭합니다.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (선택 사항) **기본 메뉴** > **요청** > **계획** 탭을 클릭하여 요청을 확인한 다음 요청 이름을 클릭합니다.

   요청 세부 정보 페이지가 열립니다.

   ![요청 세부 정보 페이지](assets/request-details-page.png)

1. (조건부) 요청 양식이 승인과 연결되어 있지 않거나 요청이 승인된 경우 요청 이름을 클릭한 다음 **레코드** 필드의 레코드 이름을 클릭합니다.

   레코드의 페이지가 Workfront Planning에 열립니다.

   >[!TIP]
   >
   >* 레코드 이름이 요청 양식에 추가되지 않은 경우 요청의 레코드 필드에 있는 레코드 이름이 **제목 없음**&#x200B;으로 표시됩니다.
   >
   >* 요청 양식이 승인과 연결된 경우 요청 페이지에서 레코드에 액세스하려면 승인을 받아야 합니다.

1. (선택 사항) **레코드 종류**&#x200B;의 이름을 클릭합니다.

   Workfront Planning에서 레코드 유형 페이지가 열립니다.




