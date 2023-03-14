---
product-area: reporting
navigation-topic: other-blocks
title: 보고 캔버스에서 웹 컨텐츠 블록을 추가하거나 편집합니다
description: 웹 컨텐츠 블록을 사용하면 보고서 내에서 직접 외부 웹 사이트의 정보를 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---


# 보고 캔버스에서 웹 컨텐츠 블록을 추가하거나 편집합니다

웹 컨텐츠 블록을 사용하면 보고서 내에서 직접 외부 웹 사이트의 정보를 표시할 수 있습니다.

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 베타: 개요](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 웹 콘텐츠 블록 추가 또는 편집

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고&#x200B;**보고**.
1. 클릭 **새 보고서**.

   또는

   기존 보고서로 이동하여 **자세히** 아이콘 ![](assets/more-icon-27x15.png) 보고서 헤더에서 **편집**.

1. 화면 오른쪽의 아래에서 **블록 추가**&#x200B;다음 중 하나를 수행합니다.

   을(를) 드래그합니다. **웹 컨텐츠** 아이콘을 캔버스에 드래그하여 원하는 위치에 직접 설정합니다.

   또는

   를 두 번 클릭합니다. **웹 컨텐츠** 캔버스 맨 위에 블록을 추가하는 아이콘

   >[!TIP]
   >
   >블록의 코너 핸들을 끌어 배치된 후 블록의 크기를 변경할 수 있습니다.

1. 클릭 **제목 없는 웹 콘텐츠** 블록 헤더에 블록의 제목을 입력합니다.
1. 을(를) 클릭합니다. **편집** 아이콘 ![](assets/edit-icon.png) ( 블록 헤더에서)를 참조하십시오.

   ![](assets/web-content-block-header-350x76.png)

1. 에서 **설정** 표시되는 패널에 표시할 페이지의 전체 URL(&quot;https://&quot; 포함)을 입력합니다 **URL** 필드.

   >[!NOTE]
   >
   >현재 선택한 도메인의 사이트만 표시할 수 있습니다. 현재 사용할 수 있는 도메인은 다음과 같습니다.
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com


   삽입할 수 없는 경우 입력한 URL 아래에 경고가 표시됩니다. 이러한 경고는 다음과 같습니다.

   | 경고 이름 | 이유 |
   |---|---|
   | 잘못된 URL | 입력한 URL이 올바른 사이트를 반환하지 않습니다. |
   | 공급자 사이트 제한 | 포함하려는 사이트는 허용되지 않습니다. |

   {style="table-layout:auto"}

1. (선택 사항) **매개 변수 전달** 사용 가능한 전달 매개 변수 목록을 열려면 를 전환합니다.

   >[!WARNING]
   >
   >현재 전달 매개 변수를 사용할 수 없습니다.

1. 클릭 **포함 URL** 선택 사항을 저장하고 보고서로 돌아가려면
