---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 보내기 [!DNL Adobe Workfront] 프로젝트 업데이트 [!DNL Anaplan] 목록 항목
description: 이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트를 [!DNL Anaplan] 예산 목록 항목. 이 정보를 공유하면 다음과 같은 비용 최적화 및 재무 분석을 보다 효과적으로 활용할 수 있습니다 [!DNL Anaplan] 을 참조하십시오.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# 보내기 [!DNL Adobe Workfront] 프로젝트 업데이트 [!DNL Anaplan] 목록 항목

이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트를 [!DNL Anaplan] 예산 목록 항목. 이 정보를 공유하면 다음과 같은 비용 최적화 및 재무 분석을 보다 효과적으로 활용할 수 있습니다 [!DNL Anaplan] 을 참조하십시오.

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
   <td> <p>작업 자동화 및 통합을 위한 Workfront Fusion </p> </td> 
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

* 의 사용자 프로필 [!DNL Workfront] 명명된 이름 **[!UICONTROL [!DNL Anaplan]통합]**&#x200B;에는 시스템 관리자 권한이 있습니다.

   사용자 만들기에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL 캠페인 개요]** 프로젝트 객체에 첨부된 사용자 정의 양식을 통해 Anaplan에 전송하도록 선택한 사용자 정의 데이터 값을 저장합니다.

   다음 필드는 사용자 지정 양식에 포함되어 Anaplan에 데이터 매핑에 도움이 될 수 있는 필드의 예를 나타내지만, 이 통합 시나리오에 필요하지 않습니다.

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>필드 이름</th> 
     <th>필드 유형</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>[!UICONTROL 날짜] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>[!UICONTROL 날짜]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign 개요]</td> 
     <td>[!UICONTROL 단락 텍스트 필드]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL 단락 텍스트 필드]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target 대상]</td> 
     <td> <p>[!UICONTROL 드롭다운]</p> <p>프로세스에 맞는 옵션을 포함합니다.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   사용자 지정 양식 만들기에 대한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## 예상됨 [!DNL Anaplan] 구성

에 다음 항목이 있어야 합니다. [!DNL Anaplan] 이 시나리오를 사용하려면 다음을 수행하십시오.

* 의 사용자 프로필 [!DNL Anaplan] 명명된 이름 **[!UICONTROL [!DNL Workfront]통합]**&#x200B;에는 시스템 관리자 권한이 있습니다.
* 다음 [!DNL Anaplan] 이 시나리오에 사용할 모델입니다.
* 내 목록 [!DNL Anaplan] 이 시나리오에 사용할 모델입니다.
* A **[!UICONTROL 프로젝트 업데이트 가져오기]** 다음 열이 들어 있는 파일을 순서대로 포함합니다.

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] 프로젝트 GUID]

3. [!UICONTROL 캠페인 이름]

4. [!UICONTROL 완료율]

5. [!UICONTROL 계획된 시작 일자]

6. [!UICONTROL 계획된 완료 일자]

7. [!UICONTROL 계획된 시간]

8. [!UICONTROL 계획된 비용]

9. [!UICONTROL 계획된 경비]

10. [!UICONTROL 실제 인건비]

11. [!UICONTROL 계획된 인건비]

12. [!UICONTROL 상태]

을(를) 준비하려면 [!UICONTROL [!DNL Anaplan] 계획된 경비 임포트] 파일:

1. 다음 내용을 복사하여 텍스트 편집기에 붙여넣습니다. [!DNL Excel]
1. 파일을 CSV 형식으로 저장
1. 파일을 Anaplan에 업로드합니다.

   자세한 내용은 [!DNL Anaplan] 파일에서 모듈로 데이터를 가져오는 방법에 대한 설명서입니다.

1. 파일에 지정한 이름을 메모하십시오. 배포 중에 사용됩니다. [!UICONTROL 융착] 시나리오 템플릿.

CSV 컨텐츠 예

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

1. [!UICONTROL 캠페인 개요]

2. [!UICONTROL 주요 메시지]

3. [!UICONTROL 시장 시작 일자]

4. [!UICONTROL 시장 종료 일자]

5. [!UICONTROL Target 대상]

매핑에 설정할 다른 필드도 포함합니다.

* A **[!UICONTROL 프로젝트 업데이트 가져오기]** 파일 업로드에서 전달된 데이터 가져오기를 실행하도록 준비된 프로세스입니다.

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서.

## 배포 대상 [!DNL Workfront Fusion]

다음 단계를 완료하여 이 통합 시나리오를 Fusion 계정에 배포합니다. 이 작업은 필요한 을 완료한 후에만 수행해야 합니다 [!DNL Workfront] 및 [!DNL Anaplan] 구성.

1. 로 이동합니다 [!UICONTROL 템플릿] 메뉴 [!DNL Workfront Fusion] 을 클릭하고 **[!UICONTROL Workfront 프로젝트 업데이트을에 보내기 [!DNL Anaplan] 목록 항목]** 시나리오 템플릿.
1. 다음 변수에 대한 변수 값을 바꿉니다 [!DNL Anaplan] 변수:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
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
      <td role="rowheader">[!UICONTROL 파일 이름: 프로젝트 업데이트 가져오기]</td> 
      <td>프로젝트 업데이트 데이터를 받을 파일의 이름입니다.<p>(예: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 프로세스 이름: 프로젝트 업데이트 가져오기]</td> 
      <td> <p>프로젝트 데이터 가져오기를 실행할 프로세스의 이름입니다.</p> <p>(예: WF Int - 캠페인 세부 사항 업데이트)</p> </td> 
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

   필터는 완료되지 않은 모든 연결된 프로젝트와 지난 29분 동안 완료된 프로젝트를 가져오도록 구성되어 있습니다. 빈도 [!DNL Fusion] 시나리오 템플릿이 배포되면 이 값을 업데이트할 수 있습니다.

1. 설정 **[!UICONTROL 프로젝트 빌드 CSV 업데이트]** 모듈, 새 데이터 구조를 추가하여 프로젝트 속성을 CSV 열에 매핑합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 나머지 항목 모두 업데이트 [!DNL Workfront] 을 사용하는 모듈 [!DNL Workfront] 연결 메시지가 표시되면

## 기타 권장 시나리오 템플릿

이 시나리오 템플릿은 다음과 같은 비용 최적화 시나리오 템플릿으로 배포될 수도 있습니다.

* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 실제 시간 업데이트 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 비용 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

예산 요청 연결에 대한 추가 시나리오:

* [[!UICONTROL 만들기 [!DNL Anaplan] 목록 항목 [!DNL Adobe Workfront] 예산 요청]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 적용 [!DNL Anaplan] 에 예산 할당 [!DNL Adobe Workfront] 프로젝트]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

캠페인 요청 연결에 대한 추가 시나리오:

* [[!UICONTROL 만들기 [!DNL Anaplan] 목록 항목 [!DNL Adobe Workfront] 캠페인 요청]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 적용 [!DNL Anaplan] 에 예산 할당 [!DNL Adobe Workfront] 캠페인 요청 또는 캠페인 프로젝트]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
