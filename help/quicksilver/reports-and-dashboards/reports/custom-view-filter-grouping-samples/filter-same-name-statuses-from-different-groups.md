---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 상태가 다른 그룹과 연결된 경우 동일한 이름 상태별로 항목 표시'
description: 3자 키 NST를 사용하여 Group A에 작업 상태를 New Status로 지정할 수 있습니다. 3자 키 NES를 사용하여 New Status라는 다른 작업 상태가 그룹 B에 할당되었을 수 있습니다. 두 상태의 이름은 동일할 수 있지만, 3자로 된 코드는 항상 고유합니다. 그룹 상태에 대한 자세한 내용은 그룹 상태 만들기 또는 편집을 참조하십시오.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 필터: 상태가 다른 그룹과 연결된 경우 동일한 이름 상태별로 항목 표시

다음과 같은 그룹 A에 작업 상태를 할당할 수 있습니다. *새 상태* 3자로 된 키 *NST*. 다음과 같은 다른 작업 상태가 그룹 B에 할당되었을 수 있습니다. *새 상태* 3자로 된 키 *네.* 두 상태의 이름은 동일할 수 있지만, 3자로 된 코드는 항상 고유합니다.\
그룹 상태에 대한 자세한 내용은 [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

필터 빌더를 사용하면 이름이 같은 두 상태 간에 식별할 수 없습니다. 두 상태를 구분하려면 텍스트 모드 를 사용해야 합니다.

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
   <td> <p>필터 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 상태가 다른 그룹과 연결된 경우 동일한 이름 상태별로 항목 표시

1. 작업 목록에 대해 사용자 지정할 필터(예: )로 이동합니다.\
   이는 프로젝트 및 문제에도 동일하게 작동합니다.
1. 클릭 **필터 규칙 추가** 대상: **상태** 목록의 개체 필드.\
   예를 들어 작업 보고서에서 다음을 추가합니다. **상태가 새 상태와 같음**, 상태의 작업만 표시하려는 경우 **새 상태**.

   >[!TIP]
   >
   >새 상태(New Status)라는 상태에 대해 하나의 옵션만 있습니다.

1. 클릭 **텍스트 모드로 전환**.\
   다음 코드가 표시됩니다.

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >여기에는 하나의 상태만 표시됩니다. 상태 라인에는 상태 중 하나에 대한 3자리 키 중 하나가 표시됩니다.

1. 다음 2줄의 코드를 추가하여 필터에서 누락된 상태를 추가합니다.

   <pre>또는:1:status=NES<br>또는:1:status_Mod=in</pre>

1. 클릭 **완료**, 그런 다음 **필터 저장**.

   목록에는 그룹 A의 상태가 &quot;신규 상태&quot;이고 그룹 B의 상태가 &quot;신규 상태&quot;인 작업이 모두 표시됩니다.
