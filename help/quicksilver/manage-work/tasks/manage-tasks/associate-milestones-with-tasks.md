---
product-area: projects
navigation-topic: manage-tasks
title: 작업과 이정표 연결
description: 프로젝트 라이프타임에서 중요한 단계에 도달하는 시기를 나타내는 이정표를 작업에 연결할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 작업과 이정표 연결

프로젝트 라이프타임에서 중요한 단계에 도달하는 시기를 나타내는 이정표를 작업에 연결할 수 있습니다.

## 액세스 요구 사항

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
  <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

이정표를 작업에 연결하려면 먼저 다음 항목이 있어야 합니다.

* Workfront 관리자는 [이정표 경로 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* 이정표 경로를 프로젝트와 연결하려면 프로젝트가 계획 또는 현재 상태여야 합니다.

>[!TIP]
>
>이정표 보기를 사용하여 프로젝트에서 이정표 진행 상황을 최상으로 보려면 상위 작업을 만들고 프로젝트의 각 주요 단계에 연결해야 합니다. 그런 다음 이러한 상위 작업을 이정표 경로의 각 이정표에 연결합니다.

## 이정표를 작업과 연결

1. 프로젝트로 이동한 다음 **자세히** 아이콘 ![](assets/more-icon.png), 그런 다음 **편집**.
1. 사용 **설정** 섹션에서 프로젝트에 사용할 이정표 경로를 설정합니다.
1. **저장**&#x200B;을 클릭합니다.

   이정표 경로가 프로젝트와 연결되면 작업에 이정표를 지정할 수 있습니다.

1. 작업으로 이동한 다음 **자세히** 아이콘 ![](assets/more-icon.png), 그런 다음 **편집**.

   작업 및 이정표는 1:1 관계를 갖습니다. 동일한 이정표를 여러 작업에 첨부할 수 없습니다. 각 작업을 하나의 이정표에 연결하거나 각 이정표를 하나의 작업에 매핑할 수 있습니다.

1. 클릭 **설정**&#x200B;를 입력한 다음 **이정표** 작업의 필드입니다.
1. 클릭 **저장**.
1. (선택 사항) 작업 목록에서 **상태 아이콘** 열을 사용하여 이정표가 있는 작업을 식별합니다.

   ![](assets/amwt3.png)

1. (선택 사항) 프로젝트 목록에서 **이정표** 이정표 작업의 진행 상황을 확인할 수 있습니다.

   ![Screen_Shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)
