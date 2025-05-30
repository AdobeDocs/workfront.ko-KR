---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 여러 열의 정보를 하나의 공유 열에 병합'
description: 여러 개별 열에 표시되는 정보를 병합하여 하나의 공유 열에 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 0%

---

# 보기: 여러 열의 정보를 하나의 공유 열에 병합

<!-- Audited: 11/2024 -->

여러 개별 열에 표시되는 정보를 병합하여 하나의 공유 열에 표시할 수 있습니다.

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
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p> 현재: 
   <ul>
   <li>보기 수정 요청</li> 
   <li>보고서 수정 계획</li>
   </ul>
     </p>
     <p> 신규: 
   <ul>
   <li>보기를 수정하는 기여자</li> 
   <li>보고서를 수정하는 표준</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 열을 공유하거나 병합할 때 고려 사항

* 두 개의 인접한 열을 병합하고 각 열의 정보를 줄 바꿈으로 구분하여 표시할 수도 있고, 각 열의 정보 사이에 구분 기호가 없는 두 개의 인접한 열에 정보를 병합할 수도 있습니다.
* 이 문서에 설명된 것과 동일한 구문을 이미 공유된 열과 인접한 열에 적용하여 두 개 이상의 열의 정보를 병합할 수 있습니다.
* `valueformat=HTML` 줄은 공유 열에서 필수입니다. 그렇지 않으면 Adobe Workfront에서 보고서를 내보낼 때 열에 정보가 포함되지 않습니다(비어 있음).
* 병합된 열에서는 조건부 서식이 지원되지 않을 수 있습니다.

  다음과 같은 예외가 있습니다.

   * Workfront에서 정보를 볼 때 병합된 열을 구성하는 열의 서식이 서로 다른 경우 첫 번째 열의 서식은 유지되고 다른 모든 열의 서식은 무시됩니다.
   * 보기를 PDF 파일로 내보낼 때 조건부 서식이 병합된 열의 첫 번째 열에 적용됩니다.
   * 뷰를 Excel 파일로 내보낼 때 병합된 열이 별도의 열로 표시됩니다. 개별 열에는 해당 조건부 서식 규칙도 표시됩니다.

* **viewalias** 특성이 있는 열은 병합할 수 있는 열의 양을 제한할 수 있습니다. 이러한 제한을 방지하려면 **viewalias** 특성을 사용하지 마십시오. 열에 **viewalias** 특성을 포함해야 하는 경우 해당 특성이 열에 나열된 마지막 항목인지 확인하십시오.

* 공유 열이 있는 목록을 Excel 또는 탭으로 구분된 형식으로 내보내면 내보낸 파일에서 해당 열이 구분됩니다.

* 하나 이상의 열에 `tile` 형식 필드가 표시되면 병합된 열에 강제 줄 바꿈이 자동으로 적용됩니다. 예를들어 서식 있는 텍스트 필드는 `tile`개의 형식 필드입니다. 이 경우 텍스트 모드에서 열을 볼 때 줄 코드가 `type=tile`입니다.

## 줄 바꿈 없이 두 열의 데이터 병합

서로 다른 여러 열의 데이터를 병합하여 각 열의 값 사이에 나누거나 공백이 없이 한 열에 표시할 수 있습니다.

>[!TIP]
>
>동일한 레코드에 대한 값을 동시에 표시할 수 없는 두 열을 병합하는 경우에는 이 방법을 사용하는 것이 좋습니다. 예를 들어 작업 항목 보고서에서 [문제 이름] 열과 [작업 이름] 열은 줄 바꿈 없이 병합될 수 있습니다. 작업 항목에는 [문제 이름]과 [작업 이름]이 동시에 포함될 수 없기 때문입니다. 작업 항목은 Workfront의 문제 또는 작업일 수 있습니다.

줄 바꿈 없이 두 열의 데이터를 병합하려면 다음을 수행합니다.

1. 개체 목록으로 이동합니다.
1. **보기** 드롭다운에서 보기를 선택한 다음 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭하여 보기를 편집합니다.
1. 병합할 첫 번째 열로 이동한 다음 **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. 병합할 첫 번째 열에 다음 텍스트를 추가합니다.

   `sharecol=true`

   Workfront 목록 또는 보고서의 처음 두 열을 병합할 때 첫 번째 열의 개체에 대한 정보가 포함된 텍스트 줄 앞에는 `column.0.`이(가) 있고 두 번째 열에 대한 정보가 포함된 텍스트 줄 앞에는 `column.1.`이(가) 있습니다.

   첫 번째 열의 열 번호 앞에 해당 열의 번호를 붙여야 합니다. 열 계산은 항상 `column.0.`(으)로 레이블이 지정된 목록 또는 보고서의 맨 왼쪽 열로 시작됩니다.

   두 개 이상의 열을 공유하는 경우 각 열에 대한 공유 정보가 들어 있는 코드 행에 열 번호를 추가해야 합니다.


   **예:** 다음은 목록의 두 번째 열부터 시작하여 세 개의 개별 열이 포함된 병합된 열의 텍스트 모드 코드입니다. 병합된 값은 프로젝트 이름, 계획된 시작 일자 및 프로젝트 소유자의 이름이며 세 값 사이에는 차이가 없습니다.

   ```
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.1.sharecol=true
   column.2.valuefield=plannedStartDate
   column.2.valueformat=atDate
   column.2.sharecol=true
   column.3.valuefield=owner:name
   column.3.valueformat=HTML
   ```

   ![줄 바꿈이 없는 공유 열](assets/shared-column-no-line-breaks-350x142.png)


1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.

## 줄 바꿈을 사용하여 두 열의 데이터 병합

여러 열의 데이터를 병합하여 각 열의 값 사이에 줄 바꿈을 사용하여 하나의 공통 열에 표시하려면 다음을 수행합니다.

1. 개체 목록으로 이동합니다.
1. **보기** 드롭다운에서 보기를 선택한 다음 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭하여 보기를 편집합니다.
1. 병합할 두 열 사이에 세 번째 열을 추가합니다.

   >[!TIP]
   >
   >* 병합할 열은 서로 인접해야 합니다.
   >* 병합할 첫 번째 열을 클릭해야 합니다.

1. **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭하고 1단계에서 추가한 가운데 열에 다음 코드를 추가합니다.

   ```
   value=<br>
   valueformat=HTML
   width=1
   sharecol=true
   ```

1. 첫 번째 열을 클릭하고 **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭한 다음 열에 다음 텍스트를 추가합니다.

   `sharecol=true`

   Workfront 목록 또는 보고서의 처음 두 열을 병합할 때 첫 번째 열의 개체에 대한 정보가 포함된 각 텍스트 줄 앞에 `column.0.`, 공유 정보가 포함된 열 뒤에 `column.1.`이(가) 있고 두 번째 열에 대한 정보가 포함된 텍스트 줄 앞에 `column.2.`이(가) 있습니다.

   결합된 열이 뷰의 중간에 있으면 뷰의 위치에 따라 열의 번호가 매겨집니다. 열 계산은 항상 `column.0.`(으)로 레이블이 지정된 목록 또는 보고서의 맨 왼쪽 열로 시작됩니다.

   두 개 이상의 열을 공유하는 경우 공유 정보가 들어 있는 코드 행에 열 번호를 추가해야 합니다.

   **예:** 다음은 프로젝트 이름, 계획된 시작 날짜 및 줄 바꿈이 있는 프로젝트 소유자 이름이 포함된 공유 열의 텍스트 모드 코드입니다. 공유 열은 프로젝트 보기의 두 번째 열입니다.

   ```
   column.1.displayname=Project_StartDate_Owner
   column.1.sharecol=true
   column.1.textmode=true
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.2.value=<br>
   column.2.width=1
   column.2.valueformat=HTML
   column.2.sharecol=true
   column.3.valuefield=plannedStartDate
   column.3.valueformat=atDate
   column.3.sharecol=true
   column.4.value=<br>
   column.4.width=1
   column.4.valueformat=HTML
   column.4.sharecol=true
   column.5.textmode=true
   column.5.valuefield=owner:name
   column.5.valueformat=HTML 
   ```

   ![줄 바꿈이 있는 공유 열](assets/shared-column-with-line-breaks-350x199.png)

1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.
