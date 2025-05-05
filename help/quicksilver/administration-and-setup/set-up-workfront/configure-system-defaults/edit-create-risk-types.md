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
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 2%

---

# 위험 유형 편집 및 만들기

<!--Audited: 03/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

Adobe Workfront에는 작업의 승인 전에 잠재적인 장애 요소를 식별하기 위해 계획 단계에서 프로젝트와 연결할 수 있는 여러 가지 기본 위험 유형이 있습니다.

위험은 프로젝트를 제때 또는 예산 내에서 완성하지 못하게 할 수 있는 가능한 사건이다.

기본 위험 유형 외에도 조직의 요구 사항을 반영하기 위해 새 위험 유형을 추가할 수 있습니다.

프로젝트에 발생할 수 있는 위험 종류를 식별하기 위해 위험 유형을 프로젝트 위험과 연결할 수 있습니다.

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
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
   또는
   <p>현재: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>
  </tr> 
 </tbody> 
</table>

*이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 위험 유형

위험 유형은 보고 목적으로 위험을 분류하는 데 사용할 수 있는 레이블입니다.

[!DNL Workfront] 관리자는 [!UICONTROL **설정**] 영역에서 [!UICONTROL 위험 유형]을 만들 수 있습니다.

위험 유형을 설정한 후에는 시스템에 범용적입니다.

모든 프로젝트 소유자는 프로젝트에 동일한 위험 유형을 사용할 수 있습니다.

## 위험 유형 편집 및 만들기

기본적으로 일부 위험 유형이 [!DNL Workfront]에 이미 있습니다.


Workfront 인스턴스의 위험 유형 수를 개선하기 위해 다음을 수행할 수 있습니다.

* [기존 위험 유형 편집](#edit-existing-risk-types)
* [위험 유형 만들기](#create-risk-types)

### 기존 위험 유형 편집 {#edit-existing-risk-types}

{{step-1-to-setup}}

1. **[!UICONTROL 위험 유형]**&#x200B;을 클릭하세요.
1. 편집할 위험 유형을 선택합니다.
1. **[!UICONTROL 편집]** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

   <span class="preview">위험 유형 [!UICONTROL **편집**] 상자가 열립니다.</span>

   ![위험 유형 편집 상자](assets/edit-risk-type-box.png)

   >[!TIP]
   >
   >   위험 유형 목록에서 위험 유형의 이름 또는 설명을 두 번 누르면 위험 유형 정보를 인라인으로 편집할 수 있습니다.

1. (선택사항) 위험 유형의 이름과 설명을 변경합니다.

   **[!UICONTROL 이름]** 및 **[!UICONTROL 설명]** 필드에는 50자로 제한되어 있습니다.

1. **[!UICONTROL 변경 내용 저장].** 클릭

1. (선택 사항) 위험 유형을 삭제하려면 목록에서 위험 유형을 선택한 다음 [!UICONTROL **삭제**] 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭하고 [!UICONTROL **예, 삭제**]&#x200B;를 클릭합니다. 위험 유형이 삭제되며 복구할 수 없습니다.

1. (선택 사항) 위험 유형 목록을 내보내려면 [!UICONTROL **내보내기**] 아이콘 ![내보내기 아이콘](assets/export-icon.png)을 클릭합니다. 다음 파일 유형으로 내보낼 수 있습니다.

   * PDF
   * Excel
   * Excel(xlsx)
   * 탭으로 구분됨

   >[!TIP]
   >
   >   먼저 제한된 수의 위험 유형을 선택한 다음 더 작은 목록으로 내보낼 수 있습니다.


### 위험 유형 만들기 {#create-risk-types}

기본 위험 유형 외에 위험 유형을 생성할 수 있습니다.

{{step-1-to-setup}}

1. **[!UICONTROL 위험 유형]**&#x200B;을 클릭하세요.

1. **[!UICONTROL 새 위험 유형]**&#x200B;을 클릭하여 [!UICONTROL **새 위험 유형**] 상자를 엽니다.

   또는

   위험 유형 목록의 왼쪽 아래에서 [!UICONTROL **위험 유형 추가**]&#x200B;를 클릭하여 위험 유형을 인라인으로 추가합니다.

   <span class="preview">새 위험 유형 **2&rbrace; 상자가 열립니다. <span>**

   ![새 위험 유형 상자](assets/new-risk-type-box.png)


1. 위험 유형에 **[!UICONTROL 이름]**(필수)과 **[!UICONTROL 설명]**(선택 사항)을 추가하십시오.

   **[!UICONTROL 이름]** 및 **[!UICONTROL 설명]** 필드에는 50자로 제한되어 있습니다.

1. **[!UICONTROL 위험 유형 만들기]**&#x200B;를 클릭합니다.

   또는 인라인 편집을 사용하여 위험 유형을 추가한 경우 완료되면 **[!UICONTROL Enter]**&#x200B;를 클릭하세요.

   >[!TIP]
   >
   >사용자 지정 위험 유형을 편집하려면 이 문서의 [[!UICONTROL 기존 위험 유형 편집]섹션](#edit-existing-risk-types)을 참조하세요.

## 프로젝트에 위험 유형과 함께 위험 첨부

위험 유형을 사용하여 프로젝트에 추가된 위험에 레이블을 지정할 수 있습니다.

프로젝트에 위험을 추가하는 방법에 대한 자세한 내용은 [프로젝트에 대한 위험 만들기 및 편집](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)을 참조하세요.
