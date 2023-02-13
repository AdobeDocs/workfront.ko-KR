---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 만들기 [!DNL Anaplan] 목록 항목 [!DNL Adobe Workfront] 예산 요청
description: 이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트(캠페인)와 [!DNL Anaplan] 예산 목록 항목. 이 작업은 예산 요청을 [!DNL Workfront] 자금을 받아야 하는 프로젝트. 이 시나리오는 처리되지 않은 예산 요청을 확인한 다음, 프로세스를 실행하여 [!DNL Anaplan] Anaplan에서 예산 할당 프로세스를 시작할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 1%

---

# 만들기 [!DNL Anaplan] 목록 항목 [!DNL Adobe Workfront] 예산 요청

이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트(캠페인)와 [!DNL Anaplan] 예산 목록 항목. 이 작업은 예산 요청을 [!DNL Workfront] 자금을 받아야 하는 프로젝트. 이 시나리오는 처리되지 않은 예산 요청을 확인한 다음, 프로세스를 실행하여 [!DNL Anaplan] 에서 예산 할당 프로세스를 시작합니다. [!DNL Anaplan].

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
   <td role="rowheader" [!DNL>Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>작업 자동화 및 통합을 위한 [!UICONTROL Workfront Fusion] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr>
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

&#42;&#42;에 대한 자세한 정보[!DNL  Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 이벤트 트리거

이 시나리오는 15분마다 실행되도록 예약되어 있습니다.

## 예상됨 [!DNL Workfront] 구성

에 다음 항목이 있어야 합니다. [!DNL Workfront] 이 시나리오를 사용하려면 다음을 수행하십시오.

* 의 사용자 프로필 [!DNL Workfront] 명명된 *[!UICONTROL *[!DNL Anaplan] 통합]** 시스템 관리자 권한이 있습니다.

   사용자 만들기에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL 예산 요청]** 에 첨부된 사용자 지정 양식 [!UICONTROL 요청] 개체.

   데이터 매핑에 도움이 되도록 다음 필수 필드를 사용자 지정 양식에 포함해야 합니다 [!DNL Anaplan]:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>필드 이름</th> 
     <th>필드 유형</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL 예산 요청 유형]</td> 
     <td> <p>[!UICONTROL 드롭다운]</p> <p>옵션:</p> 
      <ul> 
       <li> <p>[!UICONTROL 자금 조달 조정]</p> </li> 
       <li> <p>[!UICONTROL 초기 자금 조달]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Labor Fund]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Expense Fund]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

   사용자 지정 양식 만들기에 대한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* 자금을 조달해야 하는 캠페인 및 기타 프로젝트를 나타내는 프로젝트 템플릿이며 [!UICONTROL 예산 요청] 큐 항목. 다음 [!UICONTROL 예산 요청] 큐 항목이 [!UICONTROL 예산 요청] 사용자 지정 양식입니다.
* A **[!UICONTROL 캠페인 개요]** 프로젝트 개체의 형식입니다.

   이 양식에는 다음 필드가 포함되어야 합니다.

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL 리치 텍스트 필드]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL 리치 텍스트 필드]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target 대상]</td> 
     <td> <p>[!UICONTROL 드롭다운]</p> <p>프로세스에 맞는 옵션을 포함합니다.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   사용자 지정 양식 만들기에 대한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## 예상됨 [!DNL Anaplan] 구성

에 다음 항목이 있어야 합니다. [!DNL Anaplan] 이 시나리오를 사용하려면 다음을 수행하십시오.

* 의 사용자 프로필 [!DNL Anaplan] 명명된 이름 **[!UICONTROL [!DNL Workfront]통합]**&#x200B;에는 시스템 관리자 권한이 있습니다.
* 다음 [!DNL Anaplan] 이 시나리오에 사용할 모델입니다.
* 내 목록 [!DNL Anaplan] 캠페인 예산을 캡처하는 모델.

   목록의 모듈은 다음 속성 수신을 지원해야 합니다.

   * [!UICONTROL Workfront 프로젝트 GUID]
   * [!UICONTROL 캠페인 이름]
   * [!UICONTROL 요청된 인건비]
   * [!UICONTROL 요청된 비용 자금]
   * [!UICONTROL 예산 요청 유형]
   * [!UICONTROL 자금 조달 조정 사유]

   이 목록 및 모듈은 [!DNL Anaplan]예산을 설정하고 예산 목록 항목을 다시 동기화할 준비가 되었는지 알려주는 기능 등 [!DNL Workfront].

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서.

## 배포 대상 [!DNL Workfront Fusion]

다음 단계를 완료하여 이 통합 시나리오를 [!DNL Fusion] 계정이 필요합니다. 이 작업은 필요한 을 완료한 후에만 수행해야 합니다 [!DNL Workfront] 및 [!DNL Anaplan] 구성.

1. 로 이동합니다 [!UICONTROL 템플릿] 메뉴 [!DNL Workfront Fusion] 을 클릭하고 **[!UICONTROL 만들기 [!DNL Anaplan] Workfront 예산 요청의 목록 항목]** 시나리오 템플릿.
1. 다음 변수에 대한 변수 값을 바꿉니다 [!DNL Anaplan] 변수:

   | 변수 이름 | 값을 다음으로 바꾸기 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] 작업 공간 ID] | 작업 공간의 ID입니다 [!DNL Anaplan] 계정이 필요합니다. |
   | [!UICONTROL [!DNL Anaplan] 모델 ID] | 모델의 ID입니다 [!DNL Anaplan] 계정 및 선택한 작업 공간입니다. |
   | [!UICONTROL [!DNL Anaplan] 모듈 이름] | 선택한 항목에서 캠페인 속성을 설명하는 모듈의 이름입니다 [!DNL Anaplan] 목록. |
   | [!UICONTROL 캠페인 목록 이름] | 목록의 이름 [!DNL Anaplan] 계정 및 선택한 작업 영역 및 모델. |

   {style=&quot;table-layout:auto&quot;}

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설정 설명서입니다.

1. 선택 또는 추가 [!DNL Anaplan] 연결 프로필입니다.
1. 나머지 항목 모두 업데이트 [!DNL Anaplan] 을 사용하는 모듈 [!DNL Anaplan] 연결 메시지가 표시되면
1. 선택 또는 추가 [!DNL Workfront] 연결 프로필입니다.

   템플릿을 배포한 후 기본 매핑된 필드를 (으)로 변경하려는 경우 필드 속성 값에서 사용자 지정 필드 참조를 추가하거나 제거하기 위해 업데이트할 모듈입니다 [!DNL Anaplan].

1. 나머지 항목 모두 업데이트 [!DNL Workfront] 을 사용하는 모듈 [!DNL Workfront] 연결 메시지가 표시되면

## 기타 권장 시나리오 템플릿

이 템플릿으로 표시되는 워크플로우를 완료하려면 다음 추가 템플릿도 배포해야 합니다.

* [[!UICONTROL 적용 [!DNL Anaplan] 에 예산 할당 [!DNL Adobe Workfront] 프로젝트]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

비용 최적화를 위한 추가 시나리오는 다음과 같습니다.

* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 프로젝트 업데이트 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 실제 시간 업데이트 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 보내기 [!DNL Adobe Workfront] 비용 [!DNL Anaplan] 목록 항목]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
