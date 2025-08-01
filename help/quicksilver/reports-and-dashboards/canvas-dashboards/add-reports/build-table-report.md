---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 캔버스 대시보드에서 표 보고서 작성
description: 테이블 형식으로 데이터를 시각화하기 위해 캔버스 대시보드에 테이블 보고서를 추가할 수 있습니다.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 8b9676c7ef4efcad1294a9aa786aa6fe52d26cc0
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# 캔버스 대시보드에서 표 보고서 작성

>[!IMPORTANT]
>
>캔버스 대시보드 기능은 현재 베타 단계에 참여하는 사용자만 사용할 수 있습니다. 자세한 내용은 [캔버스 대시보드 베타 정보](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)를 참조하십시오.

테이블 형식으로 데이터를 시각화하기 위해 캔버스 대시보드에 테이블 보고서를 추가할 수 있습니다.

![테이블 보고서 예제](assets/table-example-main.png)

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td> 
   <td> 
<p>임의 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td> 
<p>현재: 플랜 </p> 
<p>새로운 기능: 표준</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td><p>보고서, 대시보드 및 캘린더에 대한 액세스 편집</p>
  </td> 
  </tr>  
</tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
+++

## 전제 조건

테이블 보고서를 작성하려면 먼저 대시보드를 만들어야 합니다.

## 캔버스 대시보드에서 표 보고서 작성

테이블 보고서를 작성하는 데 사용할 수 있는 구성 옵션은 여러 가지가 있습니다. 이 섹션에서는 하나를 만드는 일반적인 프로세스를 안내합니다.

{{step1-to-dashboards}}

1. 왼쪽 패널에서 **캔버스 대시보드**&#x200B;를 클릭합니다.

1. 오른쪽 상단의 **새 대시보드**&#x200B;를 클릭합니다.

1. **대시보드 만들기** 상자에 대시보드의 **이름** 및 **설명**&#x200B;을 입력하십시오.

1. Click **Create**.

1. **보고서 추가** 상자에서 **보고서 만들기**&#x200B;를 선택합니다.

1. 왼쪽에서 **테이블**&#x200B;을 선택합니다.

1. 오른쪽 상단 모서리에서 **보고서 만들기**&#x200B;를 클릭합니다.

1. (선택 사항) 아래 단계에 따라 **세부 정보** 섹션을 구성하십시오.

   1. 보고서 **이름**&#x200B;을(를) 입력하십시오.

   1. **설명** 보고서를 입력하십시오.

1. 아래 단계에 따라 **테이블 빌드** 섹션을 구성하십시오.

   1. 왼쪽 패널에서 **테이블 열** ![테이블 작성 아이콘](assets/drilldown-column.png) 아이콘을 클릭합니다.

   1. **열 추가**&#x200B;를 클릭한 다음 테이블에 열로 표시할 필드를 선택합니다. 오른쪽 미리보기 섹션에 열이 나타납니다.

   1. 추가할 각 열에 대해 위 단계를 반복합니다.

1. **필터** 섹션을 구성하려면 아래 단계를 따르십시오.

   1. 왼쪽 패널에서 **필터** ![필터 아이콘](assets/filter-icon.png) 아이콘을 클릭합니다.

   1. **필터 편집**&#x200B;을 선택합니다.

   1. **조건 추가**&#x200B;를 클릭한 다음 필터링할 필드와 필드가 충족해야 하는 조건 종류를 정의하는 수정자를 지정합니다. 오른쪽 미리보기 섹션에 열이 나타납니다.

1. (선택 사항) 다른 필터링 기준 집합을 추가하려면 **필터 그룹 추가**&#x200B;를 클릭합니다. 세트 사이의 기본 연산자는 AND입니다. 연산자를 클릭하여 OR로 변경합니다.

1. **드릴다운 그룹 설정** 섹션을 구성하려면 아래 단계를 따르십시오.

   1. 왼쪽 패널에서 **그룹 설정** ![그룹 설정 아이콘](assets/drilldown-group-icon.png) 아이콘을 클릭합니다.

   1. **그룹화 추가** 단추를 클릭한 다음 그룹화로 만들 필드를 선택합니다. 그룹화 열이 오른쪽의 미리보기 섹션에 나타납니다.

1. 보고서를 만들고 대시보드에 추가하려면 **저장**&#x200B;을 클릭하세요.