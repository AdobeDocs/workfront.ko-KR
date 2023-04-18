---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 에서 새 템플릿 만들기 [!DNL Adobe Workfront Fusion]
description: 에서 새 시나리오 템플릿을 만들 수 있습니다 [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: 612de6a98965552da6d534d9d2536237a96f7715
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# 에서 새 템플릿 만들기 [!DNL Adobe Workfront Fusion]

에서 새 시나리오 템플릿을 만들 수 있습니다 [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>새 템플릿을 만들기 전에 [!UICONTROL 공용 템플릿] 만들려는 템플릿을 아직 사용할 수 없도록 탭을 참조하십시오.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이센스**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 새 템플릿 만들기

시나리오 작성과 유사한 프로세스에서 템플릿을 작성할 수 있습니다. Fusion 관리자는 기존 시나리오에서 템플릿을 생성할 수도 있습니다.

* [템플릿 작성](#build-a-template)
* [시나리오에서 템플릿 만들기](#create-a-template-from-a-scenario)

### 템플릿 작성

1. 클릭 **[!UICONTROL 템플릿]** ![](assets/fusion-template-icon.png) 왼쪽 탐색 패널
1. 클릭 **[!UICONTROL 새 템플릿 만들기]** 오른쪽 상단 모서리에서
1. (선택 사항) 기본값을 대체하여 템플릿 이름을 변경합니다 **[!UICONTROL 새 템플릿 이름]** 왼쪽 위 모서리에서
1. (선택 사항) 템플릿의 언어를 변경하려면 **[!UICONTROL 템플릿 설정]** ![](assets/fusion-scenario-settings-icon.png) 언어 드롭다운에서 언어를 선택합니다.

   >[!IMPORTANT]
   >
   >언어 선택 항목은 시스템 설정에서 사용할 수 있는 언어에 해당하며 공개 템플릿의 이름과 해당 설명만 다룹니다. 템플릿을 저장한 후에는 템플릿 언어를 변경할 수 없습니다.

1. (선택 사항) 템플릿에 대한 설명을 입력하려면 **[!UICONTROL 템플릿 설정]** ![](assets/fusion-scenario-settings-icon.png) 설명을 입력합니다.
1. 표준 시나리오를 만들 때와 동일한 방식으로 앱, 모듈 및 도구를 추가합니다.

   모듈에 상황별 도움말을 추가하려면 다음을 참조하십시오 [설정 [!UICONTROL 마법사] 기능](#set-up-wizard-functionality) 참조하십시오.

   시나리오 빌드에 대한 자세한 내용은 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >템플릿에 연결, 자격 증명 또는 기타 개인 정보 구분 정보를 추가해야 하는 모듈이 포함되어 있으면 이 정보가 템플릿 사용자와 공유되지 않습니다.

1. (선택 사항) **[!UICONTROL 한 번 실행]** 템플릿을 테스트하려면 다음을 수행하십시오.
1. 을(를) 클릭합니다. **[!UICONTROL 저장]** 아이콘 ![](assets/save-icon.png).

>[!NOTE]
>
>템플릿을 저장하면 모든 팀 구성원이 템플릿을 볼 수 있습니다. 팀 외부에서 템플릿에 액세스할 수 있게 하려면 해당 템플릿을 게시한 다음 공유 링크를 사용하거나 관리자에게 템플릿을 승인하고 게시하도록 요청해야 합니다.

### 시나리오에서 템플릿 만들기

>[!NOTE]
>
>시나리오에서 템플릿을 만들려면 Fusion 관리자여야 합니다.

1. 시나리오를 만들 시나리오에 대한 시나리오 세부 정보 페이지를 엽니다.
1. 을(를) 클릭합니다. **관리** 페이지의 오른쪽 위 모서리 근처에 있는 드롭다운.
1. 선택 **템플릿으로 복제**.

   시나리오가 새 템플릿 페이지에 복사됩니다.
1. (선택 사항) 기본값을 대체하여 템플릿 이름을 변경합니다 **[!UICONTROL 새 템플릿 이름]** 왼쪽 위 모서리에서
1. (선택 사항) 템플릿의 언어를 변경하려면 **[!UICONTROL 템플릿 설정]** ![](assets/fusion-scenario-settings-icon.png) 언어 드롭다운에서 언어를 선택합니다.

   >[!IMPORTANT]
   >
   >언어 선택 항목은 시스템 설정에서 사용할 수 있는 언어에 해당하며 공개 템플릿의 이름과 해당 설명만 다룹니다. 템플릿을 저장한 후에는 템플릿 언어를 변경할 수 없습니다.

1. (선택 사항) 템플릿에 대한 설명을 입력하려면 **[!UICONTROL 템플릿 설정]** ![](assets/fusion-scenario-settings-icon.png) 설명을 입력합니다.
1. 표준 시나리오를 편집할 때와 동일한 방법으로 앱, 모듈 및 도구를 편집합니다.

   모듈에 상황별 도움말을 추가하려면 다음을 참조하십시오 [설정 [!UICONTROL 마법사] 기능](#set-up-wizard-functionality) 참조하십시오.

   >[!NOTE]
   >
   >템플릿에 연결, 자격 증명 또는 기타 개인 정보 구분 정보를 추가해야 하는 모듈이 포함되어 있으면 이 정보가 템플릿 사용자와 공유되지 않습니다.

1. (선택 사항) **[!UICONTROL 한 번 실행]** 템플릿을 테스트하려면 다음을 수행하십시오.
1. 을(를) 클릭합니다. **[!UICONTROL 저장]** 아이콘 ![](assets/save-icon.png).

## 설정 [!UICONTROL 마법사] 기능 {#set-up-wizard-functionality}

다음 [!DNL Workfront Fusion template] [!UICONTROL 마법사] 을 사용하면 향후 템플릿 사용자에게 모듈에서 사용되는 특정 필드와 관련된 지침이나 정보를 제공할 수 있습니다.

1. 템플릿에 추가된 모듈을 클릭하여 모듈의 필드를 확인합니다.
1. 추가할 필드를 찾습니다 [!UICONTROL 마법사] 정보 및 활성화 **[!UICONTROL 마법사에서 사용]** 해당 필드에 대해 입력합니다.
1. 사용자가 볼 수 있도록 할 정보를 [!UICONTROL 도움말] 필드.
1. (선택 사항) 템플릿을 사용할 때 사용자가 이 텍스트를 볼 수 있도록 하려면 다음을 활성화합니다 **[!UICONTROL 을 기본값으로 사용합니다]**.
1. 정보를 제공할 각 필드에 대해 2-4단계를 반복합니다.
1. 클릭 **[!UICONTROL 확인]** 변경 사항을 저장하고 모듈을 닫으려면 를 클릭합니다.
