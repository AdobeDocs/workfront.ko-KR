---
title: 개체에 대한 재무 권한 공유
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 액세스 수준을 할당할 때 재무 데이터를 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 자세한 내용은 재무 데이터에 대한 액세스 권한 부여를 참조하십시오.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 7%

---

# 개체에 대한 재무 권한 공유

Adobe Workfront 관리자는 액세스 수준을 할당할 때 재무 데이터를 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

사용자에게 부여된 액세스 수준과 함께 공유할 액세스 권한이 있는 특정 프로젝트, 작업 또는 문제에 대한 재무 보기 또는 관리 권한을 부여할 수도 있습니다.

각 액세스 수준의 사용자가 재무 데이터로 수행할 수 있는 작업에 대한 자세한 내용은 문서 [각 개체 유형에 사용할 수 있는 기능](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia)의 [재무 데이터](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md) 섹션을 참조하십시오.

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p> 
   <p>플랜</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트, 작업, 문제 및 재무 데이터 보기 또는 상위 액세스</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>적어도 재무 보기 권한이 포함된 프로젝트, 작업 및 문제에 대한 권한 이상 보기</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 개체 공유 및 재무 권한 부여

객체에 재무 권한을 부여할 때 다음 사항을 고려하십시오.

* 프로젝트, 작업 및 문제에 대한 재무 권한을 부여할 수 있습니다.
* 권한은 상속될 수 있습니다. 프로젝트에 대한 재무 보기 권한이 있는 경우 프로젝트의 작업 및 문제에 대한 재무 보기 권한을 자동으로 상속합니다.

객체에 재무 권한을 부여하려면 다음을 수행합니다.

1. 다른 사용자와 공유할 작업, 프로젝트 또는 문제로 이동합니다.
1. 개체 이름 근처에서 기타 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **공유**&#x200B;를 클릭합니다.

1. **액세스 권한 `<Object name>` 부여** 필드에서 개체를 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력하세요.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 객체를 공유할 수 있습니다.

1. 선택한 이름의 오른쪽에 드롭다운 메뉴가 나타나면 다음 옵션 중 하나를 클릭합니다.

   * **보기**
   * **참여**
   * **관리**

1. 같은 드롭다운 메뉴에서 **고급 설정**&#x200B;을 클릭한 후 다음 중 하나를 수행합니다.

   * 이전 단계에서 세 가지 옵션 중 하나를 선택한 경우 **재무 보기**&#x200B;가 선택되어 있는지 확인하십시오.
   * 이전 단계에서 **재무 관리**&#x200B;를 선택한 경우 **재무 관리**&#x200B;를 선택해야 합니다.

1. **저장**&#x200B;을 클릭합니다.

## 모든 공유 수준에 대한 재무 권한

다음 표에는 객체에 대한 보기, 기여 또는 관리 권한을 부여할 때 사용자에게 부여되는 재무 권한이 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>액션</strong> </th> 
   <th><strong>관리</strong> </th> 
   <th><strong>참여</strong> </th> 
   <th><strong>보기</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>청구 기록 관리</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>역할 청구 및 비용 요금 관리/보기</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>사용자 청구 및 비용 요금 관리/보기</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>재무 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>자원 계획 도구에서 원가별 정보 조회</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>리소스 계획 도구의 예산 리소스*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>자원 계획 도구에서 자원 조회*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;추가 리소스 관리 액세스 권한이 필요합니다.

리소스 관리 액세스에 대한 자세한 내용은 [리소스 관리에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)를 참조하십시오.
