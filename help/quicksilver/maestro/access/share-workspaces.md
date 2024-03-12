---
title: 작업 공간 공유
description: Adobe Workfront 계획 기능에서 작업할 때 공동 작업을 보장하기 위해 다른 사용자와 작업 영역을 공유할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 4c62b567fa1ebec37fc64831757eb67d4a048c1f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 2%

---


<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# 작업 공간 공유

{{maestro-important-intro}}

Adobe Workfront 계획 기능에서 작업할 때 공동 작업을 보장하기 위해 다른 사용자와 작업 영역을 공유할 수 있습니다.

>[!NOTE]
>
>작업 영역에 권한을 부여해도 다른 사용자에게 레코드 유형 페이지의 보기에 대한 권한이 부여되지 않습니다. 다른 사용자와 공유하려면 레코드 유형 페이지에서 개별 보기에 대한 권한을 부여해야 합니다. 자세한 내용은 [보기 공유](/help/quicksilver/maestro/access/share-views.md).


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
<p>Adobe Workfront 계획 기능 비공개 베타 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
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
   <p>새로운 기능: 표준</p>
   또는
   <p>현재: 플랜 </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> Adobe Workfront 계획 기능에 대한 액세스 제어가 없습니다</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 권한 관리</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 마에스트로 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> <p>자세한 내용은 <a href="/help/quicksilver/maestro/access/access-overview.md">액세스 개요</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

## 작업 공간에 대한 권한 공유

다음 사용자는 다른 사용자와 작업 영역을 공유할 수 있습니다.

* 시스템 관리자는 작성하지 않은 작업 영역을 포함하여 모든 작업 영역을 공유할 수 있습니다.
* 다른 모든 사용자는 관리 권한이 있는 작업 영역만 공유할 수 있습니다.

다른 사용자와 작업 공간을 공유하려면 다음을 수행하십시오.

{{step1-to-maestro}}

1. 공유할 작업 영역을 연 다음 **공유** 화면의 오른쪽 상단에 있습니다.

   ![](assets/share-button-on-workspace-top-right.png)

1. 다음에서 **작업 공간 액세스 권한 부여 대상:** 필드에서 사용자 또는 그룹 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

   ![](assets/sharing-ui-with-groups.png)

1. 드롭다운 메뉴에서 다음 권한 수준 중 하나를 선택합니다.
   * 보기
   * 참여
   * 관리

     권한 수준 및 사용자가 각 수준에 대해 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront 계획 기능의 공유 권한 개요](../access/sharing-permissions-overview.md).
1. 클릭 **링크 복사** 를 클릭하여 작업 영역에 대한 링크를 클립보드에 복사합니다.
1. 복사한 링크를 다른 사용자와 공유합니다. 링크를 받은 사용자가 활성 사용자여야 하며 작업 영역에 액세스할 수 있도록 Workfront에 로그인해야 합니다.
1. **저장**&#x200B;을 클릭합니다.


## 작업 공간에 대한 권한 제거


{{step1-to-maestro}}

1. 권한을 제거할 작업 영역을 연 다음 **공유** 화면의 오른쪽 상단에 있습니다.
1. 사용자 또는 그룹 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 을 클릭합니다 **제거**.
1. **저장**&#x200B;을 클릭합니다.

   제거된 그룹에 속한 사용자나 사용자는 더 이상 작업공간이나 해당 객체에 액세스할 수 없습니다.