---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 시스템 수준 및 그룹 상태 순서 바꾸기
description: Workfront 관리자는 시스템의 모든 사용자 또는 단일 그룹에 대해 프로젝트, 작업 및 문제 상태의 순서를 변경할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 7%

---

# 시스템 수준 및 그룹 상태 순서 바꾸기

Workfront 관리자는 시스템의 모든 사용자 또는 단일 그룹에 대해 프로젝트, 작업 및 문제 상태의 순서를 변경할 수 있습니다.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![상태](assets/statuses.png)

>[!NOTE]
>
>* 시스템 레벨에서 상태를 재정렬해도 그룹 내 상태 순서에 영향을 주지 않습니다.
>
>  그러나 새로 생성된 최상위 그룹 내의 상태는 시스템 레벨 상태의 순서를 상속합니다. (새 하위 그룹은 한 수준 위로 그룹내 상태의 순서를 상속합니다.)
>
>* 잠긴 상태의 순서를 변경할 수 있습니다. 잠긴 상태에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)을 참조하세요.
>* 그룹 관리자는 그룹에서 사용되는 상태를 재정렬할 수도 있습니다. 자세한 내용은 [그룹 상태 순서 바꾸기](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md)를 참조하십시오.
>

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>시스템 관리자</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기본 상태 순서

기본적으로 상태는 다음 순서로 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">프로젝트</th> 
   <th width="33.33%">작업</th> 
   <th width="33.33%">문제</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>현재</li> 
     <li>중단</li> 
     <li> 보류 중 </li> 
     <li> 계획 수립 </li> 
     <li> 완료 </li> 
     <li> 요청됨 </li> 
     <li> 승인됨 </li> 
     <li> 거부됨 </li> 
     <li> 아이디어 </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>신규</li> 
     <li>진행 중</li> 
     <li>완료</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>신규</li> 
     <li>진행 중</li> 
     <li>다시 열림</li> 
     <li>대기 중인 피드백</li> 
     <li>보류 중</li> 
     <li>복제 불가</li> 
     <li>마감됨</li> 
     <li>해결됨</li> 
     <li>확인 완료</li> 
     <li>해결되지 않음</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 작업 및 프로젝트의 시스템 전체 또는 그룹 상태 재정렬

{{step-1-to-setup}}

1. 왼쪽 패널에서 **프로젝트 환경 설정 > 상태**&#x200B;를 클릭합니다.
1. (조건부) 그룹에 대한 상태를 재정렬하는 경우 오른쪽 상단 모서리의 상자에 그룹 이름을 입력한 다음 표시될 때 이름을 클릭합니다.

   ![시스템 상태](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. 표시되는 상태 목록 위에서 **프로젝트** 또는 **작업** 탭을 클릭합니다.

1. 원하는 순서대로 상태를 끌어다 놓습니다.

   새 상태 순서는 자동으로 저장됩니다.

1. 새 상태 순서를 테스트하려면 작업 또는 프로젝트로 이동하여 오른쪽 상단 모서리의 상태를 클릭하고 구성된 순서대로 상태가 표시되는지 확인합니다.

## 문제에 대한 상태 재정렬

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **설정** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.

1. **프로젝트 환경 설정 > 상태를 클릭합니다.**
1. (조건부) 그룹에 대한 상태를 재정렬하는 경우 오른쪽 상단 모서리의 상자에 그룹 이름을 입력한 다음 표시될 때 이름을 클릭합니다.

   ![그룹에 대한 문제 상태](assets/issue-statuses-group-name.png)

1. **문제** 탭을 클릭합니다.
1. (선택 사항) 문제 유형(**버그 보고서**, **순서 변경**, **문제** 또는 **요청**)을 선택합니다.

   >[!NOTE]
   >
   >* 기본 목록에 대한 상태 순서를 사용자 정의할 수 없습니다.
   >* 각 문제에 대한 상태의 순서를 동일한 방식으로 지정하는 것이 좋습니다. 문제 유형에 대한 자세한 내용은 [요청 유형 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)을 참조하십시오.

1. 원하는 순서대로 상태를 끌어다 놓습니다.

   새 상태 순서는 자동으로 저장됩니다.

1. 새 상태 순서를 테스트하려면 문제로 이동하여 오른쪽 상단 모서리의 상태를 클릭한 다음, 표시되는 상태가 구성한 순서대로 표시되는지 확인하십시오.
