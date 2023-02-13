---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 보내기 [!DNL Adobe Workfront] 실제 시간 업데이트 [!DNL Anaplan] 목록 항목
description: 이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트를 [!DNL Anaplan] 예산 목록 항목. 이 정보를 공유하면 다음과 같은 비용 최적화 및 재무 분석을 보다 효과적으로 활용할 수 있습니다 [!DNL Anaplan] 을 참조하십시오.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# 보내기 [!DNL Adobe Workfront] 실제 시간 업데이트 [!DNL Anaplan] 목록 항목

이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트를 [!DNL Anaplan] 예산 목록 항목. 이 정보를 공유하면 다음과 같은 비용 최적화 및 재무 분석을 보다 효과적으로 활용할 수 있습니다 [!DNL Anaplan] 을 참조하십시오.

이 시나리오 템플릿은 지난 3개월 동안 활성 프로젝트에 기록된 프로젝트, 일 및 역할별로 요약된 시간 목록을 제공합니다.

>[!IMPORTANT]
>
>이 문서에서 &quot;캠페인&quot;은 이 시나리오가 나타내며 [!DNL Workfront Fusion] Adobe Campaign 커넥터 또는 최근에 사용하지 않는 커넥터 [!UICONTROL 캠페인] 개체 [!DNL Workfront].

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

&#42;&#42;에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 이벤트 트리거

이 시나리오는 15분마다 실행되도록 예약되어 있습니다.

## 예상됨 [!DNL Workfront] 구성

에 다음 항목이 있어야 합니다. [!DNL Workfront] 이 시나리오를 사용하려면 다음을 수행하십시오.

* 의 사용자 프로필 [!DNL Workfront] 명명된 이름 **[!UICONTROL Anaplan 통합]**&#x200B;에는 시스템 관리자 권한이 있습니다.

   사용자 만들기에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 예상됨 [!DNL Anaplan] 구성

에 다음 항목이 있어야 합니다. [!DNL Anaplan] 이 시나리오를 사용하려면 다음을 수행하십시오.

* 의 사용자 프로필 [!DNL Anaplan] 명명된 이름 **[!UICONTROL [!DNL Workfront ]통합]**&#x200B;에는 시스템 관리자 권한이 있습니다.
* 다음 [!DNL Anaplan] 이 시나리오에 사용할 모델입니다.
* 내 목록 [!DNL Anaplan] 이 시나리오에 사용할 모델입니다.
* 의 파일 [!DNL Anaplan] 명명된 이름 **[!UICONTROL Anaplan 실제 시간 가져오기]** 여기에는 다음 열이 순서대로 포함됩니다.

   1. [!UICONTROL Workfront 프로젝트 GUID]

   2. [!UICONTROL 시간]

   3. [!UICONTROL 예상 비용 시간]

   4. [!UICONTROL 시작 날짜]

   5. [!UICONTROL 역할 이름]

   6. [!UICONTROL 캠페인 이름]

   7. [!UICONTROL [!DNL Anaplan] 목록 항목 ID]
   을(를) 준비하려면 [!DNL Anaplan] 실제 경비 보고서 파일:

   1. 다음 내용을 복사하여 텍스트 편집기에 붙여넣습니다. [!DNL Excel]
   1. 파일을 CSV 형식으로 저장
   1. 파일을 업로드 위치 [!DNL Anaplan].

      자세한 내용은 [!DNL Anaplan] 파일에서 모듈로 데이터를 가져오는 방법에 대한 설명서입니다.

   1. 파일에 지정한 이름을 메모하십시오. 배포 중에 사용됩니다. [!UICONTROL 융착] 시나리오 템플릿.

   CSV 컨텐츠 예

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL 프로젝트 실제 시간 가져오기]** 파일 업로드에서 전달된 데이터 가져오기를 실행하도록 준비된 프로세스입니다.

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서.

## 배포 대상 [!DNL Workfront Fusion]

다음 단계를 완료하여 이 통합 시나리오를 [!DNL Fusion] 계정이 필요합니다. 이 작업은 필요한 을 완료한 후에만 수행해야 합니다 [!DNL Workfront] 및 [!DNL Anaplan] 구성.

1. 로 이동합니다 [!UICONTROL 템플릿] 메뉴 [!DNL Workfront Fusion] 을 클릭하고 **[!UICONTROL 에 Workfront 실제 시간 업데이트를 보냅니다. [!DNL Anaplan] 목록 항목]** 시나리오 템플릿.
1. 다음 변수에 대한 변수 값을 바꿉니다 [!DNL Anaplan] 변수:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>변수 이름</th> 
      <th>값을 다음으로 바꾸기</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 작업 공간 ID]</td> 
      <td>작업 공간의 ID입니다 [!DNL Anaplan] 계정이 필요합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 모델 ID] </td> 
      <td>모델의 ID입니다 [!DNL Anaplan] 계정 및 선택한 작업 공간입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign 목록 이름]</td> 
      <td>목록의 이름 [!DNL Anaplan] 계정 및 선택한 작업 영역 및 모델.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 파일 이름: 실제 시간 가져오기]</td> 
      <td> <p>프로젝트 실제 시간 데이터를 받을 파일의 이름입니다.</p> <p> (예: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 프로세스 이름: 실제 시간 가져오기]</td> 
      <td> <p>프로젝트 시간 데이터 가져오기를 실행할 프로세스의 이름입니다.</p> <p>(예: WF Int - 역할별 프로젝트 시간 로드)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] 하위 도메인]</td> 
      <td>사용자의 하위 도메인 [!DNL Workfront] 계정이 필요합니다. 링크를 다시 만드는 데 사용됩니다 [!DNL Workfront] 생성할 수 있는 참고의 프로젝트.</td> 
     </tr> 
    </tbody> 
   </table>

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설정 설명서입니다.

1. 선택 또는 추가 [!DNL Anaplan] 연결 프로필입니다.
1. 나머지 항목 모두 업데이트 [!DNL Anaplan] 을 사용하는 모듈 [!DNL Anaplan] 연결 메시지가 표시되면
1. 선택 또는 추가 [!DNL Workfront] 연결 프로필입니다.
1. 나머지 항목 모두 업데이트 [!DNL Workfront] 을 사용하는 모듈 [!DNL Workfront] 연결 메시지가 표시되면

## 기타 권장 시나리오 템플릿

이 시나리오 템플릿은 다음과 같은 비용 최적화 시나리오 템플릿으로 배포될 수도 있습니다.

* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 프로젝트 업데이트 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 비용 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

예산 요청 연결에 대한 추가 시나리오:

* [[!UICONTROL 만들기 [!DNL Anaplan] 목록 항목 [!DNL Adobe Workfront] 예산 요청]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 적용 [!DNL Anaplan] 에 예산 할당 [!DNL Adobe Workfront] 프로젝트]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

캠페인 요청 연결에 대한 추가 시나리오:

* [[!UICONTROL 만들기 [!DNL Anaplan] 목록 항목 [!DNL Adobe Workfront] 캠페인 요청]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 적용 [!DNL Anaplan] 에 예산 할당 [!DNL Adobe Workfront] 캠페인 요청 또는 캠페인 프로젝트]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
