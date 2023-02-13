---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Adobe Workfront 관리자는 Workfront에서 통화 환율을 설정할 수 있습니다.
description: 환율 설정
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# 환율 설정

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Adobe Workfront 관리자는 Workfront에서 통화 환율을 설정할 수 있습니다. 여기에는 다음 항목이 포함되어 있습니다.

* Workfront 시스템의 기본 통화 설정
* 현재 환율에 맞게 Workfront에서 환율을 업데이트하는 중
* 여러 통화에 대한 환율을 구성(이렇게 하면 사용자가 개별 프로젝트에 대한 기본 통화를 선택할 수 있음)

환율은 Workfront의 모든 재무 요소에 영향을 줍니다. 기본 통화는 주어진 프로젝트 또는 작업 역할에 대해 대체되지 않는 한 시스템 전체에서 모든 프로젝트에 대한 기본 통화입니다. 보고서 또는 목록에서 재무 정보를 볼 때 기본 통화와 다른 시스템에서 사용할 수 있는 통화 또는 프로젝트 통화와 다른 통화로 표시하도록 선택할 수도 있습니다. 자세한 내용은 [고유한 환율을 사용하여 재무 데이터 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

프로젝트 및 작업 역할에 대해 Workfront에서 기본 통화 재정의를 위한 자세한 내용은 다음 문서를 참조하십시오.

* [프로젝트 통화 변경](../../../manage-work/projects/project-finances/change-project-currency.md)
* [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

환율을 설정하는 방법은 사용자가 주어진 프로젝트에 대한 환율을 수정할 수 있는지 여부에 영향을 줍니다.

>[!IMPORTANT]
>
>Workfront의 환율은 동적이지 않습니다. 환율 변경 사항이 발생하면 설정한 값을 업데이트해야 합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 환율 설정

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **프로젝트 환경 설정** > **환율.**

1. 클릭 **통화 추가.**
1. 통화 이름을 입력하고 드롭다운 목록에 나타나면 클릭합니다.

1. 제공된 필드에 시스템에서 기본 통화로 설정된 통화와 관련된 선택한 통화의 환율을 지정합니다.
1. (선택 사항) Workfront에 대한 기본(기본) 통화로 통화를 설정합니다.

   시스템 전체에서 모든 프로젝트 및 보고서에 대한 기본값으로 사용되는 통화입니다.

1. 클릭 **저장** 변경 사항을 저장하려면 을 클릭합니다.

## 사용자가 프로젝트에 대한 기본 통화를 수정할 수 있도록 설정

다음 조건이 충족될 경우 사용자는 프로젝트에 대한 기본 통화를 수정할 수 있습니다.

* 사용자는 환율을 관리할 수 있는 계획 라이센스가 있습니다.

   자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Workfront 시스템에서 두 개 이상의 통화가 활성화되어 있습니다.

사용자가 주어진 프로젝트에서 기본 통화를 변경하는 방법에 대한 자세한 내용은 [프로젝트 통화 변경](../../../manage-work/projects/project-finances/change-project-currency.md).

## 사용자가 작업 역할에 대한 기본 통화를 수정할 수 있도록 설정

다음 조건이 충족되면 사용자가 작업 역할에 대한 통화를 수정할 수 있습니다.

* 사용자에게 작업 역할에 대한 관리자 액세스 권한이 있는 계획 라이센스가 있습니다.

   자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Workfront 시스템에서 두 개 이상의 통화가 활성화되어 있습니다.

사용자가 주어진 작업 역할에서 기본 통화를 변경하는 방법에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
