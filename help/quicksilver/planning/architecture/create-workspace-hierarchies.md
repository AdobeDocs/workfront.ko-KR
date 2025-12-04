---
title: Workspace 계층 만들기
description: 작업 영역 관리자는 Adobe Workfront Planning의 레코드 유형 간에 여러 작업 영역 계층을 생성할 수 있습니다. 작업 영역에서 레코드 유형을 연결하고 계층을 만들면 레코드 유형이 서로 연결되며, 한 레코드 유형이 상위로 지정되고 최대 6개의 다른 레코드 유형이 하위로 구성됩니다.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: ff9371b639e7684a94c08b8cd6293b632fac9edf
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# 작업 영역 계층 만들기

작업 영역 관리자는 Adobe Workfront Planning의 레코드 유형 간에 여러 작업 영역 계층을 생성할 수 있습니다.

작업 영역에서 레코드 유형을 연결하고 계층을 만들면 레코드 유형이 서로 연결되며, 한 레코드 유형이 상위로 지정되고 최대 6개의 다른 레코드 유형이 하위로 구성됩니다. <!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

계층은 헤더에 표시되는 레코드 종류 및 레코드 <!--ensure this is the case: does the breadcrumb show for both the RT and the record??-->에 대한 이동 경로를 생성합니다. 이렇게 하면 사용자는 워크플로의 모든 단계에서 계층 구조에서 자신의 위치를 알 수 있습니다.

계층 및 이동 경로에 대한 일반적인 정보는 [계층 및 이동 경로 개요](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)를 참조하십시오.


## 액세스 요구 사항

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ 을 확장하여 액세스 요구 사항을 보고 이 문서의 단계를 수행하십시오.  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul> 
<li><p>모든 Workfront 및 모든 Planning 패키지</p></li>
또는
<li><p>모든 워크플로우 및 모든 Planning 패키지</p></li></ul>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 공간에 대한 권한 관리</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 공간 계층 만들기
