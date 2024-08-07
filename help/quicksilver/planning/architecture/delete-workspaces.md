---
title: 작업 영역 삭제
description: 더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 작업 영역 삭제

{{planning-important-intro}}

Adobe Workfront Planning에서 작업 공간은 팀이 작업을 계획하는 중앙 집중식 위치입니다. 자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.

삭제하기 전에 다른 작업 영역에서 삭제하려는 작업 영역과 관련된 레코드 유형, 레코드, 필드 및 보기의 일부 또는 전체를 다시 만드는 것이 좋습니다.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Workfront Planning의 조기 액세스 단계에 조직을 등록해야 합니다. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>새로운 기능: 표준</p>
   <p>현재: 플랜</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>를 참조하십시오. </p>  
</td>
  </tr>

</tbody>
</table>

*액세스 요구 사항에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 작업 영역 삭제에 대한 고려 사항

* 작업 공간을 삭제하면 모든 레코드 유형, 레코드, 해당 필드 및 보기도 삭제됩니다.
* 삭제된 작업 영역과 여기에 포함된 정보는 복구할 수 없습니다.

## 작업 영역 삭제

{{step1-to-planning}}

1. (조건부) Workfront 관리자인 경우 **내 작업 공간**&#x200B;을 클릭하여 만든 작업 공간에 액세스하거나 **다른 작업 공간**&#x200B;을 클릭하여 나와 공유된 작업 공간에 액세스합니다. <!--change it to Workspaces I'm on-->

1. 삭제할 작업 공간의 카드를 클릭합니다.

   작업 영역 페이지가 표시됩니다.

<!--***********Replace the first step with this:*******

1. (Optional) Click **Show more** to display additional workspaces. The **Show more** link displays only when you have workspaces that display on more than two rows.
1. (Optional) ClicK **Show less** to limit the number of workspaces that display on the screen. 
1. To delete a workspace, do one of the following:

   * Hover over the workspace card, then click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the card, then click **De,ete**. 
   * Click a workspace card to open the workspace. 
   
   ***********Add (Conditional) If you clicked a workspace card,******to the step below****-->

1. 작업 영역 이름 옆의 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. 제공된 공간에 &quot;**delete**&quot;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다. 대/소문자를 구분하지 않습니다.

   작업 영역이 삭제되며 복구할 수 없습니다. 모든 레코드 종류, 레코드, 필드 및 연결된 보기도 삭제됩니다. <!--ensure this is right at or before GA-->
