---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Anaplan] 목록 항목으로  [!DNL Adobe Workfront] 경비 보내기'
description: 이 통합 시나리오는  [!DNL Adobe Workfront] 프로젝트의 경비 관련 세부 정보를  [!DNL Anaplan] 예산 목록 항목과 공유합니다. 이 정보를 공유하면  [!DNL Anaplan] 이(가) 제공하는 지출 최적화 및 재무 분석을 더 잘 활용할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# [!DNL Adobe Workfront] 경비를 [!DNL Anaplan] 목록 항목으로 보내기

이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트의 경비 관련 세부 정보를 [!DNL Anaplan] 예산 목록 항목과 공유합니다. 이 정보를 공유하면 [!DNL Anaplan]에서 제공하는 지출 최적화 및 재무 분석을 더 잘 활용할 수 있습니다.

>[!IMPORTANT]
>
>이 문서의 &quot;캠페인&quot;은 이 시나리오가 나타내는 마케팅 캠페인 사용 사례를 참조합니다. [!DNL Workfront]에서 [!DNL Workfront Fusion] Adobe Campaign 커넥터 또는 최근에 더 이상 사용되지 않는 [!UICONTROL 캠페인] 개체에 연결할 수 없습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>작업 자동화 및 통합을 위한 Workfront Fusion </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구입해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

&#42;&#42;라이선스 [!DNL Adobe Workfront Fusion]에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 이벤트 트리거 중

이 시나리오는 15분마다 실행되도록 예약되어 있습니다.

## [!DNL Workfront] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Workfront]에 다음 항목이 있어야 합니다.

* 시스템 관리자 권한이 있는 [!DNL Workfront]의 사용자 프로필(이름: *[!UICONTROL *[!DNL Anaplan] 통합]**)입니다.

  [!DNL Workfront]에서 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

* [!DNL Anaplan]에 보낼 사용자 지정 데이터 값을 저장하기 위해 프로젝트 개체에 **[!UICONTROL Campaign Brief]** 사용자 지정 양식이 첨부되었습니다.

  양식에는 다음 필드가 포함되어야 합니다.

  | 필드 이름 | 필드 유형 |
  |---|---|
  | [!UICONTROL 마지막 전송 날짜] | 일자 |
  | [!UICONTROL 통합 정보] | 단락 텍스트 필드 |

  사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)을 참조하세요.

## [!DNL Anaplan] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Anaplan]에 다음 항목이 있어야 합니다.

* [!DNL Anaplan]의 사용자 프로필(이름이 **[!UICONTROL [!DNL Workfront]통합]**&#x200B;임)에 시스템 관리자 권한이 있습니다.
* 이 시나리오에 사용할 [!DNL Anaplan] 모델입니다.
* 캠페인 예산을 캡처할 [!DNL Anaplan] 모델 내의 목록입니다.
* 다음 열을 이 순서로 포함하는 **[!UICONTROL Anaplan 실제 경비 가져오기]** 파일:

   1. [!UICONTROL [!DNL Workfront] 경비 GUID]

   2. [!UICONTROL [!DNL Workfront] 프로젝트 GUID]

   3. [!UICONTROL 실제 금액]

   4. [!UICONTROL 설명]

   5. [!UICONTROL 경비 유형]

   6. [!UICONTROL 유효 날짜]

   7. [!UICONTROL 캠페인 이름]

   8. [!UICONTROL [!DNL Anaplan] 목록 항목 ID]

  [!UICONTROL [!DNL Anaplan] 실제 경비 가져오기] 파일을 준비하려면:

   1. 다음 내용을 복사하여 텍스트 편집기 또는 [!DNL Excel]에 붙여 넣습니다.
   1. 파일을 CSV 형식으로 저장합니다.
   1. 파일을 [!DNL Anaplan]에 업로드합니다.

      지침은 파일에서 모듈로 데이터를 가져오는 방법에 대한 [!DNL Anaplan] 설명서를 참조하십시오.

   1. 파일에 지정한 이름을 기록해 두십시오. 이 이름은 [!UICONTROL Fusion] 시나리오 템플릿을 배포하는 동안 사용됩니다.

  CSV 콘텐츠 예

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* 다음 열을 이 순서로 포함하는 **[!UICONTROL [!DNL Anaplan]계획된 경비 가져오기]** 파일:

   1. [!UICONTROL [!DNL Workfront] 경비 GUID]

   2. [!UICONTROL [!DNL Workfront] 프로젝트 GUID]

   3. [!UICONTROL 실제 금액]

   4. [!UICONTROL 설명]

   5. [!UICONTROL 경비 유형]

   6. [!UICONTROL 유효 날짜]

   7. [!UICONTROL 캠페인 이름]

   8. [!UICONTROL [!DNL Anaplan] 목록 항목 ID]

  [!UICONTROL [!DNL Anaplan] 계획된 경비 가져오기] 파일을 준비하려면:

   1. 다음 내용을 복사하여 텍스트 편집기 또는 [!DNL Excel]에 붙여 넣으십시오.
   1. 파일을 CSV 형식으로 저장
   1. 파일을 Anaplan에 업로드합니다.

      지침은 파일에서 모듈로 데이터를 가져오는 방법에 대한 [!DNL Anaplan] 설명서를 참조하십시오.

   1. 파일에 지정한 이름을 기록해 두십시오. 이 이름은 [!UICONTROL Fusion] 시나리오 템플릿을 배포하는 동안 사용됩니다.

  CSV 콘텐츠 예

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* 파일 업로드에 전달된 데이터 가져오기를 실행하기 위해 **[!UICONTROL 프로젝트 업데이트 가져오기]** 프로세스가 준비되었습니다.

>[!NOTE]
>
>계획된 비용과 실제 비용에 대한 가져오기 파일이 별도로 있으므로 계획된 날짜와 유효 날짜에 각각 독립적으로 보고할 수 있습니다.

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서를 참조하십시오.

## [!DNL Fusion]에 배포 중

[!DNL Fusion] 계정에 이 통합 시나리오를 배포하려면 다음 단계를 완료하십시오. 필요한 [!DNL Workfront] 및 [!DNL Anaplan] 구성을 완료한 후에만 이 작업을 수행해야 합니다.

1. [!DNL Workfront Fusion]의 [!UICONTROL 템플릿] 메뉴로 이동한 다음 **[!UICONTROL [!DNL Anaplan] 목록 항목으로 Workfront 경비 업데이트 보내기]** 시나리오 템플릿을 클릭합니다.
1. 다음 [!DNL Anaplan]개 변수에 대한 변수 값을 바꿉니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>변수 이름</th> 
      <th>값 바꾸기</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>이 시나리오에 사용할 [!DNL Anaplan] 계정의 작업 공간 ID입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 모델 ID] </td> 
      <td>[!DNL Anaplan] 계정의 모델 ID와 이 시나리오에 사용할 선택한 작업 영역입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 캠페인 목록 이름]</td> 
      <td>[!DNL Anaplan] 계정의 목록 이름 및 이 시나리오에 사용할 선택한 작업 영역 및 모델입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 파일 이름: 실제 비용 가져오기]</td> 
      <td> <p>프로젝트 실제 경비 데이터를 받을 파일의 이름입니다.</p> <p> (예: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 파일 이름: 계획된 경비 가져오기]</td> 
      <td> <p>프로젝트 계획 경비 데이터를 받을 파일의 이름입니다.</p> <p> (예: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 프로세스 이름: 프로젝트 업데이트 가져오기]</td> 
      <td> <p>프로젝트 경비 데이터 가져오기를 실행할 프로세스의 이름.</p> <p>(예: WF 정수 - 프로젝트 경비 로드)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설치 설명서를 참조하세요.

1. [!DNL Anaplan] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Anaplan] 모듈을 모두 [!DNL Anaplan] 연결로 업데이트합니다.
1. [!DNL Workfront] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Workfront] 모듈을 모두 [!DNL Workfront] 연결로 업데이트합니다.
1. **[!UICONTROL 실제 경비 CSV 빌드]** 모듈에서 프로젝트 특성을 CSV 열에 매핑하는 새 데이터 구조를 추가합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. **[!UICONTROL 계획된 비용 CSV 빌드]** 모듈에서 프로젝트 특성을 CSV 열에 매핑하는 새 데이터 구조를 추가합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## 기타 권장 시나리오 템플릿

이 시나리오 템플릿은 다음과 같은 비용 최적화 시나리오 템플릿을 보완하며, 이 시나리오 템플릿 또한 배포할 수 있습니다.

* [[!UICONTROL 목록 항목 [!DNL Anaplan] 에 대한  [!DNL Adobe Workfront] 프로젝트 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 목록 항목  [!DNL Anaplan] 에 대한  [!DNL Adobe Workfront] 실제 시간 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

예산 요청 연결을 위한 추가 시나리오:

* [[!UICONTROL 예산 요청에서  [!DNL Anaplan] 목록 항목 만들기 [!DNL Adobe Workfront] 3}]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 프로젝트에  [!DNL Anaplan] 예산 할당 적용 [!DNL Adobe Workfront] 프로젝트]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Campaign 요청 연결을 위한 추가 시나리오:

* [[!UICONTROL 캠페인 요청에서  [!DNL Anaplan] 목록 항목 만들기 [!DNL Adobe Workfront] 3}]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 캠페인 요청 또는 캠페인 프로젝트에  [!DNL Anaplan] 예산 할당 적용 [!DNL Adobe Workfront] 3}]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
