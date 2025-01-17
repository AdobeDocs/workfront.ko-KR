---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion 템플릿 관리
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 8163f9f12bb27bbc8adfde34fc1e1f0f8c8be7f9
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 템플릿 관리

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [공개 탭에 대한 템플릿 승인 또는 승인 취소](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/approve-templates.html)
>* [템플릿 편집](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/edit-templates.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

관리자는 다른 사용자가 만든 템플릿을 보고, 수정하고, 이름을 바꾸고, 게시하고, 승인하고, 삭제할 수 있는 권한이 있습니다. [!DNL Adobe Workfront Fusion Administration] 영역의 [!UICONTROL 템플릿] 페이지에서 이러한 작업을 수행할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>조직의 Workfront Fusion 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## [!DNL Workfront Fusion] 관리자로 [!DNL Workfront Fusion] 템플릿 보기

생성된 모든 템플릿과 해당 상태의 테이블을 보려면 다음과 같이 하십시오.

1. 왼쪽 탐색 패널에서 **[!UICONTROL 관리]**&#x200B;를 클릭하여 [!UICONTROL 관리] 영역을 엽니다.

   >[!NOTE]
   >
   >관리 영역은 Workfront Fusion 관리자만 볼 수 있습니다.

1. 왼쪽 탐색 패널에서 **[!UICONTROL 템플릿]**&#x200B;을 클릭합니다.

템플릿 게시 상태와 관련된 세 가지 열이 있습니다. 열의 확인 표시는 다음을 나타냅니다.

* **[!UICONTROL 게시됨]**: 이러한 템플릿은 현재 사용자 인터페이스의 [!UICONTROL 팀 템플릿] 탭에 표시됩니다.
* **[!UICONTROL 승인 요청됨]**: 이 템플릿은 사용자의 승인을 기다리고 있습니다. 현재 사용자 인터페이스의 [!UICONTROL 팀 템플릿] 탭에 표시됩니다.
* **[!UICONTROL 승인됨]**: 이 템플릿은 승인되었습니다. 현재 표준 사용자 인터페이스의 [!UICONTROL 공개 템플릿] 탭에 표시됩니다.

>[!NOTE]
>
>[!UICONTROL 요청된 승인] 열과 [!UICONTROL 승인됨] 열 모두에 확인 표시가 있는 템플릿이 이미 승인되어 공개되었지만, 새 버전이 승인을 기다리고 있습니다.

## 관리자로 [!DNL Workfront Fusion] 템플릿 편집

1. 왼쪽 탐색 패널에서 **[!UICONTROL 관리]**&#x200B;를 클릭하여 [!UICONTROL 관리] 영역을 엽니다.
1. 왼쪽 탐색 패널에서 **[!UICONTROL 템플릿]**&#x200B;을 클릭합니다.
1. 편집할 템플릿의 오른쪽에 있는 **[!UICONTROL 세부 정보]**&#x200B;를 클릭합니다.

이제 관리자가 아닌 사용자로 템플릿을 편집하는 것과 유사하게 템플릿을 편집할 수 있습니다. 그러나 오른쪽 상단의 [!UICONTROL 옵션]에는 SVG 코드를 제공하는 SVG 다이어그램이라는 한 가지 추가 옵션이 있습니다. 또한 게시 프로세스는 표준 사용자의 경우와 동일합니다. 자세한 내용은 템플릿 게시 및 공유 섹션을 참조하십시오.

편집할 수 있는 특정 템플릿 옵션에 대한 자세한 내용은 [새 템플릿 만들기 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)를 참조하십시오.

템플릿 게시에 대한 자세한 내용은 [Publish 및 공유 [!DNL Adobe Workfront Fusion] 템플릿](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md)을 참조하세요.

## [!DNL Workfront Fusion] 템플릿 승인 또는 승인 취소

템플릿을 승인하면 [!UICONTROL 공개 템플릿] 탭에 표시되고 모든 사용자가 사용할 수 있습니다. 템플릿을 승인하지 않으면 [!UICONTROL 공개 템플릿] 탭에서 템플릿이 제거되고 템플릿을 만든 팀만 사용할 수 있게 됩니다.

1. 왼쪽 탐색 패널에서 **[!UICONTROL 관리]**&#x200B;를 클릭하여 [!UICONTROL 관리] 영역을 엽니다.
1. 왼쪽 탐색 패널에서 **[!UICONTROL 템플릿]**&#x200B;을 클릭합니다.
1. 템플릿을 승인하려면 템플릿 오른쪽에 있는 **[!UICONTROL 승인]**&#x200B;을 클릭합니다.
1. 템플릿을 승인하지 않으려면 템플릿 오른쪽에 있는 **[!UICONTROL 비승인]**&#x200B;을 클릭합니다.

>[!NOTE]
>
>이전에 승인된 후 편집한 템플릿을 승인하는 경우 두 번째 승인이 원래 템플릿을 덮어씁니다.

## 시나리오를 템플릿으로 복제

관리자는 시나리오를 템플릿으로 복제할 수 있습니다.

시나리오를 템플릿으로 복제하는 방법에 대한 지침은 [새 템플릿 만들기 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)의 [시나리오에서 템플릿 만들기](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario)를 참조하십시오.
