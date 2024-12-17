---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 개인 작업'
description: 이 작업 필터는 사용자에게 전송된 임시 작업 요청이나 홈 영역에서 사용자가 추가한 할 일 항목을 반환합니다. 개인 작업은 프로젝트에 연결되지 않지만 필요한 경우 프로젝트로 이동할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 필터: 개인 작업

<!--Audited: 10/2024-->

이 작업 필터는 사용자에게 전송된 임시 작업 요청이나 사용자가 홈 영역의 할 일 위젯에서 추가한 할 일 항목을 반환합니다.

임시 작업 요청 및 할 일 항목은 개인 작업으로 Adobe Workfront에 저장됩니다.

개인 작업은 프로젝트에 연결되지 않지만 필요한 경우 프로젝트로 이동할 수 있습니다. 자세한 내용은 [개인 작업 만들기](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)를 참조하세요.

![](assets/personal-tasks-report.png)

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>필터를 수정하는 기여자 </p></li>
   <li><p>보고서를 수정하는 표준</p></li> </ul>

<p>현재:</p>
   <ul><li><p>필터 수정 요청 </p></li>
   <li><p>보고서 수정 계획</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 개인 작업 필터링

이 필터를 만들려면 다음 작업을 수행하십시오.

1. 작업 목록 또는 작업 보고서로 이동합니다.
1. **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 클릭합니다.
1. (조건부) 보고서에서 필터에 액세스하고 있는 **필터 규칙 추가**&#x200B;를 클릭하거나 목록에서 필터에 액세스하는 경우 첫 번째 필드에서 필터 기준을 선택하기 시작합니다.
1. (조건부) 다음 필터링 기준을 선택합니다.

   * 목록 필터에서: **작업** > **개인** **참**
   * 보고서 필터에서: **작업** > **개인** > **같음(대/소문자 구분)** > **참**.
1. 필터를 저장합니다.

   목록에 프로젝트에 없는 개인 작업만 표시됩니다.
