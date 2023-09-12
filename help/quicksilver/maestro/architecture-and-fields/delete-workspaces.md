---
title: 작업 영역 삭제
description: 더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 작업 영역 삭제

>[!IMPORTANT]
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 비공개 베타 프로그램의 일부입니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe Maestro에서 작업 공간은 팀이 작업을 계획하기 위한 중앙 집중식 위치입니다. 자세한 내용은 [작업 공간 만들기](../architecture-and-fields/create-workspaces.md).

더 이상 관련이 없는 작업 공간은 삭제할 수 있습니다.

삭제하기 전에 다른 작업 영역에서 삭제하려는 작업 영역과 연관된 레코드 유형 및 분류의 일부 또는 전체를 다시 만드는 것이 좋습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>모든</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>모든</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">액세스 수준</td>
   <td> <p>모든</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">레이아웃 템플릿</td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/grant-access.md">Adobe 마에스트로에 대한 액세스 권한 부여</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 작업 영역 삭제에 대한 고려 사항

* 사용자 또는 조직의 모든 사용자가 만든 작업 영역을 삭제할 수 있습니다. <!--this will change with access levels and permissions-->
* 작업 공간을 삭제하면 모든 레코드 유형, 분류 및 해당 필드도 삭제됩니다. <!--asked Lilit because the confirmation says the records don't delete, but not sure how they can exist outside of a workspace?!-->
* 삭제된 작업 영역과 여기에 포함된 정보는 복구할 수 없습니다.

## 작업 영역 삭제

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) Workfront의 오른쪽 위 모서리에서 <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 그런 다음 을 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 삭제할 작업 영역을 선택합니다.
1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png) workspace 이름 옆에 있는 을 클릭합니다. **삭제**.
1. 클릭 **삭제** 확인할 수 있습니다.

   작업 영역이 삭제되며 복구할 수 없습니다. 모든 레코드 유형, 분류, 레코드 및 연관된 필드도 삭제됩니다. <!--ensure this is right after closed beta-->
