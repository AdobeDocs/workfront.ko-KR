---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion]에서 새 템플릿 만들기'
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 새 템플릿 만들기

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [새 템플릿 만들기](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-and-manage-templates/create-new-fusion-templates.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe] Workfront Fusion에서 새 시나리오 템플릿을 만들 수 있습니다.

>[!TIP]
>
>새 템플릿을 만들기 전에 [!UICONTROL 공개 템플릿] 탭에서 만들 템플릿을 아직 사용할 수 있는지 확인할 수 있습니다.

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
   </td>    </tr> 
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

## 새 템플릿 만들기

시나리오 작성과 유사한 프로세스에서 템플릿을 작성할 수 있습니다. Fusion 관리자는 기존 시나리오에서 템플릿을 만들 수도 있습니다.

* [템플릿 작성](#build-a-template)
* [시나리오에서 템플릿 만들기](#create-a-template-from-a-scenario)

### 템플릿 작성

1. 왼쪽 탐색 패널에서 **[!UICONTROL 템플릿]** ![](assets/fusion-template-icon.png)을(를) 클릭합니다.
1. 오른쪽 상단의 **[!UICONTROL 새 템플릿 만들기]**&#x200B;를 클릭합니다.
1. (선택 사항) 왼쪽 위 모서리에서 기본 **[!UICONTROL 새 템플릿 이름]**&#x200B;을(를) 바꾸어 템플릿 이름을 변경합니다.
1. (선택 사항) 템플릿의 언어를 변경하려면 **[!UICONTROL 템플릿 설정]** ![](assets/fusion-scenario-settings-icon.png)을 클릭하고 언어 드롭다운에서 언어를 선택합니다.

   >[!IMPORTANT]
   >
   >언어 선택은 시스템 설정에서 사용할 수 있는 언어에 해당하며 공개 템플릿의 이름과 설명만 고려합니다. 템플릿이 저장되면 템플릿 언어를 변경할 수 없습니다.

1. (선택 사항) 템플릿에 대한 설명을 입력하려면 **[!UICONTROL 템플릿 설정]** ![](assets/fusion-scenario-settings-icon.png)을 클릭하고 설명을 입력하십시오.
1. 표준 시나리오를 만들 때와 동일한 방식으로 앱, 모듈 및 도구를 추가합니다.

   모듈에 상황별 도움말을 추가하려면 이 문서에서 [[!UICONTROL 마법사] 기능 설정](#set-up-wizard-functionality)을 참조하십시오.

   시나리오 작성에 대한 자세한 내용은 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오.

   >[!NOTE]
   >
   >템플릿에 연결, 자격 증명 또는 기타 개인 정보에 민감한 정보를 추가해야 하는 모듈이 포함된 경우 이 정보는 템플릿 사용자와 공유되지 않습니다.

1. (선택 사항) 템플릿을 테스트하려면 **[!UICONTROL 한 번 실행]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 저장]** 아이콘 ![](assets/save-icon.png)을 클릭합니다.

>[!NOTE]
>
>템플릿을 저장하면 모든 팀원이 볼 수 있습니다. 팀 외부에서 템플릿에 액세스할 수 있게 하려면 요청을 제출하여 템플릿을 승인 및 게시해야 합니다. 요청이 승인을 위해 Adobe Workfront으로 이동하고 승인되면 팀 외부의 다른 사용자가 템플릿에 액세스할 수 있습니다.
>
>템플릿 게시에 대한 자세한 내용은 [Publish 및 공유 [!DNL Adobe Workfront Fusion] 템플릿](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md)을 참조하세요.

### 시나리오에서 템플릿 만들기

>[!NOTE]
>
>시나리오에서 템플릿을 만들려면 Fusion 관리자여야 합니다.

1. 시나리오를 생성하려는 시나리오에 대한 시나리오 세부 정보 페이지를 엽니다.
1. 페이지의 오른쪽 상단 근처에 있는 **관리자** 드롭다운을 클릭합니다.
1. **템플릿으로 복제**&#x200B;를 선택합니다.

   시나리오가 새 템플릿 페이지에 복사됩니다.
1. (선택 사항) 왼쪽 위 모서리에서 기본 **[!UICONTROL 새 템플릿 이름]**&#x200B;을(를) 바꾸어 템플릿 이름을 변경합니다.
1. (선택 사항) 템플릿의 언어를 변경하려면 **[!UICONTROL 템플릿 설정]** ![](assets/fusion-scenario-settings-icon.png)을 클릭하고 언어 드롭다운에서 언어를 선택합니다.

   >[!IMPORTANT]
   >
   >언어 선택은 시스템 설정에서 사용할 수 있는 언어에 해당하며 공개 템플릿의 이름과 설명만 고려합니다. 템플릿이 저장되면 템플릿 언어를 변경할 수 없습니다.

1. (선택 사항) 템플릿에 대한 설명을 입력하려면 **[!UICONTROL 템플릿 설정]** ![](assets/fusion-scenario-settings-icon.png)을 클릭하고 설명을 입력하십시오.
1. 표준 시나리오를 편집할 때와 동일한 방법으로 앱, 모듈 및 도구를 편집합니다.

   모듈에 상황별 도움말을 추가하려면 이 문서에서 [[!UICONTROL 마법사] 기능 설정](#set-up-wizard-functionality)을 참조하십시오.

   >[!NOTE]
   >
   >템플릿에 연결, 자격 증명 또는 기타 개인 정보에 민감한 정보를 추가해야 하는 모듈이 포함된 경우 이 정보는 템플릿 사용자와 공유되지 않습니다.

1. (선택 사항) 템플릿을 테스트하려면 **[!UICONTROL 한 번 실행]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 저장]** 아이콘 ![](assets/save-icon.png)을 클릭합니다.

## [!UICONTROL 마법사] 기능 설정 {#set-up-wizard-functionality}

[!DNL Workfront Fusion template] [!UICONTROL 마법사]를 사용하면 향후 템플릿 사용자에게 모듈에서 사용되는 특정 필드와 관련된 지침이나 정보를 제공할 수 있습니다.

1. 템플릿에 추가된 모듈을 클릭하여 모듈의 필드를 확인합니다.
1. [!UICONTROL 마법사] 정보를 추가할 필드를 찾은 다음 해당 필드에 대해 **[!UICONTROL 마법사에서 사용]**&#x200B;을 사용하도록 설정하십시오.
1. [!UICONTROL 도움말] 필드에 사용자에게 표시할 정보를 입력하십시오.
1. (선택 사항) 템플릿을 사용할 때 사용자가 이 텍스트를 볼 수 있도록 하려면 **[!UICONTROL 기본값으로 사용]**&#x200B;을 사용하도록 설정하십시오.
1. 정보를 제공하려는 각 필드에 대해 2~4단계를 반복합니다.
1. 변경 내용을 저장하고 모듈을 닫으려면 **[!UICONTROL 확인]**&#x200B;을 클릭하십시오.
