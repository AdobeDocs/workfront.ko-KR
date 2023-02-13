---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 작업의 들여쓰기를 통해 작업의 상위-하위 관계를 표시합니다.'
description: 작업 목록에 사용자 정의 뷰를 추가하고 목록을 내보내기 전에 이 뷰를 선택하도록 하여 내보낸 작업 목록에서 상위 - 하위 관계를 구분할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 보기: 작업을 들여써서 작업의 상위-하위 관계를 표시합니다.

작업 목록에 사용자 정의 뷰를 추가하고 목록을 내보내기 전에 이 뷰를 선택하도록 하여 내보낸 작업 목록에서 상위 - 하위 관계를 구분할 수 있습니다.  

![](assets/parent-child-indented-custom-view-350x94.png)

1. 내보낼 작업 목록이 있는 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **보기** 드롭다운 메뉴에서 **새 보기**.

1. 화면의 왼쪽 상단 모서리에서 필터 이름을 지정합니다.
1. 을(를) 클릭합니다. **작업 이름** 열 헤더.

1. 선택 **텍스트 모드로 전환** 오른쪽 상단 모서리에서
1. 텍스트를 편집하고 기존 텍스트를 모두 제거하려면 텍스트 상자의 아무 곳이나 클릭합니다.
1. 다음 텍스트를 붙여넣습니다.

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. **저장**&#x200B;을 클릭합니다.
1. 클릭 **보기 저장**.
