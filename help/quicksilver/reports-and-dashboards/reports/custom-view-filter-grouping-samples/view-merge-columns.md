---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 하나의 공유 열에 있는 여러 열의 정보 병합'
description: 여러 개의 개별 열에 표시되는 정보를 병합하여 하나의 공유 열에 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# 보기: 하나의 공유 열에 있는 여러 열의 정보 병합

여러 개의 개별 열에 표시되는 정보를 병합하여 하나의 공유 열에 표시할 수 있습니다.

## 액세스 요구 사항

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 열을 공유하거나 병합할 때의 고려 사항

* 인접한 두 열을 병합하고 각 열의 정보를 줄 바꿈으로 구분하거나, 각 열의 정보 간에 구분되지 않고 인접한 두 열의 정보를 병합할 수 있습니다.
* 이 문서에 설명된 것과 동일한 구문을 이미 공유된 열 및 인접 열에 적용하여 두 개 이상의 열의 정보를 병합할 수 있습니다.
* 해당

   ```
   valueformat=HTML
   ```

   공유 열에는 줄이 필수입니다. 그렇지 않으면 Adobe Workfront에서 보고서를 내보낼 때 열에 정보가 없습니다(비어 있음).
* 병합된 열에서 조건부 서식을 지원하지 않을 수 있습니다.

   다음과 같은 예외가 있습니다.

   * Workfront에서 정보를 볼 때 병합된 열을 구성하는 열의 서식이 서로 다른 경우 첫 번째 열의 서식이 유지되고 다른 모든 열에 대한 서식이 무시됩니다.
   * 보기를 PDF 파일로 내보낼 때 조건부 서식이 병합된 열의 첫 번째 열에 적용됩니다.
   * 보기를 Excel 파일로 내보낼 때 병합된 열이 별도의 열로 표시됩니다. 개별 열에는 해당 조건부 서식 규칙도 표시됩니다.

* 열을 **비에왈리아스** 특성은 병합할 수 있는 열의 양을 제한할 수 있습니다. 이러한 제한을 방지하려면 **비에왈리아스** 속성을 사용합니다. 를 포함해야 하는 경우 **비에왈리아스** 속성의 열 이름을 지정합니다. 열의 마지막 항목인지 확인합니다.

* 공유 열이 있는 목록을 Excel 또는 탭으로 구분된 형식으로 내보낼 경우 이러한 열은 내보낸 파일에서 분리됩니다.

## 줄바꿈 없이 두 열의 데이터 병합

데이터를 별도의 여러 열에서 병합하여 각 열의 값 간에 나누거나 공백이 없는 한 열에 표시할 수 있습니다.

>[!TIP]
>
>이 방법은 동일한 레코드에 대한 값을 동시에 표시할 수 없는 두 개의 열을 병합할 때 권장됩니다. 예를 들어, 작업 항목 보고서에서 작업 항목에는 동시에 문제 이름과 작업 이름이 있을 수 없으므로 작업 항목 간에 라인 브레이크 없이 문제 이름 및 작업 이름 열을 병합할 수 있습니다. 작업 항목은 Workfront의 문제 또는 작업일 수 있습니다.

방법은 다음과 같습니다.

1. 보기에 텍스트 모드를 사용하여 병합할 첫 번째 열에 다음 텍스트를 추가합니다.

   ```
   sharecol=true
   ```

   목록이나 보고서의 처음 두 열을 병합하면 Workfront이 첫 번째 열의 개체에 대한 정보를 포함하는 각 텍스트 줄 앞에

   ```
   column.0.
   ```

   및

   ```
   column.1.
   ```

   .\
   첫 번째 열의 열 번호 앞에 해당 열의 수가 있어야 합니다. 열 계산은 항상 목록 또는 보고서에서 맨 왼쪽 열로 시작됩니다

   ```
   column.0.
   ```

   .

   두 개 이상의 열을 공유하는 경우 각 열에 대한 공유 정보가 들어 있는 코드 행에 열 번호를 추가해야 합니다.

   **예:** 다음은 목록의 두 번째 열로 시작하는 세 개의 개별 열이 포함된 병합된 열에 대한 텍스트 모드 코드입니다. 병합된 값은 프로젝트 이름, 계획 시작 일자 및 프로젝트 소유자의 이름이며 세 값 사이에 나누기가 없습니다.

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.2.valuefield=plannedStartDate
   ```

   ```
   column.2.valueformat=atDate
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=owner:name
   ```

   ```
   column.3.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-no-line-breaks-350x142.png" style="width: 350;height: 142;"></pre>

1. 클릭 **저장**, 그런 다음 **보기 저장**.

## 두 열의 데이터를 줄바꿈으로 병합

여러 열의 데이터를 병합하여 각 열의 값 사이의 줄바꿈과 함께 하나의 공통 열에 표시합니다.

1. 병합할 두 열 사이에 세 번째 열을 추가합니다.

   >[!TIP]
   * 병합할 열이 서로 인접해야 합니다.
   * 병합할 첫 번째 열을 클릭해야 합니다.


1. 클릭 **텍스트 모드로 전환** 그리고 1단계에서 추가한 가운데 열에 다음 코드를 추가합니다.

   ```
   value=<br>
   ```

   ```
   valueformat=HTML
   ```

   ```
   width=1
   ```

   ```
   sharecol=true
   ```

1. 첫 번째 열에 다음 텍스트를 추가합니다.

   ```
   sharecol=true
   ```

   목록이나 보고서의 처음 두 열을 병합하면 Workfront이 첫 번째 열의 개체에 대한 정보를 포함하는 각 텍스트 줄 앞에

   ```
   column.0.
   ```

   , 공유 정보가 있는 열

   ```
   column.1.
   ```

   , 및

   ```
   column.2.
   ```

   . 결합된 열이 보기 중간에 있으면 보기의 위치에 따라 열에 번호가 지정됩니다. 열 계산은 항상 목록 또는 보고서에서 맨 왼쪽 열로 시작됩니다

   ```
   column.0.
   ```

   .

   두 개 이상의 열을 공유하는 경우 공유 정보가 포함된 코드 행에 열 번호를 추가해야 합니다.

   **예:** 다음은 프로젝트 이름, 계획된 시작 날짜 및 프로젝트 소유자의 이름이 줄바꿈으로 포함된 공유 열에 대한 텍스트 모드 코드입니다. 공유 열은 프로젝트 보기의 두 번째 열입니다.

   ```
   column.1.displayname=Project_StartDate_Owner
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.1.textmode=true
   ```

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.2.value=<br>
   ```

   ```
   column.2.width=1
   ```

   ```
   column.2.valueformat=HTML
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=plannedStartDate
   ```

   ```
   column.3.valueformat=atDate
   ```

   ```
   column.3.sharecol=true
   ```

   ```
   column.4.value=<br>
   ```

   ```
   column.4.width=1
   ```

   ```
   column.4.valueformat=HTML
   ```

   ```
   column.4.sharecol=true
   ```

   ```
   column.5.textmode=true
   ```

   ```
   column.5.valuefield=owner:name
   ```

   ```
   column.5.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-with-line-breaks-350x199.png" style="width: 350;height: 199;"></pre>

1. 클릭 **저장**, 그런 다음 **보기 저장**.
