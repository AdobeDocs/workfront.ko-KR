---
navigation-topic: get-started-with-workfront
title: 우선 순위 작업 목록 열 사용자 정의
description: 우선 순위의 작업 목록에서 열을 사용자 정의하여 작업 방식을 지원할 수 있습니다.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: e4232fbe-1b5c-4614-8613-3b0e25ffee46
TQID: https://experienceleague.adobe.com/YIqeZbiTZH00yXJ6LnQrpEZuHvW4Y5QZVkYU3OquWqE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1880d4370059ad654f91c6f40a0a787c51c1e54e
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 5%

---

# 우선 순위 작업 목록 열 사용자 정의

{{preview-fast-release-general}}

<!--I think this article can point to the Enhanced lists article for managing the view-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


우선 순위의 작업 목록에서 열을 사용자 정의하여 작업 방식을 지원할 수 있습니다.

우선 순위에는 사용자에게 할당된 작업 항목이 표시됩니다. 팀에 할당된 작업 항목을 볼 수 없습니다.

<!--
>[!NOTE]
>
>You cannot add custom data to columns at this time.
-->

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 패키지</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스</strong></td> 
   <td> 
   <p>검토자 이상</p>
   <p>밝거나 높음</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>업데이트가 있는 오브젝트에 대한 보기 또는 편집 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>오브젝트에 대한 액세스 보기</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 우선 순위 작업 목록 열 사용자 정의

### 열 활성화 또는 비활성화

{{step1-to-priorities}}

1. 화면 왼쪽에서 **열**&#x200B;을 클릭합니다.

   <span class="preview">미리 보기 환경의 샘플 이미지:</span>
   ![열](assets/columns-new-060226.png)

   프로덕션 환경의 샘플 이미지:
   ![열](assets/columns-new.png)

1. 토글을 사용하여 작업 목록에서 열을 표시하거나 숨깁니다.

### 열 순서 바꾸기

{{step1-to-priorities}}

1. 화면 왼쪽에서 **열**&#x200B;을 클릭합니다.
1. **드래그** 아이콘을 클릭하고 열을 원하는 위치로 이동합니다. 작업 목록에서 열을 자동으로 이동합니다.
   ![열 순서 바꾸기](assets/reorder-columns-new.png)

>[!NOTE]
>
>이름 열은 고정되어 이동할 수 없습니다.

<div class="preview">

### 열 관리자를 사용하여 열 추가 및 제거

{{step1-to-priorities}}

1. 목록의 오른쪽 위 모서리에 있는 + 아이콘을 클릭하여 **열 관리자** 상자를 엽니다.
1. 열을 추가하거나 제거한 다음 **저장**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >목록 보기에 기존 필드만 추가할 수 있습니다. 작업 및 문제에 대한 기본 필드와 사용자 정의 필드를 모두 열로 추가할 수 있습니다.

열 관리자에 대한 자세한 내용은 문서 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)에서 [열 관리자가 있는 열 추가 및 제거](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) 섹션을 참조하십시오.

</div>

### 우선 순위 목록에서 행 높이 변경

{{step1-to-priorities}}

1. **행 높이** 아이콘을 클릭합니다.

   행의 세로 길이가 업데이트됩니다. 다음 선택 사항 중 하나를 선택합니다.

   * 짧음
   * 표준. 이것이 기본 선택입니다.
   * 보통
   * 높음

   목록이 즉시 업데이트됩니다.

<div class="preview">

## 우선 순위 목록에 대한 보기 관리

보기는 사전 설정 설정으로 목록의 열, 필터 및 그룹화를 정의합니다.

기본 보기는 우선순위 목록에 지정됩니다. 자신만의 보기를 만들고 공유할 수도 있습니다.

{{step1-to-priorities}}

1. 목록의 왼쪽 상단 모서리에서 드롭다운 보기 메뉴를 확장하여 다른 보기를 선택하거나 **새 보기**&#x200B;를 클릭하여 다른 보기를 만듭니다.
1. 보기에 포함할 열, 필터 및 그룹화를 업데이트합니다.

   보기에 대한 변경 사항은 자동으로 저장됩니다. 다음에 이 보기를 적용하면 열 및 필터 설정이 설정된 방식으로 유지됩니다.

보기에 대한 자세한 내용은 문서 [고급 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)에서 [고급 목록 요소 업데이트](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#update-enhanced-list-elements) 섹션을 참조하십시오.

</div>
