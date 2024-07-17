---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront] 캠페인 요청 또는 캠페인 프로젝트에  [!DNL Anaplan] 예산 할당 적용'
description: 이 통합 시나리오는  [!DNL Anaplan] 후  [!DNL Workfront]에 수행된 모든 예산 할당을 동기화합니다. 시나리오에서는 연결된 모든 캠페인 예산 항목을 가져온 다음 예산 값이 변경된 경우 예산 값을 연결된 Workfront 프로젝트에 전달합니다.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# [!DNL Adobe Workfront] 캠페인 요청 또는 캠페인 프로젝트에 [!DNL Anaplan] 예산 할당 적용

이 통합 시나리오는 [!DNL Anaplan]에서 수행된 모든 예산 할당을 다시 [!DNL Workfront](으)로 동기화합니다. 시나리오에서는 연결된 모든 캠페인 예산 항목을 가져온 다음 예산 값이 변경된 경우 연결된 [!DNL Workfront] 프로젝트에 예산 값을 전달합니다.

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
   <td> <p>작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p> </td> 
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

* [!DNL Workfront]의 사용자 프로필(이름이 **[!DNL Anaplan Integration]**&#x200B;임)에 시스템 관리자 권한이 있습니다.

  [!DNL Workfront]에서 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

## [!DNL Anaplan] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Anaplan]에 다음 항목이 있어야 합니다.

* [!DNL Anaplan]의 사용자 프로필(이름이 **[!UICONTROL [!DNL Workfront]통합]**&#x200B;임)에 시스템 관리자 권한이 있습니다.
* 이 시나리오에 사용할 [!DNL Anaplan] 모델입니다.
* 캠페인 예산을 캡처하는 [!DNL Anaplan] 모델 내의 목록입니다.

  목록의 모듈은 다음 속성의 수신을 지원해야 합니다.

   * [!UICONTROL [!DNL Workfront] 요청 GUID]
   * [!UICONTROL [!DNL Workfront] 프로젝트 GUID]
   * [!UICONTROL 캠페인 이름]
   * [!UICONTROL 요청한 인건비]
   * [!UICONTROL 예상 매출]
   * [!UICONTROL 브랜드]

  이 목록 및 모듈에는 예산을 설정하고 예산 목록 항목을 다시 [!DNL Workfront]에 동기화할 준비가 되었음을 알리는 기능을 포함하여 [!DNL Anaplan]의 일반적인 기능에 필요한 추가 세부 정보가 저장되어야 합니다.

* [!DNL Anaplan]의 보기에서는 **[!UICONTROL Adobe Workfront의 Campaigns.Update Campaigns]**&#x200B;을(를) 호출했습니다.

  이 보기에는 다음 열이 순서대로 포함되어야 합니다.

   1. [!UICONTROL 항목 이름]

   2. [!UICONTROL [!DNL Workfront] 요청 GUID]

   3. [!UICONTROL [!DNL Workfront] 프로젝트 GUID]

   4. [!UICONTROL 캠페인 이름]

   5. [!UICONTROL 예산]

   6. [!UICONTROL 예상 매출]

   7. [!UICONTROL 브랜드]

  [!UICONTROL [!DNL Workfront] 프로젝트 GUID]이(가) 있는 항목과 예산 할당을 Workfront으로 전송해야 한다는 일부 표시기를 표시하려면 보기를 필터링해야 합니다.

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서를 참조하십시오.

## Workfront Fusion에 배포

다음 단계를 완료하여 이 통합 시나리오를 Fusion 계정에 배포합니다. 필요한 [!DNL Workfront] 및 [!DNL Anaplan] 구성을 완료한 후에만 이 작업을 수행해야 합니다.

1. [!DNL Workfront Fusion]의 [!UICONTROL 템플릿] 메뉴로 이동한 다음 **[!UICONTROL Workfront 캠페인 요청 및 프로젝트에 [!DNL Anaplan] 예산 할당 적용]** 시나리오 템플릿을 클릭합니다.
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
      <td>[!DNL Anaplan] 계정의 작업 영역 ID입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 모델 ID] </td> 
      <td>[!DNL Anaplan] 계정 및 선택한 작업 영역의 모델 ID.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 캠페인 목록 이름]</td> 
      <td>[!DNL Anaplan] 계정 및 선택한 작업 영역 및 모델의 목록 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 보기 이름]</td> 
      <td> <p>[!DNL Workfront](으)로 캠페인 예산을 전송할 준비가 된 내용이 포함된 보기의 이름입니다.</p> <p>(예: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설치 설명서를 참조하세요.

1. [!DNL Anaplan] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Anaplan] 모듈을 모두 [!DNL Anaplan] 연결로 업데이트합니다.
1. **[!UICONTROL CSV를 JSON 개체로 변환]** 모듈에서 CSV 열을 사용 가능한 JSON 개체에 매핑하는 새 데이터 구조를 추가합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Request GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. 메시지가 표시되면 이 시나리오 배포의 다른 모듈에 대한 이 데이터 구조를 선택합니다.
1. **[!UICONTROL 연결된 프로젝트 확인]** 모듈에서 [!DNL Workfront] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Workfront] 모듈을 모두 [!DNL Workfront] 연결로 업데이트합니다.

## 기타 권장 시나리오 템플릿

이 템플릿으로 표시되는 워크플로우를 완료하려면 다음 추가 템플릿도 배포해야 합니다.

* [[!UICONTROL 캠페인 요청에서  [!DNL Anaplan] 목록 항목 만들기 [!DNL Adobe Workfront] 3}]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

지출 최적화를 위한 추가 시나리오는 다음과 같습니다.

* [[!UICONTROL 목록 항목 [!DNL Anaplan] 에 대한  [!DNL Adobe Workfront] 프로젝트 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 목록 항목  [!DNL Anaplan] 에 대한  [!DNL Adobe Workfront] 실제 시간 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 목록 항목 [!DNL Anaplan] 에 경비 보내기 [!DNL Adobe Workfront] 경비]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
