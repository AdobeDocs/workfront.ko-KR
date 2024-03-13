---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 통합에서 워크플로우 사용
description: Experience Manager Assets Essentials 통합에서 워크플로우 사용
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 821e31b8c6023a9ec4e017cc5548bb9fd930983c
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# Experience Manager Assets 통합에서 워크플로우 사용

워크플로는 Workfront을 Adobe Experience Manager as a Cloud Service에 연결하는 작업 세트입니다. Workfront 관리자는 Workfront에서 워크플로우를 구성한 다음 프로젝트 템플릿에 할당할 수 있습니다. 워크플로가 할당된 프로젝트 템플릿을 사용하여 프로젝트를 만들면 워크플로에 정의된 작업이 트리거됩니다.

>[!NOTE]
>
>워크플로우는 Adobe Experience Manager as a Cloud Service 통합에서만 사용할 수 있습니다. Adobe Experience Manager Assets Essentials과의 통합에서는 사용할 수 없습니다.


## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>Adobe Workfront 플랜*</strong>
   </td>
   <td>임의
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront 라이센스*</strong>
   </td>
   <td>요청 이상
   </td>
  </tr>
  <tr>
   <td><strong>제품</strong>
   </td>
   <td><p>Experience Manager Assets as a Cloud Service 또는 Assets Essentials이 있어야 하며, Admin Console에서 사용자로 제품에 추가되어야 합니다.</p><p>Adobe Experience Manager의 저장소에 대한 쓰기 액세스 권한이 있어야 합니다.</p>
   </td>
  </tr>
  <tr>
   <td><strong>액세스 수준 구성*</strong>
   </td>
   <td>문서에 대한 액세스 편집
<p>
<strong>참고: </strong>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <strong>사용자 정의 액세스 수준 만들기 또는 수정</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>개체 권한</strong>
   </td>
   <td>프로젝트에서 액세스 권한 이상 관리 
<p>
추가 액세스 요청에 대한 자세한 내용은 <strong>오브젝트에 대한 액세스 요청 </strong>.
   </td>
  </tr>
</table>

## 전제 조건

시작하기 전에,

* Workfront 관리자는 Adobe Experience Manager 통합에서 워크플로우를 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## 템플릿에 워크플로 추가

프로젝트 템플릿에 워크플로우를 추가할 수 있습니다. 워크플로우는 템플릿에서 만든 모든 프로젝트에 적용됩니다.

1. 을 클릭하여 템플릿을 엽니다. **템플릿** 메인 메뉴에서 템플릿을 선택합니다.
1. 클릭 **Experience Manager Assets** 을 클릭합니다.

   >[!NOTE]
   >
   >Experience Manager Assets 섹션이 왼쪽 탐색에 표시되지 않으면 Workfront 관리자가 조직에 대한 워크플로우를 활성화하지 않은 것입니다. <!--Is this right?-->

1. 다음에서 **자동화된 워크플로에 대한 통합 선택 필드**&#x200B;을(를) 통해 이 템플릿에서 만든 프로젝트에 사용할 워크플로우와의 통합을 선택합니다.
1. (선택 사항) 이 템플릿에서 만든 프로젝트에 적용할 모든 워크플로 값을 편집합니다.

   특정 워크플로우에 대한 지침은 [프로젝트에서 워크플로 값 편집](#edit-workflow-values-in-a-project) 이 문서에서.

   설정의 Experience Manager 영역에서 활성화된 워크플로우만 템플릿 또는 프로젝트에서 사용할 수 있습니다.

1. 변경 사항이 자동으로 저장됩니다. <!-- do they though??-->

## 프로젝트에 워크플로우 추가

프로젝트를 만들 때 워크플로를 추가하거나 기존 프로젝트에 워크플로를 추가할 수 있습니다. 두 경우 모두 프로젝트 템플릿을 사용하여 워크플로우를 추가합니다.

### 프로젝트를 만들 때 워크플로우 추가

1. 프로젝트 만들기를 시작합니다.

   자세한 내용은 [템플릿을 사용하여 프로젝트 만들기](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. 프로젝트의 템플릿을 선택할 때 이 프로젝트에 사용할 워크플로가 포함된 템플릿을 선택합니다.
1. (선택 사항)에 설명된 대로 프로젝트에 대한 워크플로 값을 편집합니다 [프로젝트에서 워크플로 값 편집](#edit-workflow-values-in-a-project).

   설정의 Experience Manager 영역에서 활성화된 워크플로우만 템플릿 또는 프로젝트에서 사용할 수 있습니다.


### 기존 프로젝트에 워크플로우 추가

>[!NOTE]
>
>프로젝트를 만들 때(예: 연결된 폴더 만들기) 실행되는 워크플로우는 템플릿이 기존 프로젝트에 연결되어 있을 때 실행되지 않습니다. 템플릿에서 프로젝트를 만들 때만 실행됩니다.

1. 프로젝트에 템플릿 추가를 시작합니다.

   자세한 내용은 [프로젝트에 템플릿 첨부](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. 프로젝트의 템플릿을 선택할 때 이 프로젝트에 사용할 워크플로가 포함된 템플릿을 선택합니다.
1. (선택 사항)에 설명된 대로 프로젝트에 대한 워크플로 값을 편집합니다 [프로젝트에서 워크플로 값 편집](#edit-workflow-values-in-a-project).

   설정의 Experience Manager 영역에서 활성화된 워크플로우만 템플릿 또는 프로젝트에서 사용할 수 있습니다.



### 프로젝트에서 워크플로 값 편집

프로젝트 수준에서 워크플로 값을 편집할 수 있습니다. 프로젝트 수준 워크플로 값은 프로젝트 템플릿에 설정된 값을 재정의하며, 이는 Adobe Experience Manager Assets 통합에 설정된 기본값을 재정의합니다.

모든 워크플로우 값은 다음에서 찾을 수 있습니다.

* 프로젝트 만들기 또는 프로젝트 편집 창의 워크플로 또는 연결된 폴더 섹션.
* 왼쪽 탐색의 Adobe Experience Manager 섹션.


  >[!NOTE]
  >
  >이러한 영역이 표시되지 않으면 Workfront 관리자가 조직에 대한 워크플로를 활성화하지 않은 것입니다.



#### 연결된 폴더

>[!NOTE]
>
>연결된 폴더는 프로젝트를 만들 때 만들어지므로 기존 프로젝트에서 연결된 폴더 워크플로를 편집하면 효과가 없습니다. 프로젝트를 만들 때 이러한 값을 편집하면 예상대로 작동합니다.

링크된 폴더의 워크플로를 편집하려면:


1. 전환 **[!UICONTROL 연결된 폴더 만들기]** 원하는 대로 켜거나 끕니다. 이 기능을 켜면 연결된 폴더 구성을 편집할 수 있습니다.

   연결된 폴더 구성에 대한 자세한 내용은 [Adobe Experience Manager 연결 폴더 만들기](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) 이 문서에서 [구성 [!UICONTROL Experience Manager Assets as a Cloud Service] 통합](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (선택 사항) 프로젝트에 첨부된 사용자 정의 양식에 특정 값이 있는 경우에만 폴더 트리를 작성하려면 **필터 적용** 해당 폴더 트리에 대해 필드, 필드 및 필드 값을 포함하는 사용자 정의 양식을 선택합니다. 새 프로젝트에 첨부된 사용자 정의 양식의 필드에 선택한 값이 포함되어 있으면 폴더 트리가 만들어집니다.
1. (선택 사항) 폴더 이름을 구성할 때 다음 옵션 중에서 선택할 수 있습니다.

   * **이름**: 폴더 이름을 입력합니다.

   * **개체 데이터**: 폴더 이름의 소스(예: 프로젝트 이름)를 선택합니다.

   * **사용자 정의 양식 데이터**: 폴더 이름으로 사용할 사용자 정의 양식 데이터를 선택합니다.

     폴더 이름에 사용자 정의 양식 데이터를 사용하는 것은 템플릿 수준에서만 사용할 수 있으며 통합 수준에서는 구성할 수 없습니다.

     폴더 이름이 프로젝트에 첨부된 의 사용자 정의에 존재하지 않는 사용자 정의 데이터로 설정된 경우, 임의의 ID가 폴더 이름으로 할당됩니다.

1. 폴더 트리를 보려면 **미리 보기** ![미리 보기 아이콘](assets/preview-icon.png) 아이콘
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

#### 자산 게시

자산 게시를 위한 워크플로우를 편집하려면:

1. 전환 **에셋 자동 게시** 원하는 대로 켜거나 끕니다.
1. (조건부) 게시를 활성화하는 경우 게시 서비스에 게시할지, Brand Portal에 게시할지 또는 둘 다에 게시할지 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
