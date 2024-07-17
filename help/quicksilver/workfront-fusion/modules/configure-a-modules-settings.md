---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion]에서 모듈 설정 구성'
description: 만드는 모든 모듈에 대한 설정을 구성해야 합니다.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]에서 모듈 설정 구성

만드는 모든 모듈에 대한 설정을 구성해야 합니다.

예를 들어 [[!DNL Dropbox] 모듈](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) 모듈에서는 파일을 업로드할 대상 폴더를 지정해야 합니다. [[!UICONTROL 이메일] 모듈](../../workfront-fusion/apps-and-their-modules/email-modules.md) 모듈의 경우 이메일을 보낼 이메일 주소를 입력해야 합니다.

>[!NOTE]
>
>모듈 설정 외에도 시나리오의 설정을 조정할 수도 있습니다. 시나리오 이름을 바꾸고, 일정을 변경하고, 다른 작업 중에서도 추가 설정을 지정할 수 있습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr>  
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 모듈의 설정 구성

1. 시나리오에 새 모듈을 추가합니다.

   또는

   [다음 위치에 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)에 설명된 대로 시나리오 편집기에서 모듈의 아이콘을 클릭합니다.

1. 모듈에 필요한 경우 [연결 개요](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)에 설명된 대로 해당 서비스의 등록된 사용자 계정에 대해 **[!UICONTROL 연결]**&#x200B;을 만듭니다.
1. 각 필드에 적절한 텍스트를 입력합니다.

   또는

   필드 오른쪽에 나타나는 경우 **[!UICONTROL 맵]**&#x200B;을 클릭한 다음 시나리오의 다른 모듈에서 항목을 매핑합니다.

   굵게 표시된 매개 변수가 필요합니다.

   [!DNL Workfront Fusion]에서 인식할 수 있는 다른 항목 데이터 형식(예: 날짜, 숫자 및 텍스트)에 대한 자세한 내용은 [Item 데이터 형식 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)을 참조하세요.

1. (조건부) 모듈에 표시하고 사용할 고급 옵션이 있으면 **[!UICONTROL 고급 설정 표시]**&#x200B;를 선택합니다.
