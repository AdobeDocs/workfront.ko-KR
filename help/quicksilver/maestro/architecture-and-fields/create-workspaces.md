---
title: 작업 공간 만들기
description: 작업 공간은 팀에서 사용하는 운영 레코드 유형 및 분류의 모음이며 팀의 작업 주기를 나타냅니다. Maestro에서 작업 공간을 완전히 사용자 지정할 수 있습니다.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 작업 공간 만들기

>[!IMPORTANT]
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe Maestro에서 작업 공간은 팀이 작업을 계획하기 위한 중앙 집중식 위치입니다.

작업 공간은 팀에서 사용하는 운영 레코드 유형 및 분류의 모음이며 팀의 작업 주기를 나타냅니다. Maestro에서 작업 공간을 완전히 사용자 지정할 수 있습니다.

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

## 작업 공간에 대한 고려 사항

* 조직 내의 특정 조직 단위에 대한 작업 공간을 만들어 각 단위의 고유한 작업 방식을 일치시킬 수 있습니다.
* 작업 영역에 포함된 레코드 종류 및 분류는 조직 단위의 작업 주기를 반영해야 합니다.
* 작업 영역을 만들면 조직의 모든 사용자가 작업 영역을 보거나 편집하거나 삭제할 수 있습니다.  <!--this will change with access levels and permissions-->
* 조직에서 최대 1,000개의 작업 영역을 가질 수 있습니다.
* 작업 공간에는 각 작업 공간에 고유한 레코드 유형이 포함됩니다. <!--this might change-->

## 작업 공간 만들기

1. (조건부) 시스템에 작업 공간이 없는 경우 **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) Workfront의 오른쪽 위 모서리에서 <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 그런 다음 을 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   또는 기존 작업 공간에서 작업 공간 이름의 오른쪽을 가리키는 아래쪽을 클릭한 다음 를 클릭합니다 **작업 영역 만들기**.

   ![](assets/workspace-drop-down-right-menu.png)

   그러면 Maestro의 Workspaces 영역이 열립니다.
1. (선택 사항 및 조건부) 클릭 **미리 보기** 다음 사전 정의된 작업 공간 템플릿 내부:

   * 마케팅 관리
   * 영업 관리
   * 제품 관리

   각 템플릿과 연관된 운영 레코드 유형, 분류 및 필드 수가 표시됩니다.

   ![](assets/previewing-a-workspace-template.png)

   Maestro 작업 영역 템플릿에 대한 자세한 내용은 [작업 공간 템플릿 목록](../architecture-and-fields/workspace-templates.md).

1. 클릭 **템플릿 사용** 선택한 템플릿에서 작업 공간 만들기 시작하기

   또는

   클릭 **작업 영역 만들기** 처음부터 작업공간을 만듭니다.

   다음 유형의 작업 공간에 대한 하나가 만들어집니다.

   * 레코드 유형을 수동으로 추가할 수 있는 빈 작업 영역입니다.
   * 추가로 사용자 정의할 수 있는 샘플 레코드 유형으로 채워진 작업 공간입니다.

1. 새 작업 영역의 헤더에서 작업 영역 이름 내부를 클릭하여 이름을 변경한 다음 Enter 키를 누릅니다

   또는

   다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png)헤더에서 작업 공간 이름 오른쪽에 있는 을 클릭합니다. **이름 바꾸기**.

1. (선택 사항) **레코드 유형 추가** 기록 유형을 작업 공간에 추가합니다.

   자세한 내용은 [레코드 유형 만들기](../architecture-and-fields/create-record-types.md).

1. (선택 사항) **분류 추가** 작업공간에 분류를 추가합니다.

   자세한 내용은 [분류 만들기](../architecture-and-fields/create-a-taxonomy.md).