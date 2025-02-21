---
product-area: reporting
keywords: 변경,소유자,공유,보고서,공유,실행,사용자,액세스,권한,입력됨,마지막,조회함,날짜,보고,활동
navigation-topic: report-usage
title: 보고 활동에 대한 보고서 만들기
description: 보고서에 대한 보고서를 만들 때 비활성화된 사용자에게 보고서가 할당된 경우, 비활성화된 사용자의 액세스 권한으로 보고서가 실행되도록 설정된 경우, 사용자가 삭제하려는 보고서에 액세스하는 경우 등을 포함하는 특정 보고서 정보를 식별할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# 보고 활동에 대한 보고서 만들기

보고서에 대한 보고서를 만들 때 비활성화된 사용자에게 보고서가 할당된 경우, 비활성화된 사용자의 액세스 권한으로 보고서가 실행되도록 설정된 경우, 사용자가 삭제하려는 보고서에 액세스하는 경우 등을 포함하는 특정 보고서 정보를 식별할 수 있습니다.

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 기존 보고서에 대한 보고서 만들기 {#create-the-report-about-existing-reports}

1. Adobe Workfront 오른쪽 위 모서리에 있는 **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭합니다.
1. **보고서**&#x200B;를 클릭한 다음 **새 보고서**&#x200B;를 클릭합니다.
1. **새 보고서** 드롭다운 메뉴에서 **보고서**&#x200B;을(를) 선택하여 기존 보고서에 대한 보고서를 만듭니다.

1. **열(보기)** 탭에서 보고서에 원하는 열을 추가합니다.\
   다음 필드 중 일부가 유용할 수 있습니다.

   | 필드 | 설명 |
   |---|---|
   | **사용자로 실행: 이름** | 보고서의 **액세스 권한** 필드에서 이 보고서 실행에 지정된 사용자입니다. 이 사용자가 비활성화되면 보고서가 공유된 모든 사용자에 대해 보고서가 표시되지 않습니다. |
   | **다음 사용자와 공유** | 보고서가 공유되는 모든 엔티티입니다. |
   | **입력한 사람** | 이 사람이 보고서 소유자입니다. |
   | **마지막으로 본 날짜** | 사용자가 보고서를 마지막으로 본 날짜 및 시간입니다. |

   {style="table-layout:auto"}

1. (선택 사항) 비활성화된 특정 사용자로 보고서 목록을 제한하려면 다음을 수행하십시오.

   1. **필터** 탭을 선택한 다음 **필터 규칙 추가**&#x200B;를 클릭합니다.

   1. **사용자 ID로 실행** > **같음** 필터를 추가합니다.

   1. 필터에 추가할 비활성화된 사용자의 이름을 입력한 다음 목록에 표시될 때 이름을 클릭합니다.
   1. 보고서에 포함할 모든 비활성화된 사용자를 선택할 때까지 C단계를 반복합니다.

1. (선택 사항) 보고서 목록을 예약된 보고서로 제한하려면 다음을 수행합니다.

   1. **필터** 탭을 선택한 다음 **필터 규칙 추가**&#x200B;를 클릭합니다.

   1. 필터 **예약된 보고서 ID** > **비어 있지 않음**&#x200B;을(를) 추가합니다.

1. **저장 + 닫기**&#x200B;를 클릭한 다음 보고서 이름을 입력하고 **보고서 저장**&#x200B;을 클릭합니다.

   보고서 정보가 표시됩니다.

1. (선택 사항) 이 보고서를 Excel로 내보내고 컴퓨터에 저장합니다.\
   보고서 내보내기에 대한 자세한 내용은 [데이터 내보내기](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)를 참조하십시오.

## 보고서에 대한 정보 업데이트

보고서를 만든 후 필요에 따라 보고서를 업데이트할 수 있습니다.

1. 업데이트할 보고서로 이동합니다.
1. 수행할 작업에 따라 다음 중 하나를 수행합니다.

   * **다음 액세스 권한으로 이 보고서 실행:** 필드를 활성 사용자로 업데이트: 자세한 내용은 [다른 사용자의 액세스 권한으로 보고서 실행 및 전달](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)을 참조하십시오.

   * 보고서 복사본 만들기: 자세한 내용은 [보고서 복사본 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)를 참조하세요.
   * 보고서 삭제: 자세한 내용은 문서 [보고서 복사본 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)의 [정확한 보고서 복사본 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) 섹션을 참조하십시오.

   * 보고서 공유: 자세한 내용은 [Adobe Workfront에서 보고서 공유](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)를 참조하십시오.

1. (조건부) 원본 보고서를 복사하는 경우 [기존 보고서에 대한 보고서 만들기](#create-the-report-about-existing-reports)에서 만든 보고서의 정보를 사용하여 원본 보고서와 동일한 엔터티로 새 복사본을 공유합니다.
