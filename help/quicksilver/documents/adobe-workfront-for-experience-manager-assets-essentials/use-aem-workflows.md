---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 통합에서 워크플로우 사용
description: Experience Manager Assets Essentials 통합에서 워크플로우 사용
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 0%

---

# Experience Manager Assets 통합에서 워크플로우 사용

워크플로는 Workfront을 Adobe Experience Manager as a Cloud Service에 연결하는 작업 세트입니다. Workfront 관리자는 Workfront에서 워크플로우를 구성한 다음 프로젝트 템플릿에 할당할 수 있습니다.

워크플로가 할당된 프로젝트 템플릿을 사용하여 프로젝트를 만들면 워크플로에 정의된 작업이 트리거됩니다.

>[!NOTE]
>
>워크플로우는 Adobe Experience Manager as a Cloud Service 통합에서만 사용할 수 있습니다. Adobe Experience Manager Assets Essentials와의 통합에서는 사용할 수 없습니다.


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p> 임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p> 
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">추가 제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials가 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager 권한</td> 
    <td>폴더에 대한 쓰기 액세스 권한이 있어야 합니다.</td> 
   </tr>
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 이상 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에,

* Workfront 관리자는 Adobe Experience Manager 통합에서 워크플로우를 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional)을 참조하십시오.

## 템플릿에 워크플로 추가

프로젝트 템플릿에 워크플로우를 추가할 수 있습니다. 워크플로우는 템플릿에서 만든 모든 프로젝트에 적용됩니다.

1. 메인 메뉴에서 **템플릿**&#x200B;을 클릭한 다음 목록에서 템플릿을 선택하여 템플릿을 엽니다.
1. 왼쪽 탐색 패널에서 **Experience Manager Assets**&#x200B;을(를) 클릭합니다.

   >[!NOTE]
   >
   >Experience Manager Assets 섹션이 왼쪽 탐색에 표시되지 않으면 Workfront 관리자가 조직에 대한 워크플로우를 활성화하지 않은 것입니다. <!--Is this right?-->

1. **자동화된 워크플로에 대한 통합 선택 필드**&#x200B;에서 이 템플릿으로 만든 프로젝트에 사용할 워크플로와의 통합을 선택합니다.
1. (선택 사항) 이 템플릿에서 만든 프로젝트에 적용할 모든 워크플로 값을 편집합니다.

   특정 워크플로에 대한 지침은 이 문서의 [프로젝트의 워크플로 값 편집](#edit-workflow-values-in-a-project)을 참조하십시오.

   설정의 Experience Manager 영역에서 활성화된 워크플로우만 템플릿 또는 프로젝트에서 사용할 수 있습니다.

1. 변경 사항이 자동으로 저장됩니다. <!-- do they though??-->

## 프로젝트에 워크플로우 추가

프로젝트를 만들 때 워크플로를 추가하거나 기존 프로젝트에 워크플로를 추가할 수 있습니다. 두 경우 모두 프로젝트 템플릿을 사용하여 워크플로우를 추가합니다.

### 프로젝트를 만들 때 워크플로우 추가

1. 프로젝트 만들기를 시작합니다.

   지침은 [템플릿을 사용하여 프로젝트 만들기](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)를 참조하십시오.

1. 프로젝트의 템플릿을 선택할 때 이 프로젝트에 사용할 워크플로가 포함된 템플릿을 선택합니다.
1. (선택 사항) [프로젝트의 워크플로 값 편집](#edit-workflow-values-in-a-project)에 설명된 대로 프로젝트의 워크플로 값을 편집합니다.

   설정의 Experience Manager 영역에서 활성화된 워크플로우만 템플릿 또는 프로젝트에서 사용할 수 있습니다.


### 기존 프로젝트에 워크플로우 추가

>[!NOTE]
>
>프로젝트를 만들 때(예: 연결된 폴더 만들기) 실행되는 워크플로우는 템플릿이 기존 프로젝트에 연결되어 있을 때 실행되지 않습니다. 템플릿에서 프로젝트를 만들 때만 실행됩니다.

1. 프로젝트에 템플릿 추가를 시작합니다.

   자세한 내용은 [프로젝트에 템플릿 첨부](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md)를 참조하십시오.

1. 프로젝트의 템플릿을 선택할 때 이 프로젝트에 사용할 워크플로가 포함된 템플릿을 선택합니다.
1. (선택 사항) [프로젝트의 워크플로 값 편집](#edit-workflow-values-in-a-project)에 설명된 대로 프로젝트의 워크플로 값을 편집합니다.

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

1. 원하는 대로 **[!UICONTROL 연결된 폴더 만들기]**&#x200B;를 켜거나 끕니다. 이 기능을 켜면 연결된 폴더 구성을 편집할 수 있습니다.

   연결된 폴더 구성에 대한 자세한 내용은 문서 [Adobe Experience Manager 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders)에서 [Experience Manager Assets 연결된 폴더 만들기[!UICONTROL 를 참조하십시오. &#x200B;]as a Cloud Service 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)

1. (선택 사항) 프로젝트에 첨부된 사용자 정의 양식에 특정 값이 있는 경우에만 폴더 트리를 작성하려면 해당 폴더 트리의 **필터 적용**&#x200B;을 클릭한 다음, 필드, 필드 값을 포함하는 사용자 정의 양식을 선택하십시오. 새 프로젝트에 첨부된 사용자 정의 양식의 필드에 선택한 값이 포함되어 있으면 폴더 트리가 만들어집니다.
1. (선택 사항) 폴더 이름을 구성할 때 다음 옵션 중에서 선택할 수 있습니다.

   * **이름**: 폴더 이름을 입력하십시오.

   * **개체 데이터**: 폴더 이름에 대한 원본(예: 프로젝트 이름)을 선택하십시오.

   * **사용자 정의 양식 데이터**: 폴더 이름으로 사용할 사용자 정의 양식 데이터를 선택합니다.

     폴더 이름에 사용자 정의 양식 데이터를 사용하는 것은 템플릿 수준에서만 사용할 수 있으며 통합 수준에서는 구성할 수 없습니다.

     폴더 이름이 프로젝트에 첨부된 의 사용자 정의에 존재하지 않는 사용자 정의 데이터로 설정된 경우, 임의의 ID가 폴더 이름으로 할당됩니다.

1. 폴더 트리를 보려면 **미리 보기** ![미리 보기 아이콘](assets/preview-icon.png) 아이콘을 클릭하세요.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

#### 자산 게시

자산 게시를 위한 워크플로우를 편집하려면:

1. 원하는 대로 **자산을 자동으로 게시**&#x200B;하거나 해제합니다.
1. (조건부) 게시를 활성화하는 경우 게시 서비스에 게시할지, Brand Portal에 게시할지 또는 둘 다에 게시할지 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
