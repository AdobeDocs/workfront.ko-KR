---
product-area: projects
navigation-topic: approvals
title: 승인 보기
description: 승인 프로세스를 통해 프로젝트, 작업 및 문제에 대한 여러 단계의 승인을 유연하게 생성할 수 있습니다. Adobe Workfront 관리자는 승인 프로세스를 정의하여 시스템 전체에 일관성을 제공합니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: b0b83e8a8a2a076ec20691183605e3d25d10129d
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 승인 보기

승인 프로세스를 통해 프로젝트, 작업 및 문제에 대한 여러 단계의 승인을 유연하게 생성할 수 있습니다. Adobe Workfront 관리자는 승인 프로세스를 정의하여 시스템 전체에 일관성을 제공합니다.

승인 프로세스 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

Workfront에서 승인을 작업과 연결하는 방법에 대한 자세한 내용은 [새 승인 프로세스나 기존 승인 프로세스를 작업과 연결](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>승인과 연관된 객체에 대한 보기 이상의 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>승인과 연관된 오브젝트에 대한 이상 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## Adobe Workfront에서 승인 찾기

Workfront의 여러 영역에서 승인을 보거나 관리할 수 있습니다. 다양한 영역에서 승인을 관리하는 방법에 대한 자세한 내용은 [작업 승인](../../review-and-approve-work/manage-approvals/approving-work.md)을 참조하세요.

다음 영역에서 승인을 보거나 관리할 수 있습니다.

* 홈 영역에서

   * 모든 프로젝트, 작업, 문제, 타임시트, 문서 및 승인 대기 중인 액세스가 홈 영역의 내 승인 위젯에 표시됩니다.
   * 내가 제출한 승인 필터 옵션을 선택하면 직접 제출한 승인이 홈 영역의 내 승인 위젯에도 표시됩니다. 자세한 내용은 이 문서의 [홈 영역에서 승인을 위해 제출한 작업 검토](#review-work-you-submit-for-approval-in-the-home-area) 섹션을 참조하십시오.
   * 관련된 프로젝트, 작업 또는 문제가 해결됨, 보류 중, 마감됨 또는 취소됨으로 표시되면 홈 영역의 내 승인 위젯에서 승인이 제거됩니다.

  홈 사용에 대한 자세한 내용은 [홈 시작](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md)을 참조하세요.

* 프로젝트, 작업, 문제, 문서 또는 증명 헤더
* 프로젝트, 작업 또는 문제의 승인 섹션에서
* 보고서에서

  >[!NOTE]
  >
  >보고서의 승인에 대해 결정할 수 없습니다.

  승인 정보가 포함된 프로젝트, 작업, 문제 또는 문서 승인 보고서를 만들 수 있습니다.

  보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

## 홈 영역에서 승인을 위해 제출한 작업 검토 {#review-work-you-submit-for-approval-in-the-home-area}

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을(를) 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **내 승인** 위젯을 추가합니다.
1. (조건부) **필터** 드롭다운 메뉴를 클릭한 다음 **내가 제출한 승인**&#x200B;을 선택하여 제출한 승인을 확인합니다.


## 오브젝트의 승인 상태 보기

객체의 다음 섹션에서 객체의 승인 상태를 볼 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">업데이트 </td> 
   <td> <p>모든 승인 상태가 발생하면 표시합니다. 승인 상태가 <strong>업데이트</strong> 섹션에 표시된 다른 상태와 나란히 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">승인</td> 
   <td> <p>승인 프로세스의 각 단계 및 승인자의 승인 여부와 같은 승인 프로세스에 대한 자세한 정보를 표시합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 업데이트 영역을 사용하여 승인 상태를 봅니다. {#use-the-updates-area-to-view-an-approval-status}

프로젝트, 작업 또는 문제에 대한 승인이 시작되면 개체의 **업데이트** 탭에 승인 상태를 나타내는 상태가 표시됩니다. 승인 프로세스를 통해 객체가 전환될 때마다 새 상태가 표시됩니다. 여기에는 다음 이벤트가 포함됩니다.

* 승인 프로세스가 객체에 대해 시작됩니다. 상태가 변경되면 승인 프로세스가 시작됩니다.
* 개체가 거부되었습니다.
* 개체가 승인되었습니다.

>[!TIP]
>
>승인이 작업에 적용되는 경우 작업이 있는 프로젝트의 업데이트 탭이 아니라 작업의 업데이트 탭에 승인 업데이트가 표시됩니다.

### 승인 영역을 사용하여 승인 상태를 봅니다. {#use-the-approvals-area-to-view-an-approval-status}

현재 작업 중인 작업 또는 문제가 승인 프로세스에서 어디에 있는지 파악할 수 있습니다. 다음 정보를 볼 수 있습니다.

* 승인 프로세스의 단계
* 어떤 승인자가 이미 승인했습니까
* 아직 승인하지 않은 승인자

작업 또는 문제가 승인 프로세스에 있는 현재 상태를 보려면 다음과 같이 하십시오.

1. 승인이 연결된 프로젝트, 작업 또는 문제로 이동합니다.
1. 왼쪽 패널에서 **승인**&#x200B;을 클릭합니다. 먼저 **자세히 표시**&#x200B;를 클릭해야 할 수 있습니다.

   승인 탭에는 모든 과거 승인 경로 및 단계에 대한 전체 정보가 표시됩니다. 승인에 대해 누가 결정했는지 또는 팀, 작업 역할 또는 사용자에 대해 승인이 설정되었는지 정확하게 확인할 수 있습니다.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   승인 프로세스 만들기에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.
