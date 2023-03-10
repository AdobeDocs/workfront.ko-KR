---
product-area: resource-management
navigation-topic: resource-pools
title: 리소스 풀에서 사용자 제거
description: 리소스 풀에 포함할 수 있는 사용자 수에 제한이 없지만 사용자 목록에는 처음 2000명의 사용자만 알파벳순으로 표시됩니다.
author: Alina
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# 리소스 풀에서 사용자 제거

리소스 풀에 포함할 수 있는 사용자 수에 제한이 없지만 사용자 목록에는 처음 2000명의 사용자만 알파벳순으로 표시됩니다.

비활성화되었거나 역할 또는 부서를 이동한 사용자를 제거하여 모든 리소스 풀에 항상 정확한 사용자 목록을 유지하는 것이 좋습니다.

리소스 풀에 대한 자세한 내용은 [리소스 풀 개요](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 풀 관리에 대한 액세스를 포함하는 리소스 관리에 대한 액세스 편집</p> <p>사용자에 대한 액세스 권한 보기 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 리소스 풀에서 사용자 제거

해당 사용자가 해당 풀에서 더 이상 필요하지 않으면 리소스 풀에서 사용자를 제거할 수 있습니다.

리소스 풀에서 사용자를 제거하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **리소스**.
1. 클릭 **리소스 풀** 왼쪽 패널에 표시됩니다.
1. 리소스 풀을 선택하고 **편집 을 클릭합니다.**또는\
   리소스 풀 이름을 클릭합니다.

1. 제거할 사용자 이름을 **이 리소스 풀에서 검색** 필드.\
   또는\
   해당 엔터티에 연결된 모든 사용자를 제거하려면 회사, 작업 역할, 팀 또는 그룹의 이름을 입력합니다.\
   ![search_inside_NEW_resource_pool.png](assets/search-inside-new-resource-pool-350x314.png)

1. 리소스 풀에서 사용자를 제거하려면 사용자 수준에서 &#39;x&#39; 아이콘을 클릭하십시오. 표시되는 모든 목록에서 제거됩니다.\
   또는\
   작업 역할, 그룹, 팀 또는 회사와 연관된 모든 사용자를 제거하려면 **제거** 작업 역할, 그룹, 팀 수준 또는 회사 수준에서 따라서 리소스 풀에서 해당 작업 역할, 그룹, 팀 또는 회사와 연관된 모든 사용자가 제거됩니다.

1. **저장**&#x200B;을 클릭합니다.
