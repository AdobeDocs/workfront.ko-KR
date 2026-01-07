---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront] 목록 항목에  [!DNL Anaplan] 실제 시간 업데이트 보내기'
description: 이 통합 시나리오는  [!DNL Adobe Workfront] 프로젝트에서 캡처한 실제 시간 세부 정보를  [!DNL Anaplan] 예산 목록 항목과 공유합니다. 이 정보를 공유하면  [!DNL Anaplan] 이(가) 제공하는 지출 최적화 및 재무 분석을 더 잘 활용할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 15%

---

# [!DNL Adobe Workfront] 목록 항목으로 [!DNL Anaplan]개의 실제 시간 업데이트 보내기

이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트에서 캡처한 실제 시간 세부 정보를 [!DNL Anaplan] 예산 목록 항목과 공유합니다. 이 정보를 공유하면 [!DNL Anaplan]에서 제공하는 지출 최적화 및 재무 분석을 더 잘 활용할 수 있습니다.

이 시나리오 템플릿은 지난 3개월 동안 활성 프로젝트에 기록된 프로젝트, 일 및 역할별로 요약된 시간 목록을 제공합니다.

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

Adobe Workfront Fusion 라이선스에 대한 자세한 내용은 [Adobe Workfront Fusion 라이선스](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)를 참조하십시오.

+++

## 이벤트 트리거 중

이 시나리오는 15분마다 실행되도록 예약되어 있습니다.

## [!DNL Workfront] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Workfront]에 다음 항목이 있어야 합니다.

* [!DNL Workfront]의 사용자 프로필(이름이 **[!UICONTROL Anaplan 통합]**&#x200B;임)에 시스템 관리자 권한이 있습니다.

  [!DNL Workfront]에서 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

## [!DNL Anaplan] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Anaplan]에 다음 항목이 있어야 합니다.

* [!DNL Anaplan]의 사용자 프로필(이름이 **[!UICONTROL [!DNL Workfront]통합]**&#x200B;임)에 시스템 관리자 권한이 있습니다.
* 이 시나리오에 사용할 [!DNL Anaplan] 모델입니다.
* 이 시나리오에 사용할 [!DNL Anaplan] 모델 내의 목록입니다.
* [!DNL Anaplan]의 파일 **[!UICONTROL Anaplan 실제 시간 가져오기]**&#x200B;에 다음 열이 순서대로 포함되어 있습니다.

   1. [!UICONTROL Workfront 프로젝트 GUID]

   2. [!UICONTROL 시간]

   3. [!UICONTROL 시간 예상 비용]

   4. [!UICONTROL 시작 날짜]

   5. [!UICONTROL 역할 이름]

   6. [!UICONTROL 캠페인 이름]

   7. [!UICONTROL [!DNL Anaplan] 목록 항목 ID]

  [!DNL Anaplan] 실제 경비 보고서 파일을 준비하려면:

   1. 다음 내용을 복사하여 텍스트 편집기 또는 [!DNL Excel]에 붙여 넣으십시오.
   1. 파일을 CSV 형식으로 저장
   1. 파일을 [!DNL Anaplan]에 업로드합니다.

      지침은 파일에서 모듈로 데이터를 가져오는 방법에 대한 [!DNL Anaplan] 설명서를 참조하십시오.

   1. 파일에 지정한 이름을 기록해 두십시오. 이 이름은 [!UICONTROL Fusion] 시나리오 템플릿을 배포하는 동안 사용됩니다.

  CSV 콘텐츠 예

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* 파일 업로드에 전달된 데이터 가져오기를 실행하기 위해 **[!UICONTROL 프로젝트 실제 시간 가져오기]** 프로세스가 준비되었습니다.

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서를 참조하십시오.

## [!DNL Workfront Fusion]에 배포 중

[!DNL Fusion] 계정에 이 통합 시나리오를 배포하려면 다음 단계를 완료하십시오. 필요한 [!DNL Workfront] 및 [!DNL Anaplan] 구성을 완료한 후에만 이 작업을 수행해야 합니다.

1. [!UICONTROL 의 &#x200B;]템플릿[!DNL Workfront Fusion] 메뉴로 이동한 다음 **[!UICONTROL 목록 항목 [!DNL Anaplan]에 Workfront 실제 시간 업데이트 보내기]** 시나리오 템플릿을 클릭합니다.
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
      <td role="rowheader">[!UICONTROL 파일 이름: 실제 시간 가져오기]</td> 
      <td> <p>프로젝트 실제 근로시간 데이터를 받을 파일의 이름입니다.</p> <p> (예: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 프로세스 이름: 실제 시간 가져오기]</td> 
      <td> <p>프로젝트 시간 데이터 가져오기를 실행할 프로세스의 이름.</p> <p>(예: WF 정수 - 역할별 프로젝트 시간 로드)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] 하위 도메인]</td> 
      <td>[!DNL Workfront] 계정의 하위 도메인입니다. 생성된 메모에서 [!DNL Workfront] 프로젝트에 대한 링크를 다시 만드는 데 사용됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설치 설명서를 참조하세요.

1. [!DNL Anaplan] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Anaplan] 모듈을 모두 [!DNL Anaplan] 연결로 업데이트합니다.
1. [!DNL Workfront] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Workfront] 모듈을 모두 [!DNL Workfront] 연결로 업데이트합니다.

## 기타 권장 시나리오 템플릿

이 시나리오 템플릿은 다음과 같은 비용 최적화 시나리오 템플릿을 보완하며, 이 시나리오 템플릿 또한 배포할 수 있습니다.

* [[!UICONTROL 목록 항목 [!DNL Adobe Workfront] 에 대한  [!DNL Anaplan] 프로젝트 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 목록 항목 [!DNL Adobe Workfront] 에 경비 보내기 [!DNL Anaplan] 경비]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

예산 요청 연결을 위한 추가 시나리오:

* [[!UICONTROL 예산 요청에서  [!DNL Anaplan] 목록 항목 만들기 [!DNL Adobe Workfront] 3&rbrace;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 프로젝트에  [!DNL Anaplan] 예산 할당 적용 [!DNL Adobe Workfront] 프로젝트]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Campaign 요청 연결을 위한 추가 시나리오:

* [[!UICONTROL 캠페인 요청에서  [!DNL Anaplan] 목록 항목 만들기 [!DNL Adobe Workfront] 3&rbrace;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 캠페인 요청 또는 캠페인 프로젝트에  [!DNL Anaplan] 예산 할당 적용 [!DNL Adobe Workfront] 3&rbrace;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
