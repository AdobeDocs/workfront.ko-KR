---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 적용 [!DNL Anaplan] 에 예산 할당 [!DNL Adobe Workfront] 프로젝트
description: 이 통합 시나리오에서는 [!DNL Anaplan] 뒤로 [!DNL Workfront]. 시나리오는 연결된 모든 캠페인 예산 항목을 가져온 다음 예산 값이 변경된 경우 연결된 Workfront 프로젝트에 예산 값을 전달합니다.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# 적용 [!DNL Anaplan] 에 예산 할당 [!DNL Adobe Workfront] 프로젝트

이 통합 시나리오에서는 [!DNL Anaplan] 뒤로 [!DNL Workfront]. 시나리오는 연결된 모든 캠페인 예산 항목을 가져온 다음, 예산된 값을 연결된 항목에 전달합니다 [!DNL Workfront] 예산 값이 변경된 경우 프로젝트

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
   <td> <p>작업 자동화 및 통합을 위한 [!UICONTROL Workfront Fusion] </p> </td> 
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

* 의 사용자 프로필 [!DNL Workfront] 명명된 이름 **Anaplan 통합**&#x200B;에는 시스템 관리자 권한이 있습니다.

   사용자 만들기에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 예상됨 [!DNL Anaplan] 구성

에 다음 항목이 있어야 합니다. [!DNL Anaplan] 이 시나리오를 사용하려면 다음을 수행하십시오.

* 의 사용자 프로필 [!DNL Anaplan] 명명된 이름 **[!DNL Workfront]통합**&#x200B;에는 시스템 관리자 권한이 있습니다.
* 다음 [!DNL Anaplan] 이 시나리오에 사용할 모델입니다.
* 내 목록 [!DNL Anaplan] 캠페인 예산을 캡처하는 모델.

   목록의 모듈은 다음 속성 수신을 지원해야 합니다.

   * [!UICONTROL Workfront 프로젝트 GUID]
   * [!UICONTROL 캠페인 이름]
   * [!UICONTROL 요청된 인건비]
   * [!UICONTROL 예상 매출]
   * [!UICONTROL 브랜드]

   이 목록 및 모듈은 [!DNL Anaplan]예산을 설정하고 예산 목록 항목을 다시 동기화할 준비가 되었는지 알려주는 기능 등 [!DNL Workfront].

* 의 보기 [!DNL Anaplan] 명명된 이름 **[!UICONTROL Campaigns.Adobe Workfront에서 캠페인 업데이트]**.

   이 보기는 다음 열을 순서대로 포함해야 합니다.

   1. [!UICONTROL 항목 이름]

   2. [!UICONTROL [!DNL Workfront] 프로젝트 GUID]

   3. [!UICONTROL 캠페인 이름]

   4. [!UICONTROL 예산]

   5. [!UICONTROL 예상 매출]

   6. [!UICONTROL 브랜드]
   보기는 를 포함하는 항목을 표시하도록 필터링해야 합니다 [!UICONTROL [!DNL Workfront] 프로젝트 GUID] 그리고 예산 할당이 전송되어야 하는 몇 가지 지표 [!DNL Workfront].

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서.

## 배포 대상 [!DNL Workfront Fusion]

다음 단계를 완료하여 이 통합 시나리오를 [!DNL Fusion] 계정이 필요합니다. 이 작업은 필요한 을 완료한 후에만 수행해야 합니다 [!DNL Workfront] 및 [!DNL Anaplan] 구성.

1. 로 이동합니다 [!UICONTROL 템플릿] 메뉴 [!DNL Workfront Fusion] 을 클릭하고 **[!UICONTROL 적용 [!DNL Anaplan] Workfront 프로젝트에 대한 예산 할당]** 시나리오 템플릿.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 모듈 이름]</td> 
      <td>선택한 항목에서 캠페인 속성을 설명하는 모듈의 이름입니다 [!DNL Anaplan] 목록.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign 목록 이름]</td> 
      <td>목록의 이름 [!DNL Anaplan] 계정 및 선택한 작업 영역 및 모델.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 이름 보기]</td> 
      <td> <p>전송할 준비 캠페인 예산이 포함된 보기의 이름입니다. [!DNL Workfront].</p> <p>(예: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설정 설명서입니다.

1. 선택 또는 추가 [!DNL Anaplan] 연결 프로필입니다.
1. 나머지 항목 모두 업데이트 [!DNL Anaplan] 을 사용하는 모듈 [!DNL Anaplan] 연결 메시지가 표시되면
1. 설정 **[!UICONTROL CSV를 JSON 개체 모듈로 변환]**, 사용 가능한 JSON 개체에 CSV 열을 매핑하려면 새 데이터 구조를 추가합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 메시지가 표시되면 이 시나리오 배포의 다른 모듈에 대해 이 데이터 구조를 선택합니다.
1. 설정 **[!UICONTROL 연결된 프로젝트 확인]** 모듈, 선택 또는 추가 [!DNL Workfront] 연결 프로필입니다.
1. 나머지 항목 모두 업데이트 [!DNL Workfront] 을 사용하는 모듈 [!DNL Workfront] 연결 메시지가 표시되면

## 기타 권장 시나리오 템플릿

이 템플릿으로 표시되는 워크플로우를 완료하려면 다음 추가 템플릿도 배포해야 합니다.

* [[!UICONTROL 만들기 [!DNL Anaplan] 목록 항목 [!DNL Adobe Workfront] 예산 요청]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

비용 최적화를 위한 추가 시나리오는 다음과 같습니다.

* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 프로젝트 업데이트 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 실제 시간 업데이트 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 비용 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
