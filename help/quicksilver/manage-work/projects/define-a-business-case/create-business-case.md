---
navigation-topic: business-case-and-scorecards
title: 프로젝트에 대한 비즈니스 사례 만들기
description: 비즈니스 사례를 사용하여 프로젝트를 요청하고 프로젝트의 목적, 예산 및 잠재적 혜택을 정의할 수 있습니다. Portfolio 관리자 또는 프로젝트 스폰서는 비즈니스 사례의 정보를 사용하여 프로젝트를 승인하기 전에 분석하고 우선 순위를 지정합니다.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 0%

---

# 프로젝트에 대한 비즈니스 사례 만들기

비즈니스 사례를 사용하여 프로젝트를 요청하고 프로젝트의 목적, 예산 및 잠재적 혜택을 정의할 수 있습니다. Portfolio 관리자 또는 프로젝트 스폰서는 비즈니스 사례의 정보를 사용하여 프로젝트를 승인하기 전에 분석하고 우선 순위를 지정합니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>계획 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트, 재무 데이터 및 리소스 관리에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

비즈니스 사례를 통해 프로젝트를 요청할 때 다음 사항을 고려하십시오.

* Adobe Workfront 관리자 또는 그룹 관리자는 비즈니스 사례 섹션이 프로젝트에 표시되기 전에 이를 활성화해야 합니다.\
  시스템 수준에서 비즈니스 사례의 섹션을 활성화하는 방법에 대한 자세한 내용은 문서 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

  비즈니스 사례 영역에 대한 자세한 내용은 문서 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)를 참조하십시오.

* 프로젝트가 Portfolio 최적화 도구에서 점수를 받으려면 목표 영역을 제외하고 비즈니스 사례의 모든 영역을 완료해야 합니다. 목표 영역 완료는 선택 사항입니다. 이 영역이 완료되지 않은 경우에도 프로젝트는 Portfolio 최적화 도구에서 점수를 받습니다.

  스코어카드 작업 및 Portfolio 최적화 프로그램에 대한 자세한 내용은 [프로젝트에 스코어카드 적용 및 정렬 점수 생성](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) 문서를 참조하십시오.

## 비즈니스 사례 만들기

1. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **프로젝트**&#x200B;를 클릭합니다.
1. **새 프로젝트**&#x200B;를 클릭하고 **프로젝트 요청**&#x200B;을 선택합니다.\
   기본적으로 프로젝트는 **아이디어** 상태에 배치됩니다.

   >[!CAUTION]
   >
   >Workfront 인스턴스에서 아이디어 상태가 삭제된 경우 프로젝트가 프로젝트 환경 설정 영역에 정의된 새 프로젝트의 기본 상태에 배치됩니다. 프로젝트 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

1. 프로젝트의 이름을 지정한 다음 Enter 키를 누릅니다.
1. (선택 사항) 프로젝트의 작업 분류 구조를 만들려면 **자세히** 아이콘 ![](assets/qs-more-icon-on-an-object.png)을 클릭한 다음 **템플릿 첨부**&#x200B;를 클릭합니다.

   또는

   프로젝트에 작업을 수동으로 추가하기 시작합니다.

1. (조건부) 템플릿을 첨부하도록 선택한 경우 템플릿을 프로젝트에 계속 첨부합니다
1. 왼쪽 패널에서 **비즈니스 사례**&#x200B;를 클릭합니다.
1. (선택 사항) **프로젝트 정보 편집**&#x200B;을 클릭합니다. 

   비즈니스 사례의 프로젝트 정보 섹션에서 필드를 편집하는 방법에 대한 자세한 내용은 문서 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)의 [프로젝트 정보](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) 섹션을 참조하십시오.

1. (선택 사항) **목표 편집**&#x200B;을 클릭합니다.

   비즈니스 사례의 목표 섹션 편집에 대한 자세한 내용은 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md) 문서의 [목표](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) 섹션을 참조하십시오.

1. (선택 사항)**경비 편집**&#x200B;을 클릭합니다.

   비즈니스 사례의 경비 섹션 편집에 대한 자세한 내용은 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md) 문서의 [경비](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) 섹션을 참조하십시오.

1. (선택사항) 자원 예산 책정 영역을 사용하여 자원의 예산을 책정하고 프로젝트의 작업 역할과 연관된 예산 인건비를 얻습니다. 자세한 내용은 [비즈니스 사례의 리소스 예산](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)을 참조하세요.

   >[!TIP]
   >
   >여기에 표시되는 정보는 시스템 레벨 리소스 예산 책정 도구에 표시되는 정보와 동일합니다.

1. (선택 사항) **위험 편집**&#x200B;을 클릭하여 이 프로젝트에 잠재적인 위험을 추가합니다. 비즈니스 사례에 위험을 추가하는 방법에 대한 자세한 내용은 문서 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)의 [위험](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) 섹션을 참조하십시오.
1. (선택 사항) **이 프로젝트에 스코어카드 추가** 드롭다운 메뉴에서 ******스코어카드**&#x200B;를 선택합니다.

   스코어카드를 프로젝트에 첨부하려면 먼저 만들어야 합니다.

   스코어카드에 대한 자세한 내용은 [프로젝트에 스코어카드 적용 및 정렬 점수 생성](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) 문서를 참조하십시오.

1. (선택 사항) **사용자 지정 Forms** 드롭다운 메뉴에서 **사용자 지정 양식**&#x200B;을(를) 선택합니다.

   사용자 지정 Forms을 프로젝트에 첨부하려면 먼저 만들어야 합니다.

   사용자 지정 Forms에 대한 자세한 내용은 문서 [사용자 지정 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. **제출**&#x200B;을 클릭합니다.

   프로젝트 상태가 **요청됨**(으)로 변경되었으며 비즈니스 사례를 승인하도록 제출되었습니다.

   비즈니스 사례 승인에 대한 자세한 내용은 [비즈니스 사례 승인](../../../manage-work/projects/define-a-business-case/approve-business-case.md) 문서를 참조하십시오.

1. (선택 사항) 비즈니스 사례를 완료한 후 비즈니스 사례의 사본을 .pdf 파일로 내보낼 수 있습니다. 비즈니스 사례를 .pdf 파일로 내보내는 방법에 대한 자세한 내용은 문서 [비즈니스 사례 영역 개요](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)의 &quot;비즈니스 사례 내보내기&quot; 섹션을 참조하십시오.
