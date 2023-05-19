---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 표준 인터페이스에 포함되지 않은 개체 표시'
description: 표준 모드 인터페이스에 포함되지 않은 객체를 뷰에 표시할 수 있습니다. 이 작업은 텍스트 모드를 통해 참조해야만 수행할 수 있습니다. 다음 방법 중 하나로 보기에 포함할 수 있는 필드를 결정할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 보기: 표준 인터페이스에 포함되지 않은 객체를 표시합니다.

표준 모드 인터페이스에 포함되지 않은 객체를 뷰에 표시할 수 있습니다. 이 작업은 텍스트 모드를 통해 참조해야만 수행할 수 있습니다.\
다음 방법 중 하나로 보기에 포함할 수 있는 필드를 결정할 수 있습니다.

* 사용 [API 탐색기](../../../wf-api/general/api-explorer.md) 텍스트 모드를 통해 참조할 수 있는 다른 객체를 검색합니다.\
   API 탐색기에 문서화된 모든 필드가 텍스트 모드에 유효한 필드는 아닙니다. 일부 필드는 API를 통해서만 보고할 수 있습니다.

* 열에서 개체의 ID 필드를 찾습니다. 필드 ID가 있는 대부분의 개체에는 표준 모드 인터페이스를 통해 액세스할 수 없는 해당 열 또는 필드 이름도 있습니다.

   텍스트 모드를 사용하여 ID 대신 열 또는 필드 이름을 뷰에 포함할 수 있습니다. `fieldnameID` (으)로 `fieldname:name`.

   예를 들어 표준 모드 인터페이스에서 **Portfolio 소유자 ID** 필드는 프로젝트 보기에 사용할 수 있지만 **Portfolio 소유자 이름** 필드가 아닙니다. 텍스트 모드를 사용하여 다음을 표시할 수 있습니다 **Portfolio 소유자 이름** 를 입력합니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 예: 프로젝트 보기에 Portfolio 소유자 이름 열 추가

1. 프로젝트 목록으로 이동합니다.
1. 다음에서 **보기** 드롭다운 메뉴, 클릭 **새 보기**.

1. 클릭 **열 추가** 그런 다음 &quot;Portfolio 소유자 ID&quot;를 **이 열에 표시** 필드를 선택한 다음 목록에 표시될 때 선택합니다.

1. 클릭 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 다음 **텍스트를 편집하려면 클릭**.
1. 바꾸기 `valuefield` 줄 (`valuefield=portfolio:ownerID`) 아래에 나열된 행을 사용할 수 있습니다.

   ```
   valuefield=portfolio:owner:name
   ```

   또는

   에서 찾은 텍스트 제거 **텍스트 모드** 확인란을 선택하고 다음 코드로 바꿉니다.

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   이 특정 예에서 보고서는 다음에 표시된 대로 Portfolio 소유자 ID별로 보고서를 정렬합니다. `querysort` 줄.

   >[!TIP]
   >
   >필드를 바꾸려면 `ID` (필드 포함) `name` 텍스트 모드 사용, 항상 바꾸기 `ID` 포함 `:name` 다음에서 `valuefield` 줄.

1. 클릭 **저장**, 그런 다음 **보기 저장**.
