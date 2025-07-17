---
title: 필터, 보기 및 그룹화에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 목록 및 보고서에 대한 필터, 보기 및 그룹화 컨트롤에 대한 사용자 액세스 권한을 정의할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 1%

---

# 필터, 보기 및 그룹화에 대한 액세스 권한 부여

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 액세스 수준을 사용하여 목록 및 보고서에 대한 필터, 보기 및 그룹화 컨트롤에 대한 사용자 액세스 권한을 정의할 수 있습니다.

필터, 보기 및 그룹화 컨트롤에 대한 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 사용자 정의 액세스 수준을 사용하여 필터, 보기 및 그룹화에 대한 사용자 액세스 구성

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 필터 오른쪽의 ![](assets/gear-icon-settings.png)보기&#x200B;**또는**&#x200B;편집&#x200B;**단추에서 톱니바퀴 아이콘**&#x200B;을(를) 클릭한 다음 **설정을 미세 조정**&#x200B;에서 부여할 기능을 선택합니다.

   ![](assets/gear-icon-filters-dashboards-groupings.png)

   기본적으로 플랜, 작업, 검토자 또는 요청 라이선스가 있는 사용자는 전체 보기 및 편집 권한이 있습니다. 외부 사용자 라이선스가 있는 사용자는 필터, 보기 및 그룹화에 액세스할 수 없습니다.

   <!--If this changes, undraft section with table below
   -->

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나를 계속 사용하십시오(예: [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)).
1. 완료되면 **저장**&#x200B;을 클릭하세요.

   액세스 수준이 만들어지면 사용자에게 이를 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

이 표에는 Workfront 관리자가 각 라이선스 유형을 가진 사용자가 필터, 보기 및 그룹화를 수행하도록 할 수 있는 사항이 나와 있습니다. Workfront 라이선스 유형에 대한 자세한 내용은 [Adobe Workfront 라이선스 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)를 참조하십시오.

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> 액션 </th>
<th> 플래너 </th>
<th> 보조 </th>
<th> 검토자 </th>
<th> 요청자 </th>
</tr>
</thead>
<tbody>
<tr>
<td>필터, 보기 및 그룹화 편집</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>필터, 보기 및 그룹화 만들기</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>필터, 보기 및 그룹화 보기</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>필터, 보기 및 그룹화 삭제</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>필터, 보기 및 그룹화 공유</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>필터, 보기 및 그룹화를 시스템 전체에서 공유</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>
