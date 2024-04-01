---
title: 보기 공유
description: 보기를 다른 사용자와 공유하여 Adobe Workfront Planning 사용 시 공동 작업을 보장할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# 보기 공유

{{maestro-important-intro}}

보기를 다른 사용자와 공유하여 Adobe Workfront Planning에서 레코드 작업 시 공동 작업을 보장할 수 있습니다.

작업 영역에 권한을 부여해도 다른 사용자에게 레코드 유형 페이지의 보기에 대한 권한이 부여되지 않습니다. 다른 사용자와 공유하려면 레코드 유형 페이지에서 개별 보기에 대한 권한을 부여해야 합니다.

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
<p>Adobe Workfront Planning 마감된 Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
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
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> Adobe Workfront Planning에 대한 액세스 제어가 없습니다. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td> <p>보기에 대한 권한 관리</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> <p>자세한 내용은 <a href="/help/quicksilver/maestro/access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 보기에 대한 권한 공유

만든 보기 또는 관리 권한이 있는 보기를 공유할 수 있습니다.

>[!NOTE]
>
>시스템 관리자는 자신이 만들지 않은 보기를 보거나 공유할 수 없습니다. 공유된 보기에만 액세스하거나 공유할 수 있습니다.
>
>시스템 관리자는 보기에 대한 관리 권한만 가질 수 있습니다.

{{step1-to-maestro}}

1. 보기를 공유할 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다.

   그러면 레코드 유형 페이지가 열립니다.

1. 보기 탭에서 공유할 보기를 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png) 뷰 이름의 오른쪽에 있는 **공유**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. 다음에서 **보기 액세스 권한 부여 대상** 필드에서 사용자 또는 그룹 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 드롭다운 메뉴에서 다음 권한 수준 중 하나를 선택합니다.
   * 보기
   * 관리

     권한 수준 및 사용자가 각 수준에 대해 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront Planning의 공유 권한 개요](../access/sharing-permissions-overview.md).

     <!--System administrators always receive Manage permissions to views shared with them.-->

1. 클릭 **링크 복사** 를 클릭하여 보기에 대한 링크를 클립보드에 복사합니다.
1. 복사한 링크를 다른 사용자와 공유합니다. 링크를 받은 사용자는 활성 사용자여야 하며 레코드 유형 페이지에 액세스하여 선택한 보기에 표시할 수 있도록 Workfront에 로그인해야 합니다.
1. **저장**&#x200B;을 클릭합니다.

## 보기에 대한 권한 제거

{{step1-to-maestro}}

1. 보기를 공유할 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다. 그러면 레코드 유형 페이지가 열립니다.
1. 보기 드롭다운 메뉴에서 공유할 보기를 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png) 뷰 이름의 오른쪽에 있는 **공유**.
1. 제거할 사용자 또는 그룹을 찾은 다음 **제거** 사용 권한 드롭다운 메뉴에서 사용자 또는 그룹 이름 오른쪽에 있는 권한
1. 클릭 **저장**.
제거된 그룹에 속한 사용자 또는 사용자는 더 이상 보기에 액세스할 수 없습니다. 보기에 액세스하지 못하도록 제거된 사용자에 대한 알림은 없습니다.
