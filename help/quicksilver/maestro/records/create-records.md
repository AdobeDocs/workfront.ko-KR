---
title: 레코드 만들기
description: Adobe 마에스트로에서 레코드는 레코드 유형의 인스턴스입니다. 개별 레코드를 만들려면 먼저 레코드 종류를 만들어야 합니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# 레코드 만들기

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe 마에스트로에서 레코드는 레코드 유형의 인스턴스입니다.

다음과 같은 유형의 레코드를 가질 수 있습니다.

* **운영 레코드**: 작업 관련 개체를 나타냅니다. 예를 들어 &quot;Campaign&quot;이라는 운영 레코드의 경우 &quot;Monthly Newsletter&quot; 또는 &quot;Summer Sale&quot;과 같은 이름의 레코드를 사용할 수 있습니다.
* **분류 레코드**: 작업 레코드와 연결할 수 있는 속성을 나타냅니다. 예를 들어 &quot;채널&quot;이라는 분류법 레코드 유형의 경우 &quot;이메일&quot;, &quot;소셜 미디어&quot; 또는 &quot;광고&quot;와 같은 분류법에 이름을 지정할 수 있습니다.

운영 레코드를 만드는 것은 분류 레코드 또는 분류를 만드는 것과 동일합니다.

다음 중 하나를 수행하여 Maestro에서 레코드를 만들 수 있습니다.

* 수동으로 Maestro 레코드 유형에 대해 만듭니다.
* 서드파티 애플리케이션에서 Maestro 레코드에 연결합니다.
* 외부 목록에서 정보를 복사하여 붙여 넣어 레코드를 만듭니다.

이 문서에서는 Maestro 레코드를 만드는 방법을 설명합니다. 테이블 또는 타임라인 보기에서 레코드 관리에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [표 보기 관리](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [타임라인 보기 관리](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">액세스 수준</td>
   <td> <p>임의</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">레이아웃 템플릿</td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 수동으로 레코드 유형에 추가하여 레코드 만들기 <!--in a record type table (I don't think you can create them elsewhere right now)-->

레코드 유형 페이지의 표 보기에서 레코드를 만들 수 있습니다.

{#step1-to-maestro}

마지막으로 액세스한 작업공간은 기본적으로 열립니다. 작업 공간 만들기에 대한 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).
1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.
선택한 유형의 모든 레코드가 테이블 뷰에 표시됩니다.

1. (조건부) 레코드 유형 페이지가 표 보기에서 열리지 않으면 **보기** 드롭다운 메뉴를 사용하여 기존 메뉴 중 하나 선택 **표 보기** ![](assets/table-view-icon.png) 또는 클릭 **뷰 만들기 > 테이블** 테이블 뷰를 생성합니다.

1. 새 레코드를 추가하려면 **새로 만들기 &lt; 레코드 유형 이름 >** 테이블의 마지막 행에서

   또는

   클릭 **Shift + Enter** 표의 열 또는 행에서 키보드에 있는 경우 빈 행이 표시됩니다.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. 새 레코드에 대한 정보를 새 행에 입력하십시오.

   >[!NOTE]
   >
   >  * 레코드에 대한 필수 필드가 없습니다. 그러나 레코드를 서로 연결할 때 레코드를 식별하는 데 도움이 되므로 레코드에 이름을 추가하는 것이 좋습니다.
   >
   >  * 다른 레코드 종류 또는 계산된 필드를 참조하는 필드는 읽기 전용 필드입니다.

1. 각 행에 대한 정보를 계속 추가한 다음 **입력** 키보드에서 을(를) 클릭하여 변경 내용을 저장합니다.

<!--1. (Optional) Use the following keyboard shortcuts to undo or redo adding new records: 

    * **Undo**: CTRL/CMD + Z
    * **Redo**: CTRL/CMD + Shift + Z-->

## 다른 애플리케이션에서 연결하여 레코드 만들기

다른 응용 프로그램에서 레코드를 Maestro 연결 레코드에 연결하여 가져올 수 있습니다. 이렇게 하면 서드파티 애플리케이션 연결 개체에 대한 Maestro 레코드 유형이 생성됩니다. 원래 Maestro 레코드에 연결하는 레코드는 서드파티 애플리케이션 연결 객체 Maestro 레코드 유형 테이블 보기에 표시됩니다.

1. 에 설명된 대로 Maestro 레코드 유형을 만듭니다. [레코드 유형 만들기](../architecture/create-record-types.md).

1. 이전 단계에서 생성한 레코드 유형에 대해 Maestro 레코드를 생성합니다. 자세한 내용은 섹션을 참조하십시오 [수동으로 레코드 유형에 추가하여 레코드 만들기](#create-records-by-manually-adding-them-to-a-record-type) 이 문서에서.

1. 생성한 Maestro 레코드 유형의 서드파티 애플리케이션에서 객체 유형에 대한 연결을 생성합니다. 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

1. 이전 단계에서 생성한 연결된 레코드 필드를 사용하여 위에서 생성한 Maestro 레코드에 타사 애플리케이션의 레코드를 추가합니다. 자세한 내용은 [레코드 연결](../records/connect-records.md).

   Maestro에서 다음 항목이 만들어집니다.

   * 연결된 레코드 필드에서 연결한 타사 레코드 종류를 참조하는 읽기 전용 Maestro 레코드 종류.

     예를 들어 Maestro 레코드 유형을 Workfront 프로젝트에 연결하는 경우 &quot;Workfront 프로젝트&quot;라는 읽기 전용 레코드 유형이 동일한 작업 영역에 생성됩니다.
   * 서드파티 레코드 유형 페이지의 읽기 전용 레코드. 타사 응용 프로그램에서 가져온 레코드는 읽기 전용으로 유지되며 원래 응용 프로그램에서만 업데이트할 수 있습니다.

## 외부 목록에서 정보를 복사하여 붙여 넣어 레코드 만들기

1. 섹션에 설명된 대로 Maestro에서 테이블 보기에서 레코드 만들기를 시작합니다 [수동으로 레코드 유형에 추가하여 레코드 만들기](#create-records-by-manually-adding-them-to-a-record-type) 이 문서에서.

   Maestro 테이블 보기에 새 레코드 정보로 채울 열이 있는지 확인합니다.

1. 클릭 **새로 만들기 &lt; 레코드 유형 이름 >** 테이블의 마지막 행에 새 레코드를 원하는 만큼 추가합니다.

   예를 들어 다른 응용 프로그램에서 10개의 새 레코드에 대한 정보를 붙여넣으려면 10개의 행을 테이블 보기에 추가합니다.

1. 다른 응용 프로그램에서 Maestro에서 가져올 레코드 목록을 만듭니다.

   예를 들어 Excel 스프레드시트를 사용하여 목록을 만들 수 있습니다.

   목록에는 표 형식의 정보가 포함되어야 합니다.

   >[!TIP]
   >
   > 목록의 열에는 Maestro에 있는 기존 필드에 대한 정보가 포함되어야 합니다.
   >
   > 원하는 필드가 이미 Maestro에서 만들어졌고 시트의 정보가 Maestro의 각 필드와 일치하는 올바른 형식으로 표시되는지 확인합니다.

1. 서드파티 응용 프로그램에서 여러 행과 열을 선택한 다음 첫 번째 새 레코드부터 시작하여 레코드 유형 테이블 보기에 정보를 붙여 넣습니다.

   Maestro에서 다음 정보를 가져옵니다.

   * 행에는 새 레코드가 포함됩니다
   * 열은 레코드의 필드에 대한 정보를 채웁니다.
