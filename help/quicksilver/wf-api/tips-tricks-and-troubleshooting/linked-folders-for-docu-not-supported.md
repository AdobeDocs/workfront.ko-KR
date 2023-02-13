---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 연결된 폴더는 DOCX 개체에 대해 지원되지 않습니다
description: 연결된 폴더는 DOCX 개체에 대해 지원되지 않습니다
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# API를 사용하여 연결된 폴더를 추가할 수 없습니다

API를 사용하여 DOCU(문서) 개체의 폴더 배열에 연결된 폴더를 추가할 수 없습니다. 요청이 성공하지만 일부 외부 공급자가 문서를 시스템에서 제거할 수 있습니다. 외부 시스템이 최종 진실의 근원으로 이용되기 때문이다. 따라서 문서가 외부 공급자에서 제거되면 문서가 더 이상 존재하지 않는 것으로 간주됩니다. 연결된(외부) 폴더에 없는 문서는 [!DNL Workfront] 복구할 방법이 없습니다.
