---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 작업 로드 밸런서에서 리소스를 관리하는 데 필요한 액세스
description: 올바른 액세스 또는 권한이 없으면 작업 로드 밸런서에서 작업 할당을 보거나 관리할 수 없습니다.
author: Alina
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# 작업 로드 밸런서에서 리소스를 관리하는 데 필요한 액세스

올바른 액세스 또는 권한이 없으면 작업 로드 밸런서에서 작업 할당을 보거나 관리할 수 없습니다.

작업 로드 밸런서에서 작업 로드를 보거나 관리할 사용자를 볼 수 있는 액세스 권한이 있어야 합니다. 이 외에도 작업이 연결된 프로젝트에 대한 올바른 액세스 수준과 올바른 권한이 있어야 합니다.

## Adobe Workfront 계획은 다양한 영역에 대해 작업 로드 밸런서를 사용하는 데 필요합니다.

다음 표에서는 회사가 보유한 Workfront 계획과 시스템에서 작업 로드 밸런서를 사용할 수 있는 위치 간의 연결을 보여 줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Workfront 플랜</p></td> 
   <td> <p>작업 로드 밸런서에 액세스할 수 있는 영역</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">팀 이상 </td> 
   <td>팀 또는 프로젝트에 대한 작업 로드 밸런서</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro 이상</td> 
   <td>시스템 수준에서 여러 프로젝트에 대한 작업 로드 밸런서</td> 
  </tr> 
 </tbody> 
</table>

Workfront 계획에 대한 자세한 내용은 [Adobe의 계획](https://www.workfront.com/plans).

Workfront에서 작업 로드 밸런서를 찾을 수 있는 위치에 대한 자세한 내용은 [작업 로드 밸런서를 찾습니다.](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## 작업 로드 밸런서를 보는 데 필요한 액세스

작업 로드 밸런서를 보려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>리소스 영역에서 작업 로드 밸런서를 볼 계획</p>
   <p>팀 또는 프로젝트의 작업 로드 밸런서를 보는 작업</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 관리에 대한 액세스 보기 이상</p> <p>리소스 관리 액세스 수준에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">리소스 관리에 대한 액세스 권한 부여</a>.</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>지정을 보려는 프로젝트에 대한 보기 권한이 있습니다. </p> <p>프로젝트 권한에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 로드 밸런서에서 할당을 관리하는 데 필요한 액세스

작업 로드 밸런서를 관리하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>자원 관리 영역의 작업 로드 밸런서에서 지정을 관리할 계획</p>
   <p>팀 또는 프로젝트의 작업 로드 밸런서에서 지정을 관리하는 작업</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 관리에 대한 액세스 편집</p> 
     <p>리소스 관리 액세스 수준에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">리소스 관리에 대한 액세스 권한 부여</a>.</p>
     <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 할당에 지정할 권한이 포함된 할당을 관리할 프로젝트에 대한 Contribute 또는 이상의 권한을 부여합니다. </p> <p>프로젝트 권한에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->