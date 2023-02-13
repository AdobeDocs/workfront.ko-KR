---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 위험 유형 편집 및 생성
description: 계획 단계에서 프로젝트에 위험을 추가하여 작업 승인 전에 잠재적인 장애물을 식별할 수 있습니다. 위험은 프로젝트 완료를 제시간에 또는 예산 내에서 방지할 수 있는 가능한 이벤트입니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# 위험 유형 편집 및 생성

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

계획 단계에서 프로젝트에 위험을 추가하여 작업 승인 전에 잠재적인 장애물을 식별할 수 있습니다. 위험은 프로젝트 완료를 제시간에 또는 예산 내에서 방지할 수 있는 가능한 이벤트입니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 위험 유형

위험 유형은 위험을 보고용으로 분류하는 데 사용할 수 있는 레이블입니다. 이 워크플로우는 **[!UICONTROL 설정]** 영역별 [!DNL Adobe Workfront] 관리자 에서 위험 유형이 설정되면 **[!UICONTROL 설정]** 이 영역은 사용자 시스템에 일반적입니다. 모든 프로젝트 소유자는 프로젝트에 동일한 위험 유형을 사용할 수 있습니다.

## 위험 유형 편집 및 생성

일부 위험 유형이 이미 있습니다. [!DNL Workfront]기본적으로 입니다. 조직의 요구 사항을 반영하기 위해 기존 위험 유형을 편집하거나 새로운 위험 유형을 만들 수 있습니다.

* [기존 위험 유형 편집](#edit-existing-risk-types)
* [새로운 위험 유형 생성](#create-new-risk-types)

### 기존 위험 유형 편집 {#edit-existing-risk-types}

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 위험 유형]**.
1. 편집할 위험 유형을 선택합니다.
1. 클릭 **[!UICONTROL 편집]**.
1. (선택 사항) 위험 유형의 이름과 설명을 변경합니다.

   에는 50자로 제한됩니다 **[!UICONTROL 이름]** 그리고 **[!UICONTROL 설명]** 필드.

1. 클릭 **[!UICONTROL 변경 내용 저장].**

### 새로운 위험 유형 생성 {#create-new-risk-types}

조직의 요구 사항을 반영하도록 기본 위험 유형 외에도 새 위험 유형을 만들 수 있습니다.

새 위험 유형을 생성하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 위험 유형]**.
1. 클릭 **[!UICONTROL 새로운 위험 유형]**.
1. 입력 **[!UICONTROL 이름]** (필수) 및 **[!UICONTROL 설명]** (선택 사항) 을 고려합니다.

   에는 50자로 제한됩니다 **[!UICONTROL 이름]** 그리고 **[!UICONTROL 설명]** 필드.

1. 클릭 **[!UICONTROL 위험 유형 생성]**. 인라인 편집을 사용하여 위험 유형을 추가한 경우 **[!UICONTROL Enter 키]** 다 되면

   >[!NOTE]
   >
   >사용자 지정 위험 유형을 편집해야 하는 경우 섹션을 참조하십시오 [[!UICONTROL 기존 편집] 위험 유형](#edit-existing-risk-types) 참조하십시오.

## 프로젝트에 위험 유형 적용

위험 유형은 프로젝트에 추가된 위험에 레이블을 지정하는 데 사용할 수 있습니다. 프로젝트에 위험을 추가하는 방법에 대한 자세한 내용은 [프로젝트에서 위험 요소 생성 및 편집](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
