---
title: 레코드 유형 비즈니스 규칙 구성
description: Adobe Workfront Planning에서 해당 유형의 레코드를 관리하는 방법을 정의하는 레코드 유형 비즈니스 규칙을 구성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 159b845c7b755117197d18f8474c01d4b19d53b8
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 4%

---


# 레코드 유형 비즈니스 규칙 구성

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Adobe Workfront Planning에서 해당 유형의 레코드를 관리하는 방법을 정의하는 레코드 유형 비즈니스 규칙을 구성할 수 있습니다.

## 액세스 요구 사항

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
<li><p>Planning 패키지가 있는 모든 Workfront 또는 워크플로우</p></li>
또는
<li><p>독립 실행형 제품으로 구입할 경우 모든 Planning 패키지</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>워크플로우 표준</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning 라이선스</p></td> 
   <td><p>계획 수립 표준</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가해야 합니다.</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 공간 및 레코드 유형에 대한 권한 관리</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 비즈니스 규칙 구성 시 고려 사항

* 레코드를 편집하거나 삭제할 수 있는 시기에 대한 규칙을 구성할 수 있습니다.
* 레코드가 생성되는 시기에 대한 규칙을 구성할 수 없습니다. 레코드 유형에 대한 관리 권한이 있는 모든 사용자는 레코드를 만들 수 있습니다.
* 다음을 제외한 모든 필드 유형을 참조하는 비즈니스 규칙에 대한 조건을 만들 수 있습니다.
  * 공식 필드
  * 조회 필드
  * 참조 필드

## 비즈니스 규칙 구성

1. 레코드 유형으로 이동합니다.
1. 레코드 종류 이름의 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 비즈니스 규칙을 클릭합니다.



