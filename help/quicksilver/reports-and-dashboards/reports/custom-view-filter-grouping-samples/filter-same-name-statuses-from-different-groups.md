---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 상태가 다른 그룹의 상태와 연결되면 동일한 이름 상태의 항목을 표시합니다'
description: 3자로 된 키 NST를 사용하여 이름이 New Status 인 그룹 A에 작업 상태를 지정할 수 있습니다. B 그룹에 New Status라는 이름을 3자로 된 키 NES로 지정한 다른 작업 상태가 있을 수 있습니다. 두 상태의 이름이 동일할 수 있지만 세 글자 코드는 항상 고유합니다. 그룹 상태에 대한 자세한 내용은 그룹 상태 만들기 또는 편집을 참조하십시오.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 필터: 상태가 다른 그룹과 연결되어 있을 때 동일한 이름 상태의 항목을 표시합니다

이름이 지정된 그룹 A에 작업 상태를 지정할 수 있습니다 *새 상태* 3자 키로 *NST*. 그룹 B에 다른 작업 상태가 할당되어 있을 수 있습니다. *새 상태* 3자 키로 *네* 두 상태의 이름이 동일할 수 있지만 세 글자 코드는 항상 고유합니다.\
그룹 상태에 대한 자세한 내용은 [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

필터 빌더를 사용하면 동일한 이름의 두 상태 간을 식별할 수 없습니다. 텍스트 모드를 사용하여 두 상태를 구분해야 합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 상태가 다른 그룹과 연결되어 있을 때 동일한 이름 상태의 항목을 표시합니다

1. 작업 목록에 대해 사용자 지정할 필터로 이동합니다(예: ).\
   프로젝트 및 문제에도 동일하게 작동합니다.
1. 클릭 **필터 규칙 추가** 대상 **상태** 목록의 개체 필드입니다.\
   예를 들어 작업 보고서에서 을 추가합니다 **상태 같음 새 상태**&#x200B;로 설정되면, **새 상태**.

   >[!TIP]
   >
   >New Status라는 상태에 대한 옵션은 하나만 있습니다.

1. 클릭 **텍스트 모드로 전환**.\
   다음 코드가 표시됩니다.

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >여기에 하나의 상태만 표시됩니다. 상태 줄에는 상태 중 하나에 대한 3자 키 중 하나가 표시됩니다.

1. 필터에 누락된 상태를 추가하려면 다음 2줄의 코드를 추가합니다.

   <pre>또는:1:status=NES<br>또는:1:status_Mod=in</pre>

1. 클릭 **완료**, 그런 다음 **필터 저장**.

   이 목록에는 그룹 A의 상태가 &quot;새 상태&quot;이고 그룹 B의 상태가 &quot;새 상태&quot;인 두 작업이 모두 표시됩니다.
