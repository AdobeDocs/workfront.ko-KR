---
title: Workspace 계층 만들기
description: 작업 영역 관리자는 Adobe Workfront Planning의 레코드 유형 간에 여러 작업 영역 계층을 생성할 수 있습니다. 작업 영역에서 레코드 유형을 연결하고 계층을 만들면 레코드 유형이 서로 연결되며, 한 레코드 유형이 상위로 지정되고 최대 6개의 다른 레코드 유형이 하위로 구성됩니다.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# 작업 영역 계층 만들기

작업 영역 관리자는 Adobe Workfront Planning의 레코드 유형 간에 여러 작업 영역 계층을 생성할 수 있습니다.


레코드 유형이 작업 영역 내에서 연결되면 이러한 연결을 구성하는 계층 구조를 만들 수 있습니다. 계층은 레코드 유형을 상위-하위 관계로 구성하며 최대 4가지 수준의 객체 유형을 포함할 수 있습니다.

두 레코드 유형 간의 연결이 아직 없는 경우 계층 구조를 설정할 때 만들 수 있습니다. 계층이 정의되면 작업 공간 내에서 관련 레코드 유형 간에 구조화된 경로를 설정합니다.

계층은 헤더에 표시되는 레코드 종류 및 레코드 <!--ensure this is the case: does the breadcrumb show for both the RT and the record??-->에 대한 이동 경로를 생성합니다. 이렇게 하면 사용자는 워크플로의 모든 단계에서 계층 구조에서 자신의 위치를 알 수 있습니다.

계층 및 이동 경로에 대한 일반적인 정보는 [계층 및 이동 경로 개요](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)를 참조하십시오.

## 액세스 요구 사항

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ 을 확장하여 액세스 요구 사항을 보고 이 문서의 단계를 수행하십시오.  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul> 
<li><p>모든 Workfront 및 모든 Planning 패키지</p></li>
또는
<li><p>모든 워크플로우 및 모든 Planning 패키지</p></li></ul>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 공간에 대한 권한 관리</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 공간 계층 만들기

{#step1-to-planning}

1. 작업 영역 카드를 클릭합니다.
1. 작업 영역 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **설정**&#x200B;을 클릭합니다.
기본적으로 **계층** 섹션이 열립니다.
1. **계층** 페이지의 오른쪽 상단 모서리에서 **새 계층**&#x200B;을 클릭합니다.
1. **개체 추가**&#x200B;를 클릭하고 드롭다운 메뉴에서 개체를 선택합니다. 이 개체는 계층의 첫 번째 상위 개체가 됩니다.
첫 번째 상위 항목은 Planning 레코드 유형만 될 수 있습니다. Workfront 프로젝트는 계층 구조에서 다른 오브젝트 유형의 상위로 선택할 수 없습니다.
1. **개체 추가**&#x200B;를 클릭하여 계층 구조의 첫 번째 자식 항목인 두 번째 개체를 추가한 다음 드롭다운 메뉴에서 다른 개체를 선택합니다.
   ![필드를 선택하지 않은 새 계층 상자](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. **연결된 필드 선택**&#x200B;을 클릭하여 두 개체를 연결하는 필드를 나타냅니다.
1. (조건부) 두 객체 유형 사이에 연결된 필드가 있는 경우 목록에서 해당 필드를 선택합니다. 그렇지 않으면 **새 연결 추가**&#x200B;를 클릭하세요.

   >[!WARNING]
   >
   >연결된 필드를 만들 때 **연결된 레코드 형식에 해당 필드 만들기**&#x200B;를 선택하지 않은 경우 계속하려면 먼저 필드를 편집해야 합니다.

1. (조건부) 새 연결을 추가하는 경우 다음을 수행합니다.

   1. **이름** 상자에 연결된 필드의 이름을 추가하십시오.
   1. 다음 연결 유형 중에서 선택합니다.

      * **다대다**
      * **일대다**
      * **다대일**
      * **일대일**
   1. 다음 유형의 레코드 모양새 중 하나를 선택합니다.

      * **이름 및 이미지**
      * **이름**
      * **이미지**
자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.
   1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항) 위의 단계에 따라 계층에 최대 4개의 객체 유형을 계속 추가합니다. 먼저 모든 개체 유형을 추가한 다음 이들 사이에 연결 필드를 추가할 수 있습니다.
1. (선택 사항) 연결을 제거하려면 **제거** 아이콘 ![제거 아이콘](assets/minus-icon.png)을 클릭합니다.
1. 계층을 저장하려면 **저장**&#x200B;을 클릭하세요.

   >[!TIP]
   >
   >연결된 필드가 모두 없으면 **저장** 단추가 흐리게 표시됩니다.

   다음과 같은 상황이 발생합니다.

   * 작업 영역의 **계층** 섹션에 계층 구조가 추가되었습니다.
   * 연결 필드를 채우는 레코드는 레코드의 페이지로 이동할 때 이동 경로에 있는 모든 연결을 표시합니다.
1. (선택 사항) 계층 위로 마우스를 가져간 후 **자세히** 메뉴를 클릭한 후 다음 중 하나를 클릭합니다.

   * **편집**: 변경할 수 있는 **계층 구조 편집** 상자가 열립니다.
   * **삭제**: 이렇게 하면 계층이 영구적으로 삭제됩니다. 삭제된 계층은 복구할 수 없습니다. 연결 필드는 삭제되지 않습니다.





