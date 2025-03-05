---
title: 삭제된 레코드 복원
description: Adobe Workfront Planning의 최근에 삭제된 영역에서 삭제된 레코드를 복구할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: bddd0dcd2263bd65420a17e4b9cc74336877719f
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# 삭제된 레코드 복원

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning의 최근에 삭제된 영역에서 삭제된 레코드를 복구할 수 있습니다.

레코드 삭제에 대한 자세한 내용은 [레코드 삭제](/help/quicksilver/planning/records/delete-records.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 </a>에 대한 또는 더 높은 권한 제공 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 삭제된 레코드 복구에 대한 고려 사항

* 레코드는 최근에 삭제된 상자에 30일 동안 저장됩니다. 30일 후 레코드는 Workfront Planning에서 영구적으로 삭제됩니다.
* 삭제된 레코드가 다른 레코드와 연결된 경우 연결된 레코드는 삭제되지 않지만 삭제된 레코드의 정보도 삭제됩니다. 삭제된 레코드를 복원하면 연결된 레코드에서 정보가 복원됩니다.
* 레코드를 대량으로 복원할 수 있습니다.
* 레코드가 삭제되면 다음 정보가 최근에 삭제된 BIN에 저장됩니다.
   * **이름**: 레코드의 기본 필드에 있는 정보입니다. 레코드 기본 필드에 대한 자세한 내용은 [기본 필드 개요](/help/quicksilver/planning/fields/primary-field-overview.md)를 참조하세요.
   * **삭제된 날짜**: 레코드가 삭제된 시간과 날짜입니다.
   * **최근 삭제된 시간**: 레코드가 삭제된 이후 시간입니다. 현재 날짜보다 30일 이상 전에 삭제된 레코드는 최근에 삭제된 BIN에 표시되지 않습니다.
   * **삭제자**: 레코드를 삭제한 사용자의 이름입니다.

## 삭제된 레코드 복원

1. 레코드를 삭제한 레코드 유형 페이지로 이동합니다.
1. 레코드 종류 페이지 보기의 오른쪽 상단에 있는 **실행 취소** 아이콘 ![](assets/undo-icon.png)을(를) 클릭한 다음 **최근에 삭제됨**&#x200B;을(를) 클릭합니다.

   **최근에 삭제됨** 상자가 표시됩니다.

   ![](assets/recently-deleted-box.png)

1. 삭제할 레코드를 선택한 다음 **복원** > **복원**&#x200B;을 클릭합니다. 두 개 이상의 레코드를 선택할 수 있습니다.

   복원이 성공하면 화면 하단에 성공 알림이 표시됩니다.
1. 테이블 보기로 이동하여 복원된 레코드를 검토합니다.
