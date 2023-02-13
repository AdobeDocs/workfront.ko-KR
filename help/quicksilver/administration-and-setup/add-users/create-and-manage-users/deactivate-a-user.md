---
title: 사용자 비활성화 또는 다시 활성화
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront 관리자는 사용자를 비활성화하거나 다시 활성화할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# 사용자 비활성화 또는 다시 활성화

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>Adobe Admin Console에서 사용자를 비활성화하는 방법에 대한 지침은 문서에서 &quot;사용자 제거&quot; 섹션을 참조하십시오 [개별 사용자 관리](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 또는 Adobe Admin Console 관리자에게 문의하십시오.
>
>조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 다른 절차 목록은 [플랫폼 기반의 관리 차이점(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

사용자는 조직을 나갈 수 있으며 Adobe Workfront에서 사용자를 제거해야 할 수 있습니다. 이 경고는 업데이트에 사용자를 추가하거나 이 사용자가 작동하도록 할당할 때 다른 사용자에게 혼동을 초래할 수 있으므로 시스템에서 활성 상태를 유지하지 말아야 합니다. 사용자를 비활성화하면 다른 사용자가 시스템에서 사용자를 검색할 때 더 이상 사용자의 이름이 표시되지 않습니다.

관리자는 설정 영역에서 비활성 사용자를 볼 수 있습니다.

언제든지 사용자를 다시 활성화할 수 있습니다.

>[!IMPORTANT]
>
>조직을 떠난 사용자를 삭제하는 대신 비활성화하는 것이 좋습니다. 사용자가 삭제되면 해당 사용자와 연결된 Workfront의 모든 기록이 유실됩니다. 여기에는 작업 지정, 노트, 시간, 문서 및 이전에 생성된 기타 모든 객체와 관련된 작업이 포함됩니다.
>
>Workfront에서 사용자를 비활성화하면 Workfront과 디지털 언어 교정 모두에 대한 사용자의 라이선스가 제거됩니다. 또한 사용자에게 더 이상 작업을 할당할 수 없습니다. 사용자가 비활성화되면 해당 사용자의 Workfront 라이선스 및 언어 교정 라이선스를 다른 사용자가 사용할 수 있습니다. 비활성화된 사용자의 프로필에 있는 다른 모든 정보는 그대로 유지됩니다.
>
>삭제 및 사용자 비활성화의 영향에 대한 자세한 내용은 [사용자 삭제](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

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
   <td> <p>플랜 </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>. </p> </li> 
     <li> <p><b>사용자</b> 액세스 수준에서 설정 <b>편집</b> 액세스, 사용 <b>만들기</b> 둘 중 적어도 하나 <b>사용자 관리자</b> 옵션 사용 <b>설정 세부 조정</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>이 두 옵션 중 사용자가 <b>관리자(그룹 사용자)</b> 이 활성화되어 있으면 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> <p>에 대한 자세한 정보 <b>사용자</b> 액세스 수준에서 설정하는 방법은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 비활성화

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).

1. 사용자를 선택하고 자세히 아이콘을 클릭합니다 ![](assets/more-icon.png)를 클릭한 다음 **비활성화**.

1. 클릭 **비활성화** 이 표시되는 상자에 나타납니다.

## 사용자 비활성화 예약

관리자는 실제로 조직을 떠나기 전에 사용자를 비활성화 상태로 표시할 수 있습니다. 예를 들어 계약상 구속되는 사용자와 작업하는 경우, 사용자는 제한된 기간 동안 시스템에 있으며 종료 날짜를 알고 있습니다. 해당 날짜에 비활성화되도록 예약할 수 있습니다.

Workfront 관리자 및 Plan 라이선스 사용자는 사용자 프로필에서 비활성화 날짜를 확인할 수 있습니다.

사용자를 비활성화하도록 예약하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).

1. 사용자 이름을 선택합니다.

   또는

   (선택 사항) 여러 사용자를 선택하여 비활성화 일정을 일괄적으로 예약합니다.

1. 편집 아이콘을 클릭합니다 ![](assets/edit-icon.png).
1. 표시되는 사용자 편집 상자에서 **리소스 계획** 그 지역으로 가는 겁니다
1. 를 활성화합니다 **비활성화 예약** 선택 사항입니다.

1. 표시되는 달력에서 날짜 및 시간을 지정합니다 **예약된 비활성화 날짜**.

   >[!NOTE]
   >
   >* 시간 상자에서는 분이 아니라 1시간 단위만 선택할 수 있습니다.
   >* 전달된 현재 날짜의 시간을 선택하는 경우 Workfront은 다음 날 오전 12:00에 비활성화 일정을 예약합니다. 선택한 시간은 비활성화를 예약하는 사용자의 컴퓨터 시간대와 일치합니다.


1. 클릭 **변경 내용 저장**.

   사용자는 선택한 날짜에 비활성화된 경우가 있습니다. 여러 사용자를 일괄 비활성화하도록 선택한 경우 선택한 모든 사용자가 선택한 날에 비활성화되는 경우가 있습니다.

비활성화하도록 예약한 사용자를 위한 보고서를 작성하여 비활성화될 사용자에 대한 정보를 유지하는 것이 좋습니다. 사용자가 비활성화되면 비활성화되었음을 확인할 수 없습니다.

## 사용자 다시 활성화

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **사용자** ![](assets/users-icon-in-main-menu.png).

1. 사용자를 선택하고 자세히 아이콘을 클릭합니다 ![](assets/more-icon.png)를 클릭한 다음 **활성화**.

1. 새 할당 **액세스 수준**&#x200B;를 클릭합니다.

### 사용자를 다시 활성화하면 제품 교정 영향

비활성화된 사용자는 할당된 기본 언어 교정 역할과 증명 라이센스를 잃게 됩니다(Workfront Premium 레거시 플랜을 사용하고 있는 경우). 사용자를 다시 활성화하도록 선택하는 경우 다음을 수행해야 합니다.

* 라이센스를 재할당합니다(Workfront Premium 이전 플랜을 사용하는 경우). Workfront 교정 계획에 대한 자세한 내용은 [Workfront에서 언어 교정 기능에 액세스](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* 올바른 증명 역할이 있는지 확인합니다. 재활성화된 증명 사용자에게는 새 사용자를 위한 기본 증명 역할로 지정되는 모든 것이 할당됩니다. 자세한 내용은 [기본 언어 교정 역할 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) 추가 정보.

## Workfront 관리자 및 Plan 라이선스 사용자 비활성화 정보

Workfront 관리자나 플랜 라이센스가 있는 사용자를 비활성화하려면 먼저 해당 사용자와 관련된 Workfront 개체 및 활동을 확인한 다음 필요에 따라 다른 Workfront 관리자 또는 계획 라이선스 사용자와 연결해야 합니다.

이러한 개체 및 활동에는 다음이 포함될 수 있습니다.

* 사용자에게 할당된 작업 또는 문제
* 사용자가 소유한 프로젝트
* 사용자가 액세스할 수 있도록 설정된 보고서
* 사용자가 소유한 템플릿
* 사용자가 리소스 관리자로 설정된 프로젝트 및 템플릿
* Workfront 관리자 또는 계획 라이선스 사용자가 기본 할당자인 요청 큐 라우팅 규칙
* 사용자를 포함하는 단계가 있는 승인 프로세스(특히 스테이지에서 유일한 승인자인 경우)
* 사용자를 승인자로 나열하는 작업표입니다
* 사용자를 승인자로 나열하는 작업표 프로필
* 사용자를 포함하는 자동화된 워크플로우 교정

## 리소스 계획은 사용자를 비활성화하도록 예약할 때 영향을 줍니다

비활성화하도록 사용자를 스케줄링할 때, 해당 사용자는 더 이상 자원 계획자에 예산 책정 시간에 사용할 수 있는 것으로 표시되지 않습니다. 자원 풀의 일부로 남아 있는 경우 자원 계획자에 표시되지만 해당 가용성은 스케줄링된 비활성화 날짜부터 0시간으로 설정됩니다.

자원 계획자는 사용자의 모든 작업 역할과 작업의 계획 완료 일자를 고려하여 그에 따라 자원을 계산합니다.

리소스 계획자에 대한 자세한 내용은 [리소스 플래너 개요](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
