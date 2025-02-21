---
title: 보고 캔버스에서 웹 콘텐츠 블록 추가 또는 편집
description: 웹 콘텐츠 블록을 사용하면 보고서 내에서 직접 외부 웹 사이트의 정보를 표시할 수 있습니다.
hidefromtoc: true
hide: true
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 1%

---

# 보고 캔버스에서 웹 콘텐츠 블록 추가 또는 편집

웹 콘텐츠 블록을 사용하면 보고서 내에서 직접 외부 웹 사이트의 정보를 표시할 수 있습니다.

## 전제 조건

시작하기 전에 보고 캔버스 베타에 등록해야 합니다. 자세한 내용은 [보고 캔버스 베타: 개요](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md)를 참조하십시오.

## 웹 콘텐츠 블록 추가 또는 편집

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![기본 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **보고**&#x200B;를 클릭합니다.
1. **새 보고서**&#x200B;를 클릭합니다.

   또는

   기존 보고서로 이동하여 보고서 머리글에서 **자세히** 아이콘 ![자세히 아이콘](assets/more-icon-27x15.png)을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

1. 화면 오른쪽의 **블록 추가**&#x200B;에서 다음 중 하나를 수행합니다.

   **웹 콘텐츠** 아이콘을 캔버스로 원하는 위치로 바로 끌어 놓으십시오.

   또는

   **웹 콘텐츠** 아이콘을 두 번 클릭하여 캔버스 맨 위에 블록을 추가합니다.

   >[!TIP]
   >
   >블록 모서리 핸들을 드래그하여 블록을 배치한 후 블록 크기를 변경할 수 있습니다.

1. 블록 헤더에서 **제목 없는 웹 콘텐츠**&#x200B;를 클릭한 다음 블록의 제목을 입력합니다.
1. 블록 헤더에서 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

   ![블록 헤더의 편집 아이콘](assets/web-content-block-header-350x76.png)

1. 열리는 **설정** 패널에서 **URL** 필드에 표시할 페이지의 전체 URL(&quot;https://&quot; 포함)을 입력합니다.

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

1. (선택 사항) **매개 변수 전달** 토글을 클릭하여 사용 가능한 매개 변수 전달 목록을 엽니다.

   >[!WARNING]
   >
   >현재 전달 매개 변수가 비활성화되어 있습니다.

1. 선택 내용을 저장하고 보고서로 돌아가려면 **URL 포함**&#x200B;을 클릭하세요.
