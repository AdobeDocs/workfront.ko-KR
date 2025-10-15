---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 그룹 상태 순서 바꾸기
description: 그룹 관리자는 관리하는 그룹의 프로젝트, 작업 및 문제 상태를 변경할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 7%

---

# 그룹 상태 순서 바꾸기

그룹 관리자는 관리하는 그룹의 프로젝트, 작업 및 문제 상태를 변경할 수 있습니다.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![상태](assets/statuses.png)

관리하는 그룹 위에 그룹이 있는 경우 해당 관리자는 해당 그룹에 대해 이 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

>[!NOTE]
>
>* Workfront 관리자는 시스템 수준에서 상태를 재정렬할 수 있습니다. 그룹 내 상태 순서에는 영향을 주지 않습니다.
>
>  그러나 새로 생성된 최상위 그룹 내의 상태는 시스템 레벨 상태의 순서를 상속합니다. (새 하위 그룹은 한 수준 위로 그룹내 상태의 순서를 상속합니다.)
>
>* 잠긴 상태의 순서를 변경할 수 있습니다. 잠긴 상태에 대한 자세한 내용은 [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)을 참조하세요.

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
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
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
     <p>현재</p> 
     <p>중단</p> 
     <p> 보류 중 </p> 
     <p> 계획 수립 </p> 
     <p> 완료 </p> 
     <p> 요청됨 </p> 
     <p> 승인됨 </p> 
     <p> 거부됨 </p> 
     <p> 아이디어 </p> 
   </td> 
   <td> 
     <p>신규</p> 
     <p>진행 중</p> 
     <p>완료</p> 
   </td> 
   <td> 
     <p>신규</p> 
     <p>진행 중</p> 
     <p>다시 열림</p> 
     <p>대기 중인 피드백</p> 
     <p>보류 중</p> 
     <p>복제 불가</p> 
     <p>마감됨</p> 
     <p>해결됨</p> 
     <p>확인 완료</p> 
     <p>해결되지 않음</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## 관리하는 그룹의 작업 및 프로젝트에 대한 상태 순서 바꾸기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**&#x200B;을 클릭한 다음 그룹 이름을 클릭합니다.
1. 왼쪽 패널에서 **상태**&#x200B;를 클릭합니다.
1. 표시되는 상태 목록 위에서 **프로젝트** 또는 **작업** 탭을 클릭합니다.

1. 원하는 순서대로 상태를 끌어다 놓습니다.

   새 상태 순서는 자동으로 저장됩니다.

1. 새 상태 순서를 테스트하려면 그룹과 연결된 작업 또는 프로젝트로 이동하여 오른쪽 상단의 상태를 클릭하고 구성된 순서대로 표시되는 상태를 확인합니다.

## 문제에 대한 상태 재정렬

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**&#x200B;을 클릭한 다음 그룹 이름을 클릭합니다.
1. 왼쪽 패널에서 **상태**&#x200B;를 클릭합니다.
1. **문제** 탭을 클릭합니다.
1. (선택 사항) 문제 유형(**버그 보고서**, **순서 변경**, **문제** 또는 **요청**)을 선택합니다.

   >[!NOTE]
   >
   >* 기본 목록에 대한 상태 순서를 사용자 정의할 수 없습니다.
   >* 각 문제에 대한 상태의 순서를 동일한 방식으로 지정하는 것이 좋습니다. 문제 유형에 대한 자세한 내용은 [요청 유형 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)을 참조하십시오.

1. 원하는 순서대로 상태를 끌어다 놓습니다.

   새 상태 순서는 자동으로 저장됩니다.

1. 새 상태 순서를 테스트하려면 그룹과 관련된 문제로 이동하여 오른쪽 상단의 상태를 클릭한 다음, 표시되는 상태가 구성한 순서대로 표시되는지 확인합니다.
