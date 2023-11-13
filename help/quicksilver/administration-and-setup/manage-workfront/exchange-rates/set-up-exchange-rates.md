---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 환율 설정
description: Adobe Workfront 관리자는 Workfront에서 통화 환율을 설정할 수 있습니다.
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: b0cf0a5ec6b932267c8714b966638d8da93331b8
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# 환율 설정

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Adobe Workfront 관리자는 Workfront에서 통화 환율을 설정할 수 있습니다. 여기에는 다음이 포함됩니다.

* Workfront 시스템에 대한 기본 통화 설정
* 현재 환율에 일치하도록 Workfront의 환율 업데이트
* 여러 통화에 대한 환율을 구성합니다(이렇게 하면 사용자가 개별 프로젝트에 대한 기본 통화를 선택할 수 있음).

환율은 Workfront의 모든 금융 요소에 영향을 줍니다. 기본 통화는 주어진 프로젝트 또는 작업 역할에 대해 재정의되지 않는 한 시스템 전체의 모든 프로젝트에 대한 기본 통화입니다. 보고서나 목록에서 재무 정보를 볼 때 기본 통화나 프로젝트의 기본 통화와 다른 시스템에서 사용할 수 있는 통화로 표시하도록 선택할 수도 있습니다. 자세한 내용은 [고유 환율로 재무 데이터 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

프로젝트 및 작업 역할의 Workfront 기본 통화 재정의에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [프로젝트 통화 변경](../../../manage-work/projects/project-finances/change-project-currency.md)
* [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

환율을 설정하는 방식은 사용자가 주어진 프로젝트에 대한 환율을 수정할 수 있는지 여부에 영향을 줍니다.

>[!IMPORTANT]
>
>Workfront의 환율은 동적이지 않습니다. 환율이 변경되면 설정하는 값을 업데이트해야 합니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가적인 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 환율 설정

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **프로젝트 환경 설정** > **환율.**

1. 클릭 **통화를 추가합니다.**
1. 통화 이름을 입력한 다음 드롭다운 목록에 나타나면 통화를 클릭합니다.

1. 제공된 필드에 선택한 통화의 환율을 지정합니다. 이 환율은 시스템에서 기본 통화로 설정된 통화와 관련이 있습니다.
1. (선택 사항) 통화를 Workfront의 기본(기본) 통화로 설정합니다.

   시스템 전체의 모든 프로젝트 및 보고서에 대한 기본값으로 사용되는 통화입니다.

1. 클릭 **저장** 변경 사항을 저장합니다.

## 사용자가 프로젝트에 대한 기본 통화를 수정할 수 있도록 설정

사용자는 다음 조건이 충족될 때 프로젝트의 기본 통화를 수정할 수 있습니다.

* 사용자는 환율에 대한 관리 액세스 권한이 있는 플랜 라이선스를 보유하고 있습니다.

  자세한 내용은 [사용자에게 특정 영역에 대한 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Workfront 시스템에서 두 개 이상의 통화가 활성화됩니다.

사용자가 주어진 프로젝트에서 기본 통화를 변경할 수 있는 방법에 대한 자세한 내용은 [프로젝트 통화 변경](../../../manage-work/projects/project-finances/change-project-currency.md).

## 사용자가 작업 역할에 대한 기본 통화를 수정할 수 있도록 설정

사용자는 다음 조건이 충족될 때 작업 역할의 통화를 수정할 수 있습니다.

* 사용자에게 작업 역할에 대한 관리 액세스 권한이 있는 플랜 라이선스가 있습니다.

  자세한 내용은 [사용자에게 특정 영역에 대한 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Workfront 시스템에서 두 개 이상의 통화가 활성화됩니다.

사용자가 주어진 작업 역할에서 기본 통화를 변경할 수 있는 방법에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
