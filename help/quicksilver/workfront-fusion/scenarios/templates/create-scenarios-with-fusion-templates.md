---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion] 개의 템플릿을 사용하여 시나리오 만들기'
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 43b30244-f4a5-4036-939c-aff7827c21b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]개의 템플릿으로 시나리오 만들기

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [템플릿을 사용하여 시나리오 만들기](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-and-manage-templates/create-scenarios-with-fusion-templates.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe Workfront Fusion] 템플릿을 사용하면 기존 템플릿을 만들어 [!DNL Workfront Fusion] 시나리오의 시작점으로 사용할 수 있습니다.

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
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
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

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 전제 조건

템플릿을 사용하려면 먼저 템플릿을 만들어야 합니다.

## 템플릿에서 시나리오 만들기

1. 왼쪽 탐색 패널에서 **[!UICONTROL 템플릿]** 아이콘 ![](assets/fusion-template-icon.png)을(를) 클릭합니다.
1. 사용할 서식 파일이 포함된 탭을 클릭합니다(**[!UICONTROL 공개 서식 파일]** 또는 **[!UICONTROL 팀 서식 파일]**).
1. 시나리오 작성을 시작하는 데 사용할 템플릿을 클릭합니다. 검색 기능을 사용하여 템플릿 이름 또는 템플릿에 포함된 앱 이름으로 템플릿을 찾을 수 있습니다.
1. (조건부) 두 개 이상의 조직 또는 팀의 구성원인 경우 시나리오를 만들 조직 또는 팀을 선택하고 **[!UICONTROL 계속]**&#x200B;을 클릭합니다.
1. (조건부) 템플릿이 [!UICONTROL 마법사]로 구성된 경우 나타나는 메시지에 따라 시나리오를 구성하십시오. 각 프롬프트에서 **[!UICONTROL 계속]**&#x200B;을 클릭하여 확인하십시오.

   >[!NOTE]
   >
   >템플릿 설정 중에 **[!UICONTROL 기본값으로 사용]** 옵션이 선택되어 있으면 일부 필드가 미리 채워져 있을 수 있습니다.

1. 템플릿에 필요한 모든 설정을 구성한 경우 템플릿을 이동할 준비가 되었다는 알림이 표시되고 화면 하단에 표준 시나리오 옵션이 나타납니다. 이제 시나리오 빌드를 계속할 수 있습니다.

   시나리오 작성에 대한 자세한 내용은 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오.

1. 시나리오를 저장하려면 **[!UICONTROL 저장]** 아이콘 ![](assets/save-icon.png)을(를) 클릭하십시오. 시나리오는 Workfront Fusion의 시나리오 영역에 저장됩니다.
