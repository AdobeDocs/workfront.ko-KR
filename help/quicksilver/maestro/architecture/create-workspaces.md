---
title: 작업 공간 만들기
description: 작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 작업 공간 만들기

{{maestro-important-intro}}

Adobe Workfront 계획에서 작업 공간은 팀이 작업을 계획하는 중앙 집중식 위치입니다.

작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다.

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
<p>Adobe Workfront Planning 마감된 베타 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
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
   또는
   <p>현재: 플랜</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront 계획에 대한 액세스 수준 제어가 없습니다.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작성한 작업 공간에 대한 관리 권한을 받습니다. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

액세스 요구 사항에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 작업 공간에 대한 고려 사항

* 조직 내의 특정 조직 단위에 대한 작업 공간을 만들어 각 단위의 고유한 작업 방식을 일치시킬 수 있습니다.
* 작업 영역에 포함된 레코드 유형은 조직 단위의 작업 라이프사이클을 반영해야 합니다.
* 작업 공간을 만들 때 사용자만 작업 공간에 액세스하고 관리할 수 있습니다. 다른 사용자가 동일한 공간에서 나와 공동 작업하려면 이 세그먼트를 다른 사용자와 공유해야 합니다. 자세한 내용은 [작업 영역 공유](/help/quicksilver/maestro/access/share-workspaces.md). 시스템 관리자는 작성하지 않은 작업 영역까지 모든 작업 영역을 관리할 수 있습니다.
* 조직의 Workfront 인스턴스에는 최대 1,000개의 작업 공간이 있을 수 있습니다.
* 작업 공간에는 각 작업 공간에 고유한 레코드 유형이 포함됩니다. <!--this might change-->

## 작업 공간 만들기

{{step1-to-maestro}}

1. (조건부) 환경에 작업 공간이 없는 경우 **작업 영역 만들기**

   또는 기존 작업 공간에서 작업 공간 이름의 오른쪽을 가리키는 아래쪽을 클릭한 다음 를 클릭합니다 **작업 영역 만들기**.

   ![](assets/workspace-drop-down-right-menu.png)

   Workfront 계획의 작업 영역 영역이 열립니다.
1. (선택 사항 및 조건부) 클릭 **미리 보기** 다음 사전 정의된 작업 공간 템플릿 내부:

   * 마케팅 관리
   * 영업 관리
   * 제품 관리

   각 템플릿과 연관된 운영 레코드 유형, 분류 및 필드 수가 표시됩니다.

   ![](assets/previewing-a-workspace-template.png)

   Workfront Planning 작업 공간 템플릿에 대한 자세한 내용은 다음을 참조하십시오. [작업 공간 템플릿 목록](../architecture/workspace-templates.md).

1. 클릭 **템플릿 사용** 선택한 템플릿에서 작업 공간 만들기 시작하기

   또는

   클릭 **작업 영역 만들기** 처음부터 작업공간을 만듭니다.

   다음 유형의 작업 공간에 대한 하나가 만들어집니다.

   * 처음부터 작업 영역을 만들 때 레코드 유형을 수동으로 추가할 수 있는 빈 작업 영역입니다.
   * 템플릿 중 하나를 사용할 때 추가로 사용자 정의할 수 있는 샘플 레코드 유형으로 채워진 작업 공간입니다.

1. 새 작업 영역의 헤더에서 작업 영역 이름 내부를 클릭하여 이름을 변경한 다음 Enter 키를 누릅니다

   또는

   다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png)헤더에서 작업 공간 이름 오른쪽에 있는 을 클릭합니다. **이름 바꾸기**.

1. (선택 사항 및 조건부) 작업 공간에 섹션이 이미 있으면 을 클릭합니다. **섹션 추가** 작업 공간에 새 섹션을 추가합니다. 섹션에는 여러 레코드 유형이 포함될 수 있습니다.

1. (선택 사항 및 조건부) 템플릿에서 작업 영역을 만들었다면 의 이름 내부를 클릭합니다. **운영 레코드 유형** 또는 **분류** 섹션

   또는

   섹션의 이름을 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **이름 바꾸기** 을 클릭하여 섹션의 이름을 변경합니다.

   >[!TIP]
   >
   >섹션을 만든 경우에도 모든 작업 영역에서 섹션의 이름을 변경할 수 있습니다.

1. (선택 사항) 섹션의 위치를 변경하려면 다음 중 하나를 수행합니다.

   * 섹션 이름 위로 마우스를 가져간 후 **grab** 아이콘 ![](assets/grab-icon.png)을 클릭한 다음 오른쪽 위치에 드래그 앤 드롭합니다.
   * 섹션 이름 위로 마우스를 가져간 후 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **위로 이동** 또는 **아래로 이동**. 섹션은 작업 영역 내에서 위나 아래로 이동합니다.

1. (선택 사항) 새 섹션을 추가하려면 다음 중 하나를 수행합니다.

   * 클릭 **섹션 추가** 을 클릭합니다.
   * 섹션 이름 위로 마우스를 가져간 후 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **위에 섹션 추가** 또는 **아래에 섹션 추가**.

1. (선택 사항) **레코드 유형 추가** 기록 유형을 작업 공간에 추가합니다.

   자세한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).


