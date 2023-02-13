---
navigation-topic: business-case-and-scorecards
title: 프로젝트에 대한 비즈니스 사례 생성
description: 업무 사례를 사용하여 프로젝트를 요청하고 프로젝트에 대한 목적, 예산 및 잠재적 이익을 정의할 수 있습니다. Portfolio 관리자 또는 프로젝트 스폰서는 비즈니스 사례의 정보를 사용하여 프로젝트를 승인하기 전에 분석하고 우선 순위를 지정합니다.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# 프로젝트에 대한 비즈니스 사례 생성

업무 사례를 사용하여 프로젝트를 요청하고 프로젝트에 대한 목적, 예산 및 잠재적 이익을 정의할 수 있습니다. Portfolio 관리자 또는 프로젝트 스폰서는 비즈니스 사례의 정보를 사용하여 프로젝트를 승인하기 전에 분석하고 우선 순위를 지정합니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>계획 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트, 재무 데이터 및 리소스 관리에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 이상 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

비즈니스 사례를 통해 프로젝트를 요청할 때 다음 사항을 고려하십시오.

* Adobe Workfront 관리자 또는 그룹 관리자가 비즈니스 사례 섹션을 활성화해야 프로젝트에 표시됩니다.\
   시스템 수준에서 비즈니스 사례의 섹션 활성화에 대한 자세한 내용은 문서를 참조하십시오 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   비즈니스 케이스의 영역에 대한 자세한 내용은 문서를 참조하십시오 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* 프로젝트가 Portfolio 최적기에서 점수를 받도록 하려면 목표 영역을 제외한 비즈니스 사례의 모든 영역을 완료해야 합니다. 목표 영역을 완료하는 것은 선택 사항입니다. 이 영역이 완료되지 않더라도 프로젝트는 Portfolio 최적기에서 점수를 받습니다.

   스코어카드 작업 및 Portfolio 최적기 작업에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트에 스코어카드를 적용하고 정렬 점수를 생성합니다](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## 비즈니스 사례 만들기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 **프로젝트**.
1. 클릭 **새 프로젝트** 을(를) 선택합니다. **프로젝트 요청**.\
   기본적으로 프로젝트는 **아이디어** 상태.

   >[!CAUTION]
   >
   >Workfront 인스턴스에서 아이디어 상태가 삭제된 경우 프로젝트는 프로젝트 환경 설정 영역에 정의된 대로 새 프로젝트의 기본 상태에 배치됩니다. 프로젝트 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. 프로젝트 이름을 지정한 다음 Enter 키를 누릅니다.
1. (선택 사항) **자세히** 아이콘 ![](assets/qs-more-icon-on-an-object.png), 그런 다음 **템플릿 첨부**&#x200B;를 눌러 프로젝트의 작업 분류 구조를 생성합니다.

   또는

   프로젝트에 수동으로 작업 추가를 시작합니다.

1. (조건부) 템플릿을 첨부하도록 선택한 경우 계속해서 프로젝트에 템플릿을 첨부합니다
1. 클릭 **비즈니스 사례** 왼쪽 패널에 표시됩니다.
1. (선택 사항) **프로젝트 정보 편집**. 

   비즈니스 케이스의 프로젝트 정보 섹션에서 필드 편집에 대한 자세한 내용은 섹션을 참조하십시오 [프로젝트 정보](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) 기사 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (선택 사항) **목표 편집**.

   비즈니스 사례의 목표 섹션 편집에 대한 자세한 내용은 섹션을 참조하십시오 [목표](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) 기사 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (선택 사항)**비용 편집**.

   비즈니스 사례의 비용 섹션 편집에 대한 자세한 내용은 섹션을 참조하십시오 [비용](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) 기사 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (선택 사항) 자원 예산 영역을 사용하여 자원의 예산을 책정하고 프로젝트의 Job 역할과 연관된 예산책정된 노무비를 얻습니다. 자세한 내용은 [비즈니스 사례의 예산 자원](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >여기에 표시되는 정보는 시스템 레벨 자원 예산 책정 도구에 표시된 정보와 동일합니다.

1. (선택 사항) **위험 편집** 이 프로젝트에 잠재적 위험을 추가하려면 비즈니스 사례에 위험 추가에 대한 자세한 내용은 [위험](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) 문서의 섹션 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (선택 사항)**스코어카드** 에서 **이 프로젝트에 스코어카드**** 추가** 드롭다운 메뉴

   스코어카드는 프로젝트에 첨부하기 전에 만들어야 합니다.

   스코어카드에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트에 스코어카드를 적용하고 정렬 점수를 생성합니다](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (선택 사항) **사용자 지정 양식** 에서 **사용자 지정 Forms** 드롭다운 메뉴

   사용자 지정 Forms을 만들어야 프로젝트에 첨부할 수 있습니다.

   사용자 지정 Forms에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 클릭 **제출**.

   프로젝트 상태가 (으)로 변경되었습니다. **요청** 비즈니스 사례를 승인하도록 제출됩니다.

   비즈니스 사례 승인에 대한 자세한 내용은 문서를 참조하십시오 [비즈니스 사례 승인](../../../manage-work/projects/define-a-business-case/approve-business-case.md).

1. (선택 사항) 비즈니스 사례를 완료한 후 복사본을 .pdf 파일로 내보낼 수 있습니다. 비즈니스 사례를 .pdf 파일로 내보내는 방법에 대한 자세한 내용은 문서의 &quot;비즈니스 사례 내보내기&quot; 섹션을 참조하십시오 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
