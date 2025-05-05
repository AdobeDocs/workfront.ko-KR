---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Adobe Workfront API를 사용하여 시간 레코드 추적
description: 조직에서 Adobe Workfront을 사용하여 작업 시간을 입력하지만 다른 도구를 해당 데이터에 대한 기록 시스템으로 사용하는 경우 Workfront API를 사용하여 두 시스템 간에 데이터를 동기화할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Adobe Workfront API를 사용하여 시간 레코드 추적

조직에서 Adobe Workfront을 사용하여 작업 시간을 입력하지만 다른 도구를 해당 데이터에 대한 기록 시스템으로 사용하는 경우 Workfront API를 사용하여 두 시스템 간에 데이터를 동기화할 수 있습니다.

시간 항목이 제거되면 전체 레코드가 삭제되므로 전체 데이터 세트를 가져와 이전 데이터 세트와 비교해야 하므로 단순히 시간 레코드를 추적할 수는 없습니다. 다행히도 모든 시간 트랜잭션은 Workfront 분개 입력에 기록됩니다.

시스템에서 모든 현재 시간의 초기 세트를 검색한 후 분개 입력을 통해 모든 변경 사항을 추적할 수 있습니다.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>&lbrace;<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7e2e 8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "578540600 93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": 5785416ff 008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler",<br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode" ",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br></pre>다음은 포함된 필드에 대한 설명입니다.

* **changeType:** 개체에 적용되는 변경 형식:

   * **A:** 추가

   * **전자 메일:** 편집

   * **일:** 삭제

* **aux2:** 시간 기록이 있는 사용자의 이름입니다.

* **newNumberVal:** 시간 레코드의 새 값(changeType이 D인 경우 null임).

* **oldNumberVal:** 시간 레코드의 이전 값.

* **subObjCode:** 수정 중인 레코드 종류(항상 HOUR이어야 함)입니다.

* **subObjID:** 시간 레코드의 ID.

이 정보를 사용하여 변경, 편집 또는 삭제된 시간 레코드를 검색할 수 있습니다. 그런 다음 필요한 경우 subObjID를 사용하여 시간 레코드에서 자세한 정보를 검색할 수 있습니다.
