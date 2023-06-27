---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion 템플릿 관리
description: 관리자는 다른 사용자가 만든 템플릿을 보고, 수정하고, 이름을 바꾸고, 게시하고, 승인하고, 삭제할 수 있는 권한이 있습니다. 다음 작업은에서 수행할 수 있습니다. [!UICONTROL 템플릿] 페이지의 [!DNL Adobe Workfront Fusion Administration] 영역입니다.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 템플릿 관리

관리자는 다른 사용자가 만든 템플릿을 보고, 수정하고, 이름을 바꾸고, 게시하고, 승인하고, 삭제할 수 있는 권한이 있습니다. 다음 작업은에서 수행할 수 있습니다. [!UICONTROL 템플릿] 페이지의 [!DNL Adobe Workfront Fusion Administration] 영역입니다.

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
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>조직의 Workfront Fusion 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 보기 [!DNL Workfront Fusion] 관리자인 템플릿

생성된 모든 템플릿과 해당 상태의 테이블을 보려면 다음과 같이 하십시오.

1. 클릭 **[!UICONTROL 관리]** 을 클릭하여 왼쪽 탐색 패널에서 [!UICONTROL 관리] 영역입니다.
1. 클릭 **[!UICONTROL 템플릿]** 을 클릭합니다.

템플릿 게시 상태와 관련된 세 가지 열이 있습니다. 열의 확인 표시는 다음을 나타냅니다.

* **[!UICONTROL 게시됨]**: 이러한 템플릿은 현재 [!UICONTROL 팀 템플릿] 사용자 인터페이스의 탭입니다.
* **[!UICONTROL 승인 요청됨]**: 이 템플릿들은 사용자의 승인을 기다리고 있습니다. 현재 다음 위치에 표시됩니다. [!UICONTROL 팀 템플릿] 사용자 인터페이스의 탭입니다.
* **[!UICONTROL 승인됨]**: 이 템플릿들은 승인되었습니다. 현재 다음 위치에 표시됩니다. [!UICONTROL 공개 템플릿] 표준 사용자 인터페이스의 탭.

>[!NOTE]
>
>양쪽에 확인 표시가 있는 템플릿 [!UICONTROL 승인 요청됨] 열 및 [!UICONTROL 승인됨] 열이 이미 승인되어 공개되었지만, 최신 버전이 승인을 기다리고 있습니다.

## 편집 [!DNL Workfront Fusion] 관리자인 템플릿

1. 클릭 **[!UICONTROL 관리]** 을 클릭하여 왼쪽 탐색 패널에서 [!UICONTROL 관리] 영역입니다.
1. 클릭 **[!UICONTROL 템플릿]** 을 클릭합니다.
1. 클릭 **[!UICONTROL 세부 사항]** 편집할 템플릿의 오른쪽에 있습니다.

이제 관리자가 아닌 사용자로 템플릿을 편집하는 것과 유사하게 템플릿을 편집할 수 있습니다. 그러나 [!UICONTROL 옵션] 오른쪽 상단 모서리에는 SVG 코드를 제공하는 SVG 다이어그램과 같은 한 가지 추가 옵션이 있습니다. 또한 게시 프로세스는 표준 사용자의 경우와 동일합니다. 자세한 내용은 템플릿 게시 및 공유 섹션을 참조하십시오.

편집할 수 있는 특정 템플릿 옵션에 대한 자세한 내용은 [에서 새 템플릿 만들기 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

템플릿 게시에 대한 자세한 내용은 [게시 및 공유 [!DNL Adobe Workfront Fusion] 템플릿](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## 승인 또는 비승인 [!DNL Workfront Fusion] 템플릿

템플릿을 승인하면 다음에서 볼 수 있습니다. [!UICONTROL 공개 템플릿] 모든 사용자가 사용할 수 있습니다. 템플릿을 승인하지 않으면 템플릿에서 제거됩니다. [!UICONTROL 공개 템플릿] 을 탭하여 만든 팀에서만 사용할 수 있도록 합니다.

1. 클릭 **[!UICONTROL 관리]** 을 클릭하여 왼쪽 탐색 패널에서 [!UICONTROL 관리] 영역입니다.
1. 클릭 **[!UICONTROL 템플릿]** 을 클릭합니다.
1. 템플릿을 승인하려면 다음을 클릭하십시오. **[!UICONTROL 승인]** 템플릿의 오른쪽에 있습니다.
1. 템플릿을 승인하지 않으려면 **[!UICONTROL 비승인]** 템플릿의 오른쪽에 있습니다.

>[!NOTE]
>
>이전에 승인된 후 편집한 템플릿을 승인하는 경우 두 번째 승인이 원래 템플릿을 덮어씁니다.

## 시나리오를 템플릿으로 복제

관리자는 시나리오를 템플릿으로 복제할 수 있습니다.

시나리오를 템플릿으로 복제하는 방법에 대한 지침은 [시나리오에서 템플릿 만들기](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) 위치: [에서 새 템플릿 만들기 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
