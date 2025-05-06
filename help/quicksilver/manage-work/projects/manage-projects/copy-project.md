---
product-area: projects
navigation-topic: manage-projects
title: 프로젝트 복사
description: 처음부터 프로젝트를 만드는 대신 프로젝트를 복사할 수 있습니다. 한 번에 한 프로젝트만 복사할 수 있습니다. 프로젝트를 일괄적으로 복사할 수 없습니다.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 4%

---

# 프로젝트 복사

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

처음부터 프로젝트를 만들지 않고 기존 프로젝트에서 프로젝트를 복사할 수 있으므로 시간을 절약할 수 있습니다.

프로젝트를 일괄적으로 복사할 수 없습니다.

>[!IMPORTANT]
>
>다음 항목은 기존 프로젝트에서 새 프로젝트로 복사되지 않습니다.
>
>* 문제
>* 결제 요율
>* 청구 기록
>* 메모
>* 시간
>* 프로젝트 간 전임 작업
>* 예산 시간
>
>다음 항목은 항상 기존 프로젝트에서 새 프로젝트에 복사됩니다.
>
>* 작업
>* 템플릿
>* 위험
>* 대기열 설정 정보
>* Portfolio 및 프로그램
>* 스코어카드
>* 작업 기본 정보(작업 기본 승인 프로세스, 작업 기본 사용자 지정 Forms)
>
> 원래 프로젝트의 작업 날짜가 새 프로젝트에 복사됩니다. 작업 날짜를 업데이트하려면 프로젝트의 시작 또는 완료 날짜(일정 모드에 따라)를 변경해야 합니다. 작업 제한으로 인해 프로젝트의 날짜를 변경할 수 없습니다.

## 액세스 요구 사항

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.
이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront 플랜</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront 라이선스</p> </td> 
   <td> <p>새로운 기능: 표준 </p> 
   <p>또는</p>
   <p>현재: 플랜 </p>

</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>액세스 수준 구성 </td> 
   <td> <p><span>개의 프로젝트를 만들고</span>개 복사하는 기능을 가진 프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>프로젝트에 대한 권한 이상 보기</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 단일 프로젝트 복사

프로젝트를 복사하면 원래 프로젝트의 일부 정보도 새 프로젝트에 복사됩니다. 복사 프로세스 중에 새 프로젝트에 복사하지 말아야 할 항목을 지정할 수도 있습니다.

프로젝트를 복사하려면 다음 작업을 수행하십시오.

{{step1-to-projects}}

1. 프로젝트 목록에서 복사할 프로젝트를 선택한 다음 프로젝트 이름의 오른쪽에 있는 **자세히** 아이콘 ![추가 메뉴](assets/more-icon.png)를 클릭합니다.

   또는

   프로젝트 목록 또는 보고서로 이동하여 프로젝트를 선택한 다음 목록 맨 위에 있는 **자세히** 아이콘 ![추가 메뉴](assets/more-icon.png)를 클릭합니다.

1. **자세히** 드롭다운 메뉴에서 **복사**&#x200B;를 클릭합니다. **[프로젝트 이름]** 복사 대화 상자가 나타납니다.

1. (선택 사항) **프로젝트 이름**&#x200B;을(를) 업데이트합니다. 기본적으로 새 이름은 **원본 프로젝트 이름 [의 복사본]**&#x200B;입니다.

   ![프로젝트 상자 복사](assets/copy-of-project-box.png)

1. **상태**&#x200B;를 선택하세요. 기본적으로 원본 프로젝트의 상태가 선택되어 있습니다.

1. (선택 사항) 새 프로젝트로 복사하지 않으려는 항목의 선택을 취소합니다. 다음 표에서는 항목을 선택 해제할 때 발생하는 상황을 설명합니다.


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">모두 선택</td> 
      <td> <p>모든 옵션을 선택하고 새 프로젝트에서 나열된 모든 필드와 개체를 지웁니다. </p>

   <p> 이 옵션을 선택 해제하면 모든 항목이 선택 해제됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">할당</td> 
      <td>모든 프로젝트 및 작업 할당을 제거합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">진행</td> 
      <td>모든 작업의 진행률을 제거하고 새 작업으로 표시합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 데이터</td> 
      <td> <p>프로젝트의 사용자 정의 양식에 대한 정보와 다음 항목과 연결된 사용자 정의 양식에 대한 정보를 제거합니다.</p> 
       <ul> 
        <li>작업</li> 
        <li>경비</li> 
        <li> 문서</li> 
       </ul> 
      <p>사용자 정의 양식은 작업, 경비, 문서 및 프로젝트에 첨부된 상태로 유지되지만 양식의 사용자 정의 필드에 있는 정보는 새 프로젝트에 복사되지 않습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문서</td> 
      <td> <p>문서 탭의 문서 버전, 링크된 문서 및 폴더를 모두 제거합니다.</p> <p>기본적으로 문서 증명 및 승인은 다른 프로젝트에 복사할 수 없습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">모든 전임 작업</td> 
      <td> <p>프로젝트의 작업 간 모든 전임 작업 관계를 제거합니다. </p> <p>

   프로젝트 간 전임 작업은 선택 여부에 관계없이 새 프로젝트로 이전되지 않습니다. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">예산 시간</td> 
      <td> <p>복사된 프로젝트에서 프로젝트 비즈니스 사례의 리소스 계획 영역에 예산 책정된 시간을 제거합니다.</p> 
    <p>
   새 프로젝트가 시나리오 플래너의 이니셔티브에 연결되어 있지 않으므로 시나리오 플래너를 사용하여 예산 책정된 시간은 새 프로젝트에 복사되지 않습니다. 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">시나리오 플래너를 사용하여 비즈니스 사례에서 리소스 예산</a>을 참조하세요.</p>
   </tr></td>
    <tr> 
      <td role="rowheader">재무 정보</td> 
      <td> <p>다음 영역의 정보를 제거합니다. </p> 
       <ul> 
        <li>프로젝트의 재무 하위 탭</li> 
        <li> 비즈니스 사례의 계획된 이익</li> 
        <li>모든 작업의 재무 정보<br></li> 
       </ul> <p>프로젝트 재무 하위 탭에 대한 자세한 내용은 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">프로젝트 재무 영역의 정보 관리</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인 진행</td> 
      <td>작업 또는 프로젝트와 관련된 모든 승인을 제거합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td> 작업 또는 프로젝트와 관련된 미리 알림을 제거합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td>작업 또는 프로젝트와 관련된 비용을 제거합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">권한</td> 
      <td> 작업 또는 프로젝트에 대한 모든 사용자의 권한을 제거합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **프로젝트 복사**&#x200B;를 클릭합니다. 복사된 프로젝트가 생성됩니다.
