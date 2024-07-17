---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 프로젝트의 실제 시작 일자 개요
description: 프로젝트, 작업 및 문제의 Adobe Workfront 실제 시작 일자는 다음과 같습니다. 작업 및 문제의 경우 진행 중으로 표시된 날짜입니다. 프로젝트의 경우 프로젝트의 첫 번째 작업이 진행 중으로 표시되거나 완료된 날짜입니다.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# 프로젝트의 실제 시작 일자 개요

프로젝트, 작업 및 문제의 Adobe Workfront 실제 시작 일자는 다음과 같습니다. 작업 및 문제의 경우 진행 중으로 표시된 날짜입니다. 프로젝트의 경우 프로젝트의 첫 번째 작업이 진행 중으로 표시되거나 완료된 날짜입니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 보기 또는 상위 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 이상의 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## Workfront의 실제 시작 날짜에 대한 고려 사항

* 실제 시작 일자는 프로젝트, 작업 및 문제의 세부 정보 섹션에 있습니다. 
* 이러한 항목이 생성될 때 프로젝트, 작업 또는 문제의 실제 시작 날짜가 채워지지 않습니다.
* 실제 시작 일자는 작업이 프로젝트, 작업 또는 문제에서 실제로 시작될 때 채워집니다.
* 프로젝트에 대한 작업이 아직 시작되지 않은 경우 실제 시작 일자가 프로젝트 세부 정보 탭에 표시되지 않습니다.

  작업이 아직 시작되지 않은 경우 작업 및 문제 세부 정보 탭에 실제 시작 일자가 비어 있습니다.

* 작업 또는 문제의 실제 시작 일자는 수동으로 수정할 수 있지만, 프로젝트의 실제 시작 일자는 수정할 수 없습니다.

## 프로젝트의 실제 시작 날짜에 대한 고려 사항

* Workfront은 다음 중 하나가 발생하는 경우 프로젝트의 실제 날짜를 자동으로 설정합니다.

   * 작업 할당자가 작업 상태를 *새로 만들기*&#x200B;에서 *새로 만들기*&#x200B;와(과) 같지 않은 다른 상태로 변경합니다.

   * 작업 할당자는 작업의 완료율을 변경합니다.

     >[!IMPORTANT]
     >
     >프로젝트가 현재 (Current)로 표시된 경우 프로젝트 실제 시작 일자가 채워지지 않습니다. 프로젝트의 실제 시작 일자가 채워지기 전에 실제 작업이 프로젝트의 작업에서 시작해야 합니다.

     이러한 경우 프로젝트의 실제 시작 일자는 프로젝트의 가장 빠른 작업에 대해 이러한 작업이 발생한 일자 및 시간으로 설정됩니다. 이는 프로젝트가 실제로 이 날짜 및 시간에 시작되었음을 나타냅니다.

## 프로젝트의 실제 시작 일자 찾기

다음 영역에서 프로젝트의 실제 시작 일자를 찾을 수 있습니다.

* 프로젝트의 세부 정보 섹션에서 다음을 수행합니다.
* 프로젝트 보고서 또는 보기에서 보고서에 객체 프로젝트의 실제 시작 일자를 추가할 때.

  보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

프로젝트의 세부 정보 섹션에서 실제 시작 일자를 찾으려면 다음을 수행합니다.

1. Workfront의 오른쪽 상단에 있는 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **프로젝트**&#x200B;를 클릭합니다.
1. 실제 시작 일자를 보려는 프로젝트를 클릭합니다.
1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭한 다음 **개요** 섹션으로 이동합니다.

   실제 시작 일자 는 다른 프로젝트 일자 와 함께 표시됩니다.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
