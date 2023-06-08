---
product-area: reporting
navigation-topic: other-blocks
title: 보고 캔버스에서 웹 콘텐츠 블록 추가 또는 편집
description: 웹 콘텐츠 블록을 사용하면 보고서 내에서 직접 외부 웹 사이트의 정보를 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: ca70952bf0acd71f748b042852d434b560727a83
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---


# 보고 캔버스에서 웹 콘텐츠 블록 추가 또는 편집

웹 콘텐츠 블록을 사용하면 보고서 내에서 직접 외부 웹 사이트의 정보를 표시할 수 있습니다.

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 Beta: 개요](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 웹 콘텐츠 블록 추가 또는 편집

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음&#x200B;**보고**.
1. 클릭 **새 보고서**.

   또는

   기존 보고서로 이동하여 **자세히** 아이콘 ![](assets/more-icon-27x15.png) 보고서 헤더에서 를 클릭하고 **편집**.

1. 화면 오른쪽의 **블록 추가**, 다음 중 하나를 수행합니다.

   드래그 **웹 콘텐츠** 아이콘을 캔버스에 올려 원하는 위치로 바로 이동합니다.

   또는

   를 두 번 클릭합니다. **웹 콘텐츠** 캔버스 맨 위에 블록을 추가하는 아이콘.

   >[!TIP]
   >
   >블록 모서리 핸들을 드래그하여 블록을 배치한 후 블록 크기를 변경할 수 있습니다.

1. 클릭 **제목 없는 웹 컨텐츠** 블록 헤더에 블록의 제목을 입력합니다.
1. 다음을 클릭합니다. **편집** 아이콘 ![](assets/edit-icon.png) 블록 헤더에서.

   ![](assets/web-content-block-header-350x76.png)

1. 다음에서 **설정** 열리는 패널에 표시할 페이지의 전체 URL(&quot;https://&quot; 포함)을 **URL** 필드.

   >[!NOTE]
   >
   >현재는 선택한 도메인의 사이트만 표시할 수 있습니다. 현재 사용할 수 있는 도메인은 다음과 같습니다.
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com


   포함할 수 없는 경우 입력한 URL 아래에 경고가 표시됩니다. 이러한 경고에는 다음이 포함됩니다.

   | 경고 이름 | 이유 |
   |---|---|
   | 잘못된 URL | 입력한 URL이 올바른 사이트를 반환하지 않습니다. |
   | 공급자 사이트 제한 사항 | 임베드하려는 사이트는 허용되지 않습니다. |

   {style="table-layout:auto"}

1. (선택 사항) **매개 변수 전달** 사용 가능한 패스 매개 변수 목록을 열려면 전환합니다.

   >[!WARNING]
   >
   >현재 전달 매개 변수가 비활성화되어 있습니다.

1. 클릭 **URL 포함** 선택 내용을 저장하고 보고서로 돌아갑니다.
