---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 최근에 삭제된 그룹 항목 보기 및 관리
description: 그룹 영역에서 관리하는 그룹을 볼 때 최근에 삭제된 작업 항목, 문서 및 템플릿을 보고 필터링하고 복원하고 내보낼 수 있습니다.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 1%

---

# 최근에 삭제된 그룹 항목 보기 및 관리

그룹 영역에서 관리하는 그룹을 볼 때 다음과 같은 방법으로 최근에 삭제된 프로젝트, 작업, 문제, 문서 및 템플릿을 보고 작업할 수 있습니다.

* 최근에 삭제된 항목 목록 보기, 필터링 및 그룹화
* 선택한 최근에 삭제된 항목 복원
* 최근에 삭제된 항목 목록 내보내기

그룹 위에 그룹이 있는 경우 해당 관리자는 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

삭제된 항목에 대한 자세한 내용은 [삭제된 항목 관리](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md)를 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr>
   <td>액세스 수준 구성</td> 
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr>
  <tr> 
   <td>개체 권한</td>
   <td>삭제된 항목은 그룹 또는 해당 하위 그룹과 연결되어 있어야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 최근에 삭제된 그룹 항목 보기 및 관리

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

1. 그룹 이름을 클릭합니다.
1. 왼쪽 패널에서 **최근에 삭제됨**&#x200B;을 클릭합니다.
1. 그룹에서 최근에 삭제된 항목을 보고 관리할 다음 탭 중 하나를 엽니다.

   * 프로젝트
   * 작업
   * 문제
   * 문서
   * 템플릿

   각 탭에는 현재 그룹 또는 해당 하위 그룹에 속하고 지난 30일 이내에 삭제된 해당 객체 유형의 항목이 나열됩니다.

   >[!NOTE]
   >
   >누군가가 프로젝트를 삭제한 경우 해당 개별 작업, 문제 및 문서가 함께 삭제되었습니다. 작업, 문제, 문서 또는 템플릿 탭에는 개별적으로 표시되지 않습니다. 그러나 프로젝트를 복원하면 이러한 모든 하위 개체도 프로젝트로 복원됩니다.
   >
   >
   >누군가 작업, 문제, 문서 또는 템플릿을 개별적으로 삭제한 경우 해당 탭에서 보고 관리할 수 있습니다.

1. 다음 작업 중 하나를 완료합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>개체 복원</p> </td> 
      <td> <p>최대 10개의 개체를 선택한 다음 <strong>복원</strong>을 클릭합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>탭에서 전체 개체 목록 내보내기</p> </td> 
      <td> <p><strong>내보내기</strong>를 클릭합니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>목록의 정보 표시 변경</p> </td> 
      <td> <p>목록 위의 오른쪽 상단 모서리에서 <strong>필터</strong>를 사용하여 제공한 기준에 따라 표시되는 내용을 정의합니다. 열로 표시되는 필드를 정의하려면 <strong>보기</strong>를 사용하십시오. 항목을 범주로 그룹화하려면 <strong>그룹화</strong>을 사용하세요.</p> </td> 
     </tr> 
    </tbody> 
   </table>
