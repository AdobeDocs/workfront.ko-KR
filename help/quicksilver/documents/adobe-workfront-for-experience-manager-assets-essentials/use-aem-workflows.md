---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 통합에서 워크플로우 사용
description: Experience Manager Assets Essentials 통합에서 워크플로우 사용
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 038f5f3c941ea69feb43492a30b5abea39f7c932
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Experience Manager Assets 통합에서 워크플로우 사용

워크플로우는 Workfront을 Adobe Experience Manager as a Cloud Service에 연결하는 작업 세트입니다. Workfront 관리자는 Workfront에서 워크플로우를 구성한 다음 프로젝트 템플릿에 할당할 수 있습니다. 워크플로우가 할당된 프로젝트 템플릿을 사용하여 프로젝트를 만들 때 워크플로우에 정의된 작업이 트리거됩니다.

>[!NOTE]
>
>워크플로우는 Adobe Experience Manager as a Cloud Service 통합에서만 사용할 수 있습니다. 이 기능은 Adobe Experience Manager Assets Essentials과의 통합에서 사용할 수 없습니다.


## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>Adobe Workfront 플랜*</strong>
   </td>
   <td>모든
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront 라이선스*</strong>
   </td>
   <td>요청 이상
   </td>
  </tr>
  <tr>
   <td><strong>제품</strong>
   </td>
   <td><p>Experience Manager Assets as a Cloud Service 또는 Assets Essentials이 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.</p><p>연결된 폴더를 만들려면 Adobe Experience Manager의 리포지토리에 대한 쓰기 액세스 권한이 있어야 합니다.</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>액세스 수준 구성*</strong>
   </td>
   <td>문서 액세스 편집
<p>
<strong>참고: </strong>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <strong>사용자 정의 액세스 수준 만들기 또는 수정</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>개체 권한</strong>
   </td>
   <td>프로젝트에서 액세스 이상 관리 
<p>
추가 액세스 요청에 대한 자세한 내용은 <strong>개체에 대한 액세스 요청 </strong>.
   </td>
  </tr>
</table>

## 전제 조건

시작하기 전에

* Workfront 관리자는 Adobe Experience Manager 통합에서 워크플로우를 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## 템플릿에 워크플로우 추가

프로젝트 템플릿에 워크플로우를 추가할 수 있습니다. 워크플로우는 템플릿에서 만든 모든 프로젝트에 적용됩니다.

1. <!-- main menu snippet??--> 을 클릭하여 템플릿을 엽니다. **템플릿** 주 메뉴에서 목록에서 템플릿을 선택합니다.
1. 클릭 **Experience Manager Assets** 왼쪽 탐색 패널

   >[!NOTE]
   >
   >Experience Manager Assets 섹션이 왼쪽 탐색에 표시되지 않으면 Workfront 관리자가 조직에 대해 워크플로우를 활성화하지 않은 것입니다. <!--Is this right?-->

1. 에서 **자동화된 워크플로우에 대한 통합 필드를 선택합니다**&#x200B;을(를) 선택하고 이 템플릿에서 만든 프로젝트에 사용할 워크플로우와의 통합을 선택합니다.
1. (선택 사항) 이 템플릿에서 만든 프로젝트에 적용할 워크플로우 값을 편집합니다.

   예를 들어, 기본값이 아닌 다른 위치에 링크된 폴더를 만들려면 링크된 폴더 위치를 입력합니다.

   설정 의 Experience Manager 영역에서 활성화된 워크플로우만 템플릿 또는 프로젝트에서 사용할 수 있습니다.

1. 변경 사항이 자동으로 저장됩니다. <!-- do they though??-->

## 프로젝트에 워크플로우 추가

프로젝트를 만들 때 워크플로우를 추가하거나 기존 프로젝트에 워크플로우를 추가할 수 있습니다. 두 경우 모두 프로젝트 템플릿을 사용하여 워크플로우를 추가합니다.

### 프로젝트를 만들 때 워크플로우 추가

1. 프로젝트 만들기를 시작합니다.

   자세한 내용은 [템플릿을 사용하여 프로젝트 만들기](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. 프로젝트에 대한 템플릿을 선택할 때 이 프로젝트에 사용할 워크플로우가 포함된 템플릿을 선택합니다.
1. (선택 사항) 다음에 설명된 대로 프로젝트의 워크플로우 값을 편집합니다. [프로젝트에서 워크플로우 값 편집](#edit-workflow-values-in-a-project).

   설정 의 Experience Manager 영역에서 활성화된 워크플로우만 템플릿 또는 프로젝트에서 사용할 수 있습니다.


### 기존 프로젝트에 워크플로우 추가

1. 프로젝트에 템플릿 추가를 시작합니다.

   자세한 내용은 [프로젝트에 템플릿 첨부](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. 프로젝트에 대한 템플릿을 선택할 때 이 프로젝트에 사용할 워크플로우가 포함된 템플릿을 선택합니다.
1. (선택 사항) 다음에 설명된 대로 프로젝트의 워크플로우 값을 편집합니다. [프로젝트에서 워크플로우 값 편집](#edit-workflow-values-in-a-project).

### 프로젝트에서 워크플로우 값 편집

프로젝트 수준에서 워크플로우 값을 편집할 수 있습니다. 프로젝트 수준 워크플로우 값은 Adobe Experience Manager Assets 통합에 설정된 기본값을 무시하는 프로젝트 템플릿에 설정된 값을 재정의합니다.

모든 워크플로우 값은

* 프로젝트 만들기 또는 프로젝트 편집 창의 워크플로우 섹션.
* 왼쪽 탐색 메뉴의 Adobe Experience Manager 섹션.


   >[!NOTE]
   >
   >이러한 영역이 표시되지 않으면 Workfront 관리자가 조직에 대해 워크플로우 를 활성화하지 않은 것입니다.

#### 연결된 폴더

링크된 폴더의 워크플로우를 편집하려면

1. 전환 **[!UICONTROL 링크된 폴더 만들기]** 설정
1. 이 통합과 관련된 모든 연결된 폴더를 표시할 폴더 경로를 선택합니다.
1. 프로젝트 생성 또는 프로젝트 편집 창을 사용하는 경우 저장 을 클릭합니다.

   또는

   Adobe Experience Manager 영역에 있는 경우 변경 사항이 자동으로 저장됩니다. <!--Do they though?-->

