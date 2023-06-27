---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion에서 트리거 모듈이 시작되는 위치 선택
description: 일부 트리거 모듈을 사용하면 번들 검색을 시작할 첫 번째 번들을 선택할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# 트리거 모듈의 시작 위치 선택 [!DNL Adobe Workfront Fusion]

일부 트리거 모듈을 사용하면 번들 검색을 시작할 첫 번째 번들을 선택할 수 있습니다.

특정 날짜 이후에 모든 번들을 검색할지 아니면 번들만 검색할지 지정할 수도 있습니다.

트리거 모듈에 대한 자세한 내용은 섹션을 참조하십시오 [트리거 모듈](../../workfront-fusion/modules/module-types.md#triggers) 이 문서에서 [모듈 유형](../../workfront-fusion/modules/module-types.md).

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
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 트리거 모듈의 시작 위치 선택

1. 트리거 모듈을 저장합니다.

   또는

   에 설명된 대로 트리거 모듈의 설정을 변경합니다. [에서 모듈 설정 구성 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   또는

   에서 트리거 모듈의 아이콘을 마우스 오른쪽 단추로 클릭합니다. [!UICONTROL 시나리오 편집기]에 설명된 대로 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 에서 옵션 선택 **[!UICONTROL 시작할 위치 선택]** 상자가 나타납니다.

   ![](assets/choose-where-to-start-350x346.jpg)

   표시되는 옵션은 제공된 서비스의 가능성에 따라 다릅니다. 여기에는 다음이 포함될 수 있습니다.

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL From now on] (기본값)</td>
            <td>이제부터 추가 또는 업데이트된 모든 번들(설정에 따라 다름)을 검색합니다.</td>
        </tr>
        <tr>
            <td>[!UICONTROL 특정 날짜 이후]</td>
            <td>지정된 날짜/시간 이후에 추가되거나 업데이트된 모든 번들(설정에 따라 다름)을 검색합니다.</td>
        </tr>
        <tr>
            <td>[!UICONTROL ID가 특정 값보다 크거나 같음]</td>
            <td>ID가 지정된 ID보다 크거나 같은 모든 번들을 검색합니다.</td> 
        </tr>
        <tr>
            <td>[!UICONTROL All bundles]</td>
            <td>사용 가능한 모든 번들 검색</td>
        </tr>
        <tr>
            <td>[!UICONTROL 첫 번째 번들 선택]</td>
            <td>번들 검색을 시작할 첫 번째 번들을 선택할 수 있습니다.</td>
        </tr>
   </table>
