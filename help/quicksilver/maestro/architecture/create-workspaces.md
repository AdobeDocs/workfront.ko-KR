---
title: 작업 공간 만들기
description: 작업 공간은 팀에서 사용하는 운영 레코드 유형 및 분류의 모음이며 팀의 작업 주기를 나타냅니다. Maestro에서 작업 공간을 완전히 사용자 지정할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 작업 공간 만들기

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
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
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
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
   <td> <p>Maestro에 대한 액세스 수준 제어 없음</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작성한 작업 공간에 대한 관리 권한을 받습니다. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

액세스 요구 사항에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
* 작업 공간을 만들 때 사용자만 작업 공간에 액세스하고 관리할 수 있습니다. 다른 사용자가 동일한 공간에서 나와 공동 작업하려면 이 세그먼트를 다른 사용자와 공유해야 합니다. 자세한 내용은 [작업 영역 공유](/help/quicksilver/maestro/access/share-workspaces.md).
* 조직에서 최대 1,000개의 작업 영역을 가질 수 있습니다.
* 작업 공간에는 각 작업 공간에 고유한 레코드 유형이 포함됩니다. <!--this might change-->

## 작업 공간 만들기

{{step1-to-maestro}}

1. (조건부) 환경에 작업 공간이 없는 경우 **작업 영역 만들기**

   또는 기존 작업 공간에서 작업 공간 이름의 오른쪽을 가리키는 아래쪽을 클릭한 다음 를 클릭합니다 **작업 영역 만들기**.

   ![](assets/workspace-drop-down-right-menu.png)

   그러면 Maestro의 Workspaces 영역이 열립니다.
1. (선택 사항 및 조건부) 클릭 **미리 보기** 다음 사전 정의된 작업 공간 템플릿 내부:

   * 마케팅 관리
   * 영업 관리
   * 제품 관리

   각 템플릿과 연관된 운영 레코드 유형, 분류 및 필드 수가 표시됩니다.

   ![](assets/previewing-a-workspace-template.png)

   Maestro 작업 영역 템플릿에 대한 자세한 내용은 [작업 공간 템플릿 목록](../architecture/workspace-templates.md).

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

   자세한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

1. (선택 사항) **분류 추가** 작업공간에 분류를 추가합니다.

   자세한 내용은 [분류 만들기](../architecture/create-a-taxonomy.md).
