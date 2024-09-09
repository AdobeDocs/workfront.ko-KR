---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 업무 균형자에서 리소스를 관리하는 데 필요한 액세스
description: 올바른 액세스 또는 권한이 없으면 업무 균형자에서 작업 할당을 보거나 관리하지 못할 수 있습니다.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# 업무 균형자에서 리소스를 관리하는 데 필요한 액세스

올바른 액세스 또는 권한이 없으면 업무 균형자에서 작업 할당을 보거나 관리하지 못할 수 있습니다.

업무 균형자에서 보거나 관리할 업무 부하를 가진 사용자를 보려면 액세스 권한이 있어야 합니다. 이 외에도 작업과 연결된 프로젝트에 대해 올바른 액세스 수준과 올바른 권한이 있어야 합니다.

## Adobe Workfront에서는 영역별로 업무 균형자를 사용해야 합니다.

다음 표는 회사의 Workfront 계획과 업무 균형자를 사용할 수 있는 시스템 내 위치 간의 연결을 보여 줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront 플랜(현재)</b></p></td> 
   <td> <p><b>업무 균형자에 액세스할 수 있는 영역</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">팀 이상 </td> 
   <td>팀 또는 프로젝트의 업무 균형자</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro 이상</td> 
   <td>시스템 수준에서 여러 프로젝트에 대한 워크로드 밸런서</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p><b>Workfront 플랜(신규)</b></p></td> 
   <td> <p><b>업무 균형자에 액세스할 수 있는 영역</b></p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">임의 </td> 
   <td>Workfront의 어디에서든 업무 균형자에 액세스</td> 
  </tr> 
 </tbody> 
</table>

Workfront 플랜에 대한 자세한 내용은 [플랜](https://www.workfront.com/plans)을 참조하세요.

Workfront에서 업무 균형자를 찾을 수 있는 위치에 대한 자세한 내용은 [업무 균형자 찾기](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)를 참조하십시오.

## 업무 균형자 보기에 필요한 액세스

업무 균형자를 보려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 계획, 리소스 조달 영역에서 업무 균형자 보기;</br>
       팀 또는 프로젝트의 업무 균형자를 보려면 작업</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>리소스 관리에 대한 보기 이상의 액세스 권한</p> <p>리소스 관리 액세스 수준에 대한 자세한 내용은 문서 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">리소스 관리에 대한 액세스 권한 부여</a>를 참조하십시오.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>할당을 보려는 프로젝트에 대한 보기 권한이 있어야 합니다. </p> <p>프로젝트 권한에 대한 자세한 내용은 문서 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>를 참조하십시오.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 업무 균형자에서 할당을 관리하는 데 필요한 액세스

업무 균형자 를 관리하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 리소스 조달 영역의 업무 균형자에서 할당을 관리하도록 계획합니다.</br>
       팀 또는 프로젝트의 업무 균형자에서 할당을 관리하려면 작업</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>리소스 관리에 대한 액세스 편집</p> 
     <p>리소스 관리 액세스 수준에 대한 자세한 내용은 문서 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">리소스 관리에 대한 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 할당할 프로젝트에 대한 Contribute 이상의 권한으로, 할당에 대한 권한이 포함되어 있습니다. </p> <p>프로젝트 권한에 대한 자세한 내용은 문서 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>를 참조하십시오.</p></td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->