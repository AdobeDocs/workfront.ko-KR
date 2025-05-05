---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront] campaign 요청에서  [!DNL Anaplan] 목록 항목 만들기'
description: 이 통합 시나리오는  [!DNL Adobe Workfront] 프로젝트를  [!DNL Anaplan] 예산 목록 항목과 연결합니다.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 2%

---

# [!DNL Adobe Workfront] 캠페인 요청에서 [!DNL Anaplan] 목록 항목 만들기

이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트와 [!DNL Anaplan] 예산 목록 항목을 연결합니다.

이 시나리오는 요청 대기열에 추가된 새 캠페인 요청을 감시합니다. 캠페인 요청이 기록되는 즉시 [!DNL Anaplan]에 예산 항목이 추가되어 자금 조달 프로세스가 시작됩니다.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront] 계획*</td> 
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

&#42;&#42;라이선스 [!DNL Adobe Workfront Fusion]에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)를 참조하세요.

## 이벤트 트리거 중

이 시나리오는 15분마다 실행되도록 예약되어 있습니다.

## [!DNL Workfront] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Workfront]에 다음 항목이 있어야 합니다.

* [!DNL Workfront]의 사용자 프로필(이름이 **[!UICONTROL [!DNL Anaplan]통합]**&#x200B;임)에 시스템 관리자 권한이 있습니다.

  [!DNL Workfront]에서 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

* **[!UICONTROL Campaign Brief]** 사용자 지정 양식이 [!UICONTROL Request] 개체에 첨부되었습니다.

  Anaplan에 대한 데이터 매핑을 지원하려면 사용자 정의 양식에 다음 필수 필드를 포함해야 합니다.

  | 필드 이름 | 필드 유형 |
  |---|---|
  | [!UICONTROL 총 요청 자금] |   |
  | [!UICONTROL 요청한 인건비] |   |
  | [!UICONTROL 요청된 경비 자금] |   |
  | [!UICONTROL 을(를) [!DNL Anaplan]] (으)로 보냄 | 확인란 |

  양식에 다음 옵션 필드가 있을 수 있습니다. 이 시나리오는 위의 필드만 매핑하지만, 캠페인 브리핑의 추가 필드를 매핑할 수 있습니다.

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
     <td role="rowheader">시장 시작 날짜의 </td> 
     <td>일자 </td> 
    </tr> 
    <tr> 
     <td role="rowheader">시장 종료 날짜의 </td> 
     <td>일자</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL 캠페인 개요]</td> 
     <td>단락 텍스트 필드</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL 키 메시지]</td> 
     <td>단락 텍스트 필드</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>드롭다운</p> <p>프로세스에 맞는 옵션을 포함합니다.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

* 새 캠페인 요청을 캡처하기 위한 요청 대기열로 설정된 프로젝트. [!UICONTROL 캠페인 개요] 양식을 이러한 요청에 첨부해야 합니다.

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
   * [!UICONTROL 요청된 경비 자금]
   * [!UICONTROL 예산 요청 유형]

  이 목록 및 모듈에는 예산을 설정하고 예산 목록 항목을 다시 [!DNL Workfront]에 동기화할 준비가 되었음을 알리는 기능을 포함하여 [!DNL Anaplan]의 일반적인 기능에 필요한 추가 세부 정보가 저장되어야 합니다.

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서를 참조하십시오.

## [!DNL Workfront Fusion]에 배포 중

[!DNL Fusion] 계정에 이 통합 시나리오를 배포하려면 다음 단계를 완료하십시오. 필요한 [!DNL Workfront] 및 [!DNL Anaplan] 구성을 완료한 후에만 이 작업을 수행해야 합니다.

1. [!DNL Workfront Fusion]의 [!UICONTROL 템플릿] 메뉴로 이동한 다음 **[!UICONTROL Workfront 캠페인 요청에서 [!DNL Anaplan] 목록 항목 만들기]** 시나리오 템플릿을 클릭합니다.
1. 다음 [!DNL Anaplan]개 변수에 대한 변수 값을 바꿉니다.

   | 변수 이름 | 값 바꾸기 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | [!DNL Anaplan] 계정의 작업 영역 ID입니다. |
   | [!UICONTROL [!DNL Anaplan] 모델 ID] | [!DNL Anaplan] 계정 및 선택한 작업 영역의 모델 ID. |
   | [!UICONTROL [!DNL Anaplan] 모듈 이름] | 선택한 [!DNL Anaplan] 목록의 캠페인 특성을 설명하는 모듈의 이름입니다. |
   | [!UICONTROL 캠페인 목록 이름] | [!DNL Anaplan] 계정 및 선택한 작업 영역 및 모델의 목록 이름입니다. |

   {style="table-layout:auto"}

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설치 설명서를 참조하세요.

1. [!DNL Anaplan] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Anaplan] 모듈을 모두 [!DNL Anaplan] 연결로 업데이트합니다.
1. [!DNL Workfront] 연결 프로필을 선택하거나 추가하십시오.

   템플릿을 배포한 후 기본 매핑된 필드를 [!DNL Anaplan] (으)로 변경하려는 경우 필드 속성 값에서 사용자 지정 필드 참조를 추가하거나 제거하기 위해 업데이트하는 모듈입니다.

1. 메시지가 표시되면 나머지 [!DNL Workfront] 모듈을 모두 [!DNL Workfront] 연결로 업데이트합니다.

## 기타 권장 시나리오 템플릿

이 템플릿으로 표시되는 워크플로우를 완료하려면 다음 추가 템플릿도 배포해야 합니다.

* [[!UICONTROL 캠페인 요청 또는 캠페인 프로젝트에  [!DNL Anaplan] 예산 할당 적용 [!DNL Adobe Workfront] 3&rbrace;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

지출 최적화를 위한 추가 시나리오는 다음과 같습니다.

* [[!UICONTROL 목록 항목 [!DNL Anaplan] 에 대한  [!DNL Adobe Workfront] 프로젝트 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 목록 항목  [!DNL Anaplan] 에 대한  [!DNL Adobe Workfront] 실제 시간 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 목록 항목 [!DNL Anaplan] 에 경비 보내기 [!DNL Adobe Workfront] 경비]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
