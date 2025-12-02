---
title: 다른 Workspace에서 기존 레코드 유형 추가
description: 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 다른 작업 영역에서 생성된 기존 레코드 유형을 추가할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 1%

---


# 다른 작업 영역에서 기존 레코드 유형 추가

{{planning-important-intro}}

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

작업 영역 관리자는 다른 작업 영역에 있는 레코드 유형을 Adobe Workfront Planning에서 관리하는 작업 영역에 추가할 수 있습니다.

작업 영역 관리자는 먼저 레코드 유형을 글로벌 레코드 유형으로 지정해야 기존 레코드 유형으로 관리하는 작업 영역에 레코드 유형을 추가할 수 있습니다. Workspace 관리자는 레코드 유형의 작업 영역 간 설정을 정의하여 레코드 유형을 만들거나 편집할 때 글로벌로 지정할 수 있습니다.

자세한 내용은 [레코드 형식에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하십시오.

이 문서에서는 기존 레코드 유형에서 레코드 유형을 추가하는 방법에 대해 설명합니다.

전역 레코드 형식에서 작업 영역에 레코드를 추가하기 전에 문서 [작업 영역 간 레코드 형식 개요](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)를 참조하십시오.


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
<ul><li><p>모든 Workfront 패키지 및 Planning Plus 패키지</p></li>
또는
<li><p>모든 워크플로우 및 Planning Prime 또는 Ultimate 패키지</p></p></li></ul>
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

<!--Old:
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
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## 다른 작업 영역에서 기존 레코드 유형을 추가하여 레코드 유형 만들기

>[!NOTE]
>
>하나 이상의 다른 기본 작업 영역에 전역으로 지정된 레코드 유형이 하나 이상 있는지 확인합니다.
>
>자세한 내용은 [레코드 형식에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하십시오.

1. 레코드 유형을 만들려는 작업 영역(보조 작업 영역)으로 이동합니다.
1. 문서 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)에 설명된 대로 레코드 종류 만들기를 시작한 다음 **기존 항목 추가**&#x200B;를 클릭합니다. <!--check this - the option might have been renamed in the UI-->

   ![다른 작업 영역에서 추가할 수 있는 옵션과 함께 레코드 종류를 추가하는 모달](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >시스템의 다른 작업 영역에 추가하도록 구성된 레코드 형식이 없으면 **기존 항목 추가** 옵션이 표시되지 않습니다.

1. **계속**&#x200B;을 클릭합니다.
1. **레코드 종류 선택** 상자에서 기존 작업 영역에서 추가할 레코드 종류의 카드를 클릭한 다음 **추가**&#x200B;를 클릭합니다.

   레코드 종류가 선택한 보조 작업 영역에 추가되고 **글로벌 레코드 종류** 아이콘 ![](assets/global-icon.png)이(가) 레코드 종류의 카드에 표시됩니다.

   다음과 같은 상황이 발생합니다.

   * 기존 글로벌 레코드 유형에서도 다음 정보가 추가됩니다.

      * 모든 원본 필드
      * 모든 레코드 연결
   * 해당 작업 영역에 대해 적어도 보기 권한이 있는 경우에만 동일한 글로벌 레코드 유형을 사용하는 다른 작업 영역에서 추가된 레코드를 볼 수 있습니다.
   * 읽기 전용 **Workspace** 필드가 새 레코드 형식 테이블 보기에 추가되었습니다. 필드에는 각 레코드가 생성된 작업 공간이 표시됩니다.

     >[!NOTE]
     >
     >새 레코드 종류의 모양, 추가 설정 또는 원본 필드는 편집할 수 없습니다. 원본 작업공간에서만 레코드 종류 및 원본 필드와 설정을 편집할 수 있습니다.

1. (선택 사항) 을 클릭한 다음, 새로 추가된 레코드 유형을 작업 공간 내의 임의의 섹션으로 끌어다 놓습니다.
1. (선택 사항) 새 레코드 종류의 카드 또는 해당 페이지의 레코드 종류 이름 오른쪽에 있는 **자세히** 메뉴를 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   자세한 내용은 문서 [레코드 종류 삭제](/help/quicksilver/planning/architecture/delete-record-types.md)의 &quot;전역 레코드 종류 삭제&quot; 섹션을 참조하십시오.

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—Lilit를 사용하여 자동화 또는 요청 양식을 보조 글로벌 RT에 추가할 수 있는지 확인??—/ yes인 경우 해당 문서에 대한 링크가 있는 단계 추가—>







