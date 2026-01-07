---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Anaplan] 프로젝트에  [!DNL Adobe Workfront] 예산 할당 적용'
description: 이 통합 시나리오는  [!DNL Anaplan] 후  [!DNL Workfront]에 수행된 모든 예산 할당을 동기화합니다. 시나리오에서는 연결된 모든 캠페인 예산 항목을 가져온 다음 예산 값이 변경된 경우 예산 값을 연결된 Workfront 프로젝트에 전달합니다.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 16%

---

# [!DNL Anaplan] 프로젝트에 [!DNL Adobe Workfront] 예산 할당 적용

이 통합 시나리오는 [!DNL Anaplan]에서 수행된 모든 예산 할당을 다시 [!DNL Workfront]&#x200B;(으)로 동기화합니다. 시나리오에서는 연결된 모든 캠페인 예산 항목을 가져온 다음 예산 값이 변경된 경우 예산 값을 연결된 [!DNL Workfront] 프로젝트에 전달합니다.

>[!IMPORTANT]
>
>이 문서의 &quot;캠페인&quot;은 이 시나리오가 나타내는 마케팅 캠페인 사용 사례를 참조합니다. [!DNL Workfront Fusion]에서 [!UICONTROL &#x200B; Adobe Campaign 커넥터 또는 최근에 더 이상 사용되지 않는 &#x200B;]캠페인[!DNL Workfront] 개체에 연결할 수 없습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>모든 Adobe Workfront 워크플로 패키지 및 모든 Adobe Workfront 자동화 및 통합 패키지</p><p>Workfront Ultimate</p><p>Workfront Prime 및 Select 패키지 및 Workfront Fusion 추가 구매.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p><p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion 라이선스</td> 
   <td>
   <p>작업 기반: Workfront Fusion 라이선스 요구 사항 없음</p>
   <p>커넥터 기반(이전): 작업 자동화 및 통합을 위한 Workfront Fusion </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>조직에 Workfront 자동화 및 통합이 포함되지 않은 Select 또는 Prime Workfront 패키지가 있는 경우 Adobe Workfront Fusion을 구매해야 합니다.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

이 테이블의 정보에 대한 자세한 내용은 [설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

Adobe Workfront Fusion 라이선스에 대한 자세한 내용은 [Adobe Workfront Fusion 라이선스](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)를 참조하십시오.

+++

## 이벤트 트리거 중

이 시나리오는 15분마다 실행되도록 예약되어 있습니다.

## [!DNL Workfront] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Workfront]에 다음 항목이 있어야 합니다.

* [!DNL Workfront]의 사용자 프로필(이름이 **Anaplan 통합**&#x200B;임)에 시스템 관리자 권한이 있습니다.

  [!DNL Workfront]에서 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

## [!DNL Anaplan] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Anaplan]에 다음 항목이 있어야 합니다.

* [!DNL Anaplan]의 사용자 프로필(이름이 **[!DNL Workfront]통합**&#x200B;임)에 시스템 관리자 권한이 있습니다.
* 이 시나리오에 사용할 [!DNL Anaplan] 모델입니다.
* 캠페인 예산을 캡처하는 [!DNL Anaplan] 모델 내의 목록입니다.

  목록의 모듈은 다음 속성의 수신을 지원해야 합니다.

   * [!UICONTROL Workfront 프로젝트 GUID]
   * [!UICONTROL 캠페인 이름]
   * [!UICONTROL 요청한 인건비]
   * [!UICONTROL 예상 매출]
   * [!UICONTROL 브랜드]

  이 목록 및 모듈에는 예산을 설정하고 예산 목록 항목을 다시 [!DNL Anaplan]에 동기화할 준비가 되었음을 알리는 기능을 포함하여 [!DNL Workfront]의 일반적인 기능에 필요한 추가 세부 정보가 저장되어야 합니다.

* [!DNL Anaplan]의 **[!UICONTROL Adobe Workfront의 Campaigns.Update Campaigns]** 보기.

  이 보기에는 다음 열이 순서대로 포함되어야 합니다.

   1. [!UICONTROL 항목 이름]

   2. [!UICONTROL [!DNL Workfront] 프로젝트 GUID]

   3. [!UICONTROL 캠페인 이름]

   4. [!UICONTROL 예산]

   5. [!UICONTROL 예상 매출]

   6. [!UICONTROL 브랜드]

  [!UICONTROL [!DNL Workfront] 프로젝트 GUID]이(가) 있는 항목과 예산 할당을 [!DNL Workfront]&#x200B;(으)로 전송해야 한다는 일부 표시기를 표시하려면 보기를 필터링해야 합니다.

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서를 참조하십시오.

## [!DNL Workfront Fusion]에 배포 중

[!DNL Fusion] 계정에 이 통합 시나리오를 배포하려면 다음 단계를 완료하십시오. 필요한 [!DNL Workfront] 및 [!DNL Anaplan] 구성을 완료한 후에만 이 작업을 수행해야 합니다.

1. [!UICONTROL 의 &#x200B;]템플릿[!DNL Workfront Fusion] 메뉴로 이동한 다음 **[!UICONTROL Workfront 프로젝트에 [!DNL Anaplan] 예산 할당 적용]** 시나리오 템플릿을 클릭합니다.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 모듈 이름]</td> 
      <td>선택한 [!DNL Anaplan] 목록의 캠페인 특성을 설명하는 모듈의 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 캠페인 목록 이름]</td> 
      <td>[!DNL Anaplan] 계정 및 선택한 작업 영역 및 모델의 목록 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 보기 이름]</td> 
      <td> <p>[!DNL Workfront] (으)로 캠페인 예산을 전송할 준비가 된 내용이 포함된 보기의 이름입니다.</p> <p>(예: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설치 설명서를 참조하세요.

1. [!DNL Anaplan] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Anaplan] 모듈을 모두 [!DNL Anaplan] 연결로 업데이트합니다.
1. **[!UICONTROL CSV를 JSON 개체 모듈로 변환]**&#x200B;에서 새 데이터 구조를 추가하여 CSV 열을 사용 가능한 JSON 개체에 매핑합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. 메시지가 표시되면 이 시나리오 배포의 다른 모듈에 대한 이 데이터 구조를 선택합니다.
1. **[!UICONTROL 연결된 프로젝트 확인]** 모듈에서 [!DNL Workfront] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Workfront] 모듈을 모두 [!DNL Workfront] 연결로 업데이트합니다.

## 기타 권장 시나리오 템플릿

이 템플릿으로 표시되는 워크플로우를 완료하려면 다음 추가 템플릿도 배포해야 합니다.

* [[!UICONTROL 예산 요청에서  [!DNL Anaplan] 목록 항목 만들기 [!DNL Adobe Workfront] 3&rbrace;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

지출 최적화를 위한 추가 시나리오는 다음과 같습니다.

* [[!UICONTROL 목록 항목 [!DNL Adobe Workfront] 에 대한  [!DNL Anaplan] 프로젝트 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 목록 항목  [!DNL Adobe Workfront] 에 대한  [!DNL Anaplan] 실제 시간 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 목록 항목 [!DNL Adobe Workfront] 에 경비 보내기 [!DNL Anaplan] 경비]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
