---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 연결된 폴더는 DOCU 개체에 대해 지원되지 않습니다.
description: 연결된 폴더는 DOCU 개체에 대해 지원되지 않습니다.
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 0%

---

# API를 사용하여 연결된 폴더를 추가하는 작업은 지원되지 않습니다

API를 사용하여 문서(DOCU) 객체의 폴더 배열에 연결된 폴더를 추가할 수 없습니다. 요청이 성공하지만 일부 외부 공급자에 의해 문서가 시스템에서 제거될 수 있습니다. 외부 시스템이 진실의 최종 원천으로 활용될 것이기 때문이다. 따라서 문서가 외부 공급자에서 제거되면 문서가 더 이상 존재하지 않는 것으로 간주됩니다. 연결된(외부) 폴더에서 찾을 수 없는 모든 문서는 복구할 방법이 없이 [!DNL Workfront]에서 자동으로 제거될 수 있습니다.
