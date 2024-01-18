---
navigation-topic: business-case-and-scorecards
title: 비즈니스 사례 목표 만들기
description: 비즈니스 사례를 만드는 과정의 일부로, 일련의 목표를 생성하여 프로젝트의 목표를 정의할 수 있습니다. 비즈니스 사례 목표는 프로젝트 완료를 위해 Portfolio 관리자 또는 프로젝트 스폰서에게 전달하는 데 사용됩니다.
author: Alina
feature: Work Management
exl-id: c5f4c095-ea21-4205-a747-e8923de7030f
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# 비즈니스 사례 목표 만들기

비즈니스 사례를 만드는 과정의 일부로, 일련의 목표를 생성하여 프로젝트의 목표를 정의할 수 있습니다. 비즈니스 사례 목표는 프로젝트 완료를 위해 Portfolio 관리자 또는 프로젝트 스폰서에게 전달하는 데 사용됩니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>프로젝트의 개별 비즈니스 사례에 연결되지 않은 조직의 전략적 목표를 생성할 수 있습니다. 전략적 목표를 만들려면 Adobe Workfront 목표에 액세스할 수 있어야 합니다. 그런 다음 비즈니스 사례 이외의 프로젝트와 연결할 수 있습니다. Workfront 목표를 사용하여 목표를 만드는 방법에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 목표 개요](../../../workfront-goals/goal-management/wf-goals-overview.md).

프로젝트에 대한 비즈니스 사례 목표를 생성할 때 다음 사항을 고려하십시오.

* 비즈니스 사례 목표는 프로젝트별로 다릅니다. 한 프로젝트에서 다른 프로젝트로 목표를 복사하거나 시스템 수준에서 목표를 설정할 수 없습니다. 각 프로젝트의 수준에서 정의되어야 합니다.
* Adobe Workfront 관리자 또는 그룹 관리자는 프로젝트의 비즈니스 사례에 표시되기 전에 프로젝트에 대한 목표 섹션을 활성화해야 합니다. 프로젝트의 비즈니스 사례 필드 활성화에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 목표는 프로젝트의 비즈니스 사례에서 필수 섹션이 아닙니다.

  비즈니스 사례의 목표 섹션이 정의되지 않은 경우에도 프로젝트는 Portfolio 최적화 도구에서 우선 순위 지정할 점수를 받을 수 있습니다.

  Portfolio 최적화 프로그램 점수에 대한 자세한 내용은 [프로젝트에 스코어카드를 적용하고 정렬 점수 생성](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

* 비즈니스 사례 목표에 대해서는 보고할 수 없습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 이상 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 프로젝트의 비즈니스 사례에 목표 추가

1. 비즈니스 사례 목표를 정의할 프로젝트로 이동합니다.
1. 클릭 **왼쪽 패널의 비즈니스 사례.**

   비즈니스 사례가 표시됩니다.

   ![](assets/business-case-page-info-goals-expenses-nwe-350x123.png)

1. 다음에서 **목표** 섹션, 클릭 **목표 편집**.

1. 목표를 지정합니다.
다음에서 **중요도** 드롭다운 메뉴에서 중요도를 선택합니다.

   * 가장 높음
   * 높음
   * 중간
   * 낮음
   * 가장 낮음

     ![](assets/g1-350x76.png)

     목표의 중요도 수준은 사용자 지정할 수 없습니다.

1. (선택 사항) 다른 목표를 추가하려면 **다른 목표 추가** 5단계와 6단계를 반복합니다.
1. 클릭 **저장**.
