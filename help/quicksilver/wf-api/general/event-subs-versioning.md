---
content-type: api
navigation-topic: general-api
title: 이벤트 구독 버전 관리
description: 이벤트 구독 API
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: 19e0b792bc49ede0504af479952fdbdf384dc73c
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 0%

---

# 이벤트 구독 버전 관리

Workfront에는 두 가지 버전의 이벤트 구독이 있습니다. 이 문서에서는 두 요소의 차이점에 대해 설명합니다.

새 버전은 Workfront API가 아니라 이벤트 구독 기능이 변경되었습니다.

이벤트 구독을 업그레이드하거나 다운그레이드할 수 있으므로 이벤트 구조가 변경될 때 기존 구독이 중단되지 않으므로 이벤트 구독에 공백 없이 새 버전으로 테스트하고 업그레이드할 수 있습니다.


이벤트 구독을 다른 버전으로 업그레이드하거나 다운그레이드하면 버전 변경 후 5분 동안 모든 이벤트 게재에 대해 중복 이벤트를 받습니다. 중복에는 이벤트 구독 버전 1과 버전 2가 각각 하나씩 포함됩니다. 이렇게 하면 이벤트 구독 버전 변경으로 인해 이벤트를 놓치지 않습니다.

이벤트 구독을 업그레이드하거나 다운그레이드하는 데 사용되는 끝점에 대한 자세한 내용은 이벤트 구독 API 문서에서 [이벤트 구독 버전 관리](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning)를 참조하십시오.

>[!IMPORTANT]
>
>다음 릴리스는 이벤트 구독 버전 관리에 영향을 줍니다.
>
>* **25.2 릴리스**(2025년 4월 10일): 25.2 릴리스 이후에 만들어진 모든 새 구독은 버전 2로 만들어집니다.
>* **25.3 릴리스**(2025년 7월 17일): 25.3 릴리스 이후 구독을 더 이상 버전 1로 다운그레이드할 수 없습니다.
>* **2026년 1월 15일**: 나머지 모든 버전 1 구독이 버전 2로 마이그레이션됩니다.

## 버전 1과 버전 2 간의 변경 사항

이벤트 구독 버전 2가 다음과 같이 변경되었습니다.


### 일반 변경 사항


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>영향을 받는 필드</b></p> </th> 
   <th> <p><b>버전 1(이전 비헤이비어)</b></p> </th> 
   <th> <p><b>버전 2(변경)</b></p> </th> 
   <th> <p><b>업데이트 관리 작업</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>계산된 매개변수 값</p> </td> 
   <td> <p>계산된 매개 변수 값이 있는 사용자 정의 양식을 포함한 템플릿에서 만든 모든 오브젝트는 <code>CREATE</code> 이벤트가 전송되고 <code>UPDATE</code>은(는) 매개 변수 값(계산된 필드 및 해당 값 포함)과 함께 전송됩니다. </p> </td> 
   <td> <p>계산된 매개 변수 값이 있는 사용자 정의 양식을 포함하는 템플릿에서 개체를 만들면 <code>CREATE</code> 이벤트만 전송되고 계산된 필드를 포함하는 매개 변수 값을 포함합니다.</p> </td> 
   <td> <p><code>UPDATE</code> 이벤트에 대한 구독이 있고 계산된 매개 변수 값으로 개체를 만든 후 <code>UPDATE</code> 이벤트를 받아야 하는 경우 해당 <code>UPDATE</code> 이벤트는 더 이상 받지 않습니다. 개체를 만들 때 계산된 매개 변수 값을 보려면 추가 <code>CREATE</code> 구독을 만들어야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>다중 선택 유형 필드</p> </td> 
   <td> <p>다중 선택 유형 필드에 대한 변경 사항을 포함하는 모든 유형의 이벤트에 대해 필드에 하나의 값만 포함된 경우 해당 값이 로 변환되어 문자열로 전송됩니다. 그렇지 않으면 배열로 전송됩니다. </p><p>예:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> <code>myMultiSelectField: "oneValue"</code>(으)로 변환되어 전송됩니다.</li><li><code>myMultiSelectField: ["first", "second"]</code> 은(는) <code>myMultiSelectField: ["first", "second"]</code>(으)로 전송됩니다.</li></ul> </td> 
   <td> <p>배열에 있는 값의 수에 관계없이 배열로 전송됩니다. </p><p>예:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> 은(는) <code>myMultiSelectField: ["oneValue"]</code>(으)로 전송됩니다.</li><li><code>myMultiSelectField: ["first", "second"]</code> 은(는) <code>myMultiSelectField: ["first", "second"]</code>(으)로 전송됩니다.</li></ul> </td> 
   <td> <p>다중 선택 필드에 필터가 있는 구독이 있고 값이 문자열인 경우 값이 배열로 있는 것과 동일한 필터로 새 구독을 만들어야 합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

### 오브젝트별 변경 사항

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>개체 코드</b> </th> 
   <th> <b>영향을 받는 필드</b> </th> 
   <th> <b>버전 1(이전 동작)</b></th> 
   <th> <b>버전 2(변경)</b> </th> 
   <th> <b>업데이트 관리 작업</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ASSIGN</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>이 개체가 업데이트되면 <code>UPDATE</code> 이벤트에 영향을 받는 필드가 <code>null</code>에서 <code>ID value</code>(으)로 변경되는 것으로 잘못 표시되기도 합니다.</td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.</td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 다른 값이 변경된 것이 아니라 이러한 필드가 실제로 변경된 경우에만 <code>UPDATE</code> 이벤트를 받습니다.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">도쿠</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>이 개체에서 매개 변수 값이 업데이트되면 <code>UPDATE</code> 이벤트에 영향을 받는 필드가 <code>null</code>에서 <code>object id</code>(으)로 잘못 표시되었습니다. </td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.</td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 다른 값이 변경된 것이 아니라 이러한 필드가 실제로 변경된 경우에만 <code>UPDATE</code> 이벤트를 받습니다.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>문서가 삭제되면 <code>DELETE</code> 이벤트가 영향을 받는 필드를 이전 상태의 빈 배열로 잘못 표시했습니다.    </td> 
   <td><code>DELETE</code> 이벤트는 이전 상태의 영향을 받는 필드를 올바르게 표시합니다.</td> 
   <td>없음. <code>DELETE</code> 이벤트가 계속 전송되지만 지금은 영향을 받는 필드에 대한 올바른 데이터를 표시합니다. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>이 개체가 업데이트되면 두 개의 <code>UPDATE</code> 이벤트가 전송됩니다. 첫 번째 이벤트에는 영향을 받는 필드가 포함되지 않았지만 두 번째 이벤트에는 영향을 받는 필드가 포함되지 않았습니다.</td> 
   <td>영향을 받는 필드를 포함한 모든 필드 업데이트가 하나의 <code>UPDATE</code> 이벤트에만 있으며 두 번째 불필요한 이벤트는 전송되지 않습니다.     </td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 이벤트는 첫 번째 이벤트에서 전달됩니다. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">확장</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>비용에 대해 매개 변수 값이 업데이트되면 <code>UPDATE</code> 이벤트에서 <code>EXPNS</code>에서 <code>PROJ</code>(으)로 topReferenceObjCode가 잘못 변경되고 <code>referenceObjectName</code>에서 <code>null</code>에서 <code>string value of project name</code>(으)로 변경되었습니다.      </td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.</td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 다른 값이 변경된 것이 아니라 이러한 필드가 실제로 변경된 경우에만 <code>UPDATE</code> 이벤트를 받습니다.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>경비 개체가 삭제되면 <code>DELETE</code> 이벤트가 전송되기 전에 영향을 받는 필드를 null로 변경하는 <code>UPDATE</code> 이벤트가 전송되었습니다.    </td> 
   <td>추가 <code>UPDATE</code> 이벤트가 전송되지 않습니다. <code>DELETE</code> 이벤트에 이전 상태의 영향을 받는 필드에 대한 올바른 값이 있습니다. </td> 
   <td><code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 필터가 있고 개체가 삭제될 때 해당 필드를 받아야 하는 경우 해당 <code>UPDATE</code> 이벤트는 더 이상 받지 않습니다. 개체가 삭제될 때 이러한 필드를 보려면 추가 <code>DELETE</code> 구독을 만들어야 합니다.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">시간</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>이 개체가 삭제되면 <code>DELETE</code> 이벤트가 영향을 받는 필드를 이전 상태의 <code>null</code>(으)로 잘못 표시했습니다. </td> 
   <td><code>DELETE</code> 이벤트는 이전 상태의 영향을 받는 필드를 올바르게 표시합니다.</td> 
   <td>없음. <code>DELETE</code> 이벤트가 계속 전송되지만, 지금은 영향을 받는 필드에 대한 올바른 데이터가 표시됩니다. </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>이 개체에서 매개 변수 값이 업데이트되면 <code>UPDATE</code> 이벤트에 영향을 받는 필드가 <code>null</code>에서 <code>ID value</code>(으)로 잘못 표시되었습니다. </td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.</td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 <code>UPDATE</code> 이벤트는 해당 필드가 실제로 변경된 경우에만 수신되며, 다른 매개 변수 값이 변경된 경우에는 수신되지 않습니다.
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>이 개체가 업데이트되면 <code>UPDATE</code> 이벤트에 영향을 받는 필드가 <code>null</code>에서 <code>ID value</code>(으)로 변경되는 것으로 잘못 표시되기도 합니다.</td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">프로젝트</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>이 개체에서 매개 변수 값이 업데이트되면 <code>UPDATE</code> 이벤트에 영향을 받는 필드가 <code>null</code>에서 <code>ID value</code>(으)로 잘못 표시되었습니다. </td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.</td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 <code>UPDATE</code> 이벤트는 해당 필드가 실제로 변경된 경우에만 수신되며, 다른 매개 변수 값이 변경된 경우에는 수신되지 않습니다.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>이 개체가 업데이트되면 <code>UPDATE</code> 이벤트에 영향을 받는 필드가 <code>null</code>에서 <code>ID value</code>(으)로 변경되는 것으로 잘못 표시되기도 합니다.</td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.</td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 <code>UPDATE</code> 이벤트는 해당 필드가 실제로 변경된 경우에만 수신되며, 다른 매개 변수 값이 변경된 경우에는 수신되지 않습니다.
  </tr> 
  <tr> 
   <th rowspan="2">작업</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>이 개체에서 매개 변수 값이 업데이트되면 <code>UPDATE</code> 이벤트에 영향을 받는 필드가 <code>null</code>에서 <code>ID value</code>(으)로 잘못 표시되었습니다. </td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.</td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 <code>UPDATE</code> 이벤트는 해당 필드가 실제로 변경된 경우에만 수신되며, 다른 매개 변수 값이 변경된 경우에는 수신되지 않습니다.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>이 개체가 업데이트되면 <code>UPDATE</code> 이벤트에 영향을 받는 필드가 <code>null</code>에서 <code>ID value</code>(으)로 변경되는 것으로 잘못 표시되기도 합니다.</td> 
   <td>모든 <code>UPDATE</code> 이벤트에 영향을 받는 필드에 대한 올바른 값이 표시됩니다.</td> 
   <td>없음. 영향을 받는 필드에 필터가 있는 경우 <code>UPDATE</code> 이벤트는 해당 필드가 실제로 변경된 경우에만 수신되며, 다른 매개 변수 값이 변경된 경우에는 수신되지 않습니다.
 </tbody> 
</table>


## Workfront Fusion 시나리오에서 이벤트 구독 버전 업데이트

Workfront Fusion은 이벤트 구독을 사용하여 Workfront의 변경 사항을 살펴보고 시나리오를 트리거합니다. Workfront > 이벤트 페이로드 버전 업데이트 모듈을 사용하여 Fusion이 시나리오에서 직접 사용하는 이벤트 구독 버전을 업데이트할 수 있습니다.

이 모듈 사용에 대한 지침은 Workfront Fusion 설명서의 [Workfront 모듈](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules)을 참조하십시오.
