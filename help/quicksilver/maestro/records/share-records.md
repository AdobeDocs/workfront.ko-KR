---
title: 레코드 공유
description: 다른 사용자와 레코드를 공유하여 공동 작업을 향상시킬 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 1%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 레코드 공유

>[!IMPORTANT]
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

다른 사용자와 공동 작업하려면 레코드를 다른 사용자와 공유할 수 있습니다.

다음과 같은 방법으로 Maestro 레코드를 공유할 수 있습니다.

* 페이지가 열릴 때 브라우저에서 레코드의 세부 정보 페이지의 링크를 복사합니다.

* 레코드 유형의 테이블 보기에서 레코드를 볼 때 레코드의 세부 정보 페이지에 대한 링크를 복사합니다.

이 문서에서는 레코드 유형의 테이블 보기에서 레코드의 세부 정보 페이지에 대한 링크를 복사하는 방법에 대해 설명합니다.

<!-- add information about permissions, like:
- in the table below, you must have at least View permissions to the record
- the user you're sharing with must have at least View permissions to the record to view it
- etc - others???-->

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

## 레코드 유형 테이블 보기에서 레코드 링크 공유

1. 다음을 클릭합니다. **메인 메뉴** ![](assets/main-menu-workfront.png) 오른쪽 위 모서리에서 <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> 그런 다음 을 클릭합니다. **마에스트로**.

   마지막으로 액세스한 작업 영역이 열립니다.
1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. (조건부) **보기** 테이블 오른쪽 위 모서리에서 드롭다운 메뉴를 사용하여 테이블 뷰를 선택합니다. 레코드 유형에 마지막으로 액세스했을 때 타임라인 보기에서 확인하지 않은 경우 기본 보기여야 합니다.

   선택한 레코드 유형과 연관된 레코드가 테이블 뷰에 표시됩니다.
1. 레코드 행을 마우스 오른쪽 단추로 클릭

   또는

   레코드 이름 위로 마우스를 가져간 다음 기타 메뉴를 클릭합니다. ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **링크 복사**.

   ![](assets/contextual-menu-for-record-row.png)

   링크가 클립보드에 복사됩니다.

1. 링크를 이메일 또는 채팅 창에 붙여넣어 다른 사용자와 공유할 수 있습니다. 사용자가 링크를 수신하면 레코드의 세부 정보 페이지가 열립니다.

   >[!TIP]
   >
   >세부 정보 페이지에 있는 레코드의 필드는 해당 레코드의 테이블 보기에서 사용할 수 있는 동일한 필드입니다.


   <!--add there when it will be available: if they have access to this record-->