---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 스마트 할당 만들기
description: 스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 리소스에 작업 항목을 할당할 때 Adobe Workfront이 사용자에게 제공하는 제안입니다. 스마트 할당에 대한 자세한 내용은 스마트 할당 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# 스마트 할당 만들기

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>   
  
<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> 
-->

스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 리소스에 작업 항목을 할당할 때 Adobe Workfront이 사용자에게 제공하는 제안입니다. 스마트 할당에 대한 자세한 내용은 [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 표준</p>
      또는
      <p>현재: 작업 시간 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 문제에 대한 액세스 편집</p> <p>프로젝트에 대한 보기 또는 상위 액세스 권한</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 문제에 할당할 수 있는 권한으로 기여하거나 더 높은 권한 부여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 스마트 할당 만들기

스마트 할당은 Workfront에서 할당할 수 있는 대부분의 위치에서 사용할 수 있습니다.

1. 다음 영역으로 이동하여 **할당** 또는 **할당 대상:** 필드:   

   * 작업 또는 문제 목록 또는 보고서
   * 작업 또는 문제 헤더
   * 작업 또는 문제 요약 패널
   * 홈 영역에 나열된 항목에 대한 지정 필드
   * 예약 또는 예약 영역의 작업 또는 문제
   * 업무 균형자의 작업 또는 문제

1. 할당 필드에 커서를 놓고 2초 동안 기다립니다. 다음 **제안된 할당** 또는 **다음은 몇 가지 권장 사항입니다** 목록이 표시됩니다.

   <!--check the casing for "assignments" should be lower case in task lists??-->

   <!--replace the last sentence above with this when we release smarter assignments:
   The **Suggested assignments** list displays. 
   NOTE (********and add preview tags for the note*****)
   The list header displays **Here are a few recommendations** instead of **Suggested assignments** in an issue list.
   -->

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   이 목록에 표시되는 사용자는 작업 또는 문제에 대한 스마트 할당 제안입니다.

   스마트 할당이 표시되는 위치에 대한 자세한 내용은 문서의 &quot;스마트 할당 제안 찾기&quot; 섹션을 참조하십시오 [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. Recommendations 목록에서 해당 이름을 클릭하여 사용자를 선택합니다. 클릭 **나에게 할당** 자신에게 작업 항목을 할당합니다.

   >[!TIP]
   >
   >제안이 없으면 제안 목록이 열리지 않습니다.

1. (선택 사항) 스마트 할당 목록에서 권장되는 사용자 중 하나를 사용하지 않으려면 원하는 사용자의 이름을 입력하고 목록에 표시될 때 이름을 선택합니다.
1. 클릭 **입력** 할당에 사용됩니다.

   선택한 사용자가 작업 또는 문제에 할당되었습니다.
