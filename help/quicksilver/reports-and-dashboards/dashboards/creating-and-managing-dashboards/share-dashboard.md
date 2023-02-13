---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드 공유
description: Adobe Workfront 관리자는 액세스 수준을 지정할 때 대시보드를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 사용자에게 부여된 액세스 수준과 함께 사용자에게 공유 액세스 권한이 있는 특정 대시보드를 보거나 관리할 권한을 부여할 수도 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 대시보드 공유

Adobe Workfront 관리자는 액세스 수준을 지정할 때 대시보드를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 문제에 대한 액세스 권한 부여에 대한 자세한 내용은 [보고서, 대시보드 및 달력에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

사용자에게 부여된 액세스 수준과 함께 사용자에게 공유 액세스 권한이 있는 특정 대시보드를 보거나 관리할 권한을 부여할 수도 있습니다. 액세스 수준 및 권한에 대한 자세한 내용은 [액세스 수준 및 권한이 함께 작동하는 방법](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아니더라도 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

## 액세스 요구 사항

객체를 공유하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 또는 그 이상의 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>사용 권한 보기 또는 대시보드 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

대시보드를 공유하려면 먼저 대시보드를 만들어야 합니다.

대시보드 만들기에 대한 자세한 내용은 [대시보드 만들기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 대시보드 공유에 대한 고려 사항

아래 고려 사항 외에 다음을 참조하십시오 [보고서, 대시보드 및 달력 공유](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* 대시보드 작성자는 기본적으로 이 대시보드에 대한 관리 권한이 있습니다.

* 만든 대시보드를 다른 개인, 팀, 그룹, Job 역할 또는 회사와 공유할 수 있습니다. 또한 만든 다른 대시보드 및 사용자와 공유된 대시보드를 공유할 수도 있습니다.
* 시스템 전체에 걸쳐 표시함으로써 전체 조직과 공유할 수도 있습니다.
* 개별 대시보드를 공유하거나 목록에서 여러 개의 대시보드를 공유할 수 있습니다.
* 대시보드를 공유할 때는 기본적으로 사용자는 대시보드의 모든 보고서 개체에 대한 보기 권한을 상속합니다.

   Workfront에서 개체의 계층 구조에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   상속된 권한 보기에 대한 자세한 내용은 [객체에 대한 상속된 권한 보기](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## 대시보드 공유

목록에서 대시보드 하나 또는 여러 개의 대시보드를 공유하는 것은 동일합니다.

1. 대시보드 목록으로 이동하고 하나 이상의 대시보드를 선택한 다음 을 클릭합니다 **공유** ![](assets/share-icon.png).

   또는

   한 대시보드의 이름을 클릭한 다음 **대시보드 작업 >****공유**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. 에서 **사람, 팀, 역할, 그룹 또는 회사 추가...** 필드를 입력하고 대시보드를 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 이름을 클릭합니다.
1. (선택 사항) 시스템의 모든 사용자가 대시보드에 액세스할 수 있도록 하려면 **설정** 공유 대화 상자의 오른쪽 상단 모서리에 있는 아이콘을 선택한 다음 **시스템 전체에 표시**.

1. **저장**&#x200B;을 클릭합니다.
