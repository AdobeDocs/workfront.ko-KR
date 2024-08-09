---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 위험 유형 편집 및 만들기
description: 계획 단계에서 프로젝트에 위험을 추가하여 작업의 승인 전에 잠재적인 장애물을 식별할 수 있습니다. 위험은 프로젝트를 제때 또는 예산 내에서 완성하지 못하게 할 수 있는 가능한 사건이다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 2%

---

# 위험 유형 편집 및 만들기

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

계획 단계에서 프로젝트에 위험을 추가하여 작업의 승인 전에 잠재적인 장애물을 식별할 수 있습니다. 위험은 프로젝트를 제때 또는 예산 내에서 완성하지 못하게 할 수 있는 가능한 사건이다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 위험 유형

위험 유형은 보고 목적으로 위험을 분류하는 데 사용할 수 있는 레이블입니다. [!DNL Adobe Workfront] 관리자가 **[!UICONTROL 설정]** 영역에서 만듭니다. 위험 유형이 **[!UICONTROL 설정]** 영역에 설정되면 시스템에 범용적입니다. 모든 프로젝트 소유자는 프로젝트에 동일한 위험 유형을 사용할 수 있습니다.

## 위험 유형 편집 및 만들기

기본적으로 일부 위험 유형이 [!DNL Workfront]에 이미 있습니다. 조직의 요구 사항을 반영하기 위해 기존 위험 유형을 편집하거나 새 위험 유형을 만들 수 있습니다.

* [기존 위험 유형 편집](#edit-existing-risk-types)
* [새 위험 유형 만들기](#create-new-risk-types)

### 기존 위험 유형 편집 {#edit-existing-risk-types}

{{step-1-to-setup}}

1. **[!UICONTROL 위험 유형]**&#x200B;을 클릭하세요.
1. 편집할 위험 유형을 선택합니다.
1. **[!UICONTROL 편집]**&#x200B;을 클릭합니다.
1. (선택사항) 위험 유형의 이름과 설명을 변경합니다.

   **[!UICONTROL 이름]** 및 **[!UICONTROL 설명]** 필드에는 50자로 제한되어 있습니다.

1. **[!UICONTROL 변경 내용 저장].** 클릭

### 새 위험 유형 만들기 {#create-new-risk-types}

기본 위험 유형 외에 새로운 위험 유형을 만들어 조직의 요구 사항을 반영할 수 있습니다.

신규 위험 유형을 생성하려면

{{step-1-to-setup}}

1. **[!UICONTROL 위험 유형]**&#x200B;을 클릭하세요.
1. **[!UICONTROL 새 위험 유형]**&#x200B;을 클릭합니다.
1. 위험 유형에 **[!UICONTROL 이름]**(필수)과 **[!UICONTROL 설명]**(선택 사항)을 입력하십시오.

   **[!UICONTROL 이름]** 및 **[!UICONTROL 설명]** 필드에는 50자로 제한되어 있습니다.

1. **[!UICONTROL 위험 유형 만들기]**&#x200B;를 클릭합니다. 인라인 편집을 사용하여 위험 유형을 추가한 경우 완료되면 **[!UICONTROL Enter]**&#x200B;를 클릭하세요.

   >[!NOTE]
   >
   >사용자 지정 위험 유형을 편집해야 하는 경우 이 문서의 [[!UICONTROL 기존 위험 유형 편집]](#edit-existing-risk-types) 섹션을 참조하십시오.

## 프로젝트에 위험 유형과 함께 위험 첨부

위험 유형은 프로젝트에 추가된 위험에 레이블을 지정하는 데 사용할 수 있습니다. 프로젝트에 위험을 추가하는 방법에 대한 자세한 내용은 [프로젝트에 대한 위험 만들기 및 편집](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)을 참조하세요.
