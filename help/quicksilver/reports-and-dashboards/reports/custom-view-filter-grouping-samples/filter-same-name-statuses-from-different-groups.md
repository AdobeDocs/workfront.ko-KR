---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 상태가 다른 그룹과 연관된 경우 동일한 이름 상태별로 항목 표시'
description: 3자 키 NST를 사용하여 Group A에 작업 상태를 New Status로 지정할 수 있습니다. 3자 키 NES를 사용하여 New Status라는 다른 작업 상태가 그룹 B에 할당되었을 수 있습니다. 두 상태의 이름은 동일할 수 있지만, 3자로 된 코드는 항상 고유합니다. 그룹 상태에 대한 자세한 내용은 그룹 상태 만들기 또는 편집을 참조하십시오.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 필터: 상태가 다른 그룹과 연결된 경우 동일한 이름 상태별로 항목 표시

<!--Audited: 10/2024-->

3자리 키 *NST*&#x200B;을(를) 사용하여 *새 상태*(이)라는 그룹 A에 작업 상태를 할당할 수 있습니다. 3자리 키 *NES를 사용하여*&#x200B;새 상태&#x200B;*(이)라는 다른 작업 상태가 그룹 B에 할당되었을 수 있습니다.* 두 상태의 이름은 동일할 수 있지만, 3자로 된 코드는 항상 고유합니다.

그룹 상태에 대한 자세한 내용은 [그룹 상태 만들기 또는 편집](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)을 참조하세요.

필터 빌더를 사용하면 이름이 같은 두 상태 간에 식별할 수 없습니다. 두 상태를 구분하려면 사용자 지정 필터에서 텍스트 모드 를 사용해야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>필터 수정을 위한 기여자 또는 요청 </p>
   <p>표준 또는 보고서 수정 계획</p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 상태가 다른 그룹과 연결된 경우 동일한 이름 상태별로 항목 표시

1. 작업 목록에 대해 사용자 지정할 필터의 **필터** 드롭다운으로 이동합니다.\
   이는 프로젝트 및 문제에도 동일하게 작동합니다.
1. **새 필터**&#x200B;를 클릭합니다.
1. 왼쪽 상단 모서리의 첫 번째 드롭다운에서 작업 > 상태 를 선택합니다.
1. 한정자에 대해 **같음**&#x200B;을 선택한 다음 보고할 상태 중 하나를 선택하십시오.

   예를 들어, **새 상태** 상태의 작업만 표시하려면 작업 보고서에 **상태가 새 상태와 같음**&#x200B;을(를) 추가하십시오.

   >[!TIP]
   >
   >새 상태(New Status)라는 상태에 대해 하나의 옵션만 있습니다.

1. **텍스트 모드**&#x200B;를 클릭합니다.\
   다음 코드는 제공된 공간에 표시되어야 합니다.

   <pre>또는:1:상태=NST<br>또는:1:상태_Mod=in </pre>

   >[!NOTE]
   >
   >여기에는 하나의 상태만 표시됩니다. 상태 라인에는 상태 중 하나에 대한 3자리 키 중 하나가 표시됩니다.

1. 다음 2줄의 코드를 추가하여 필터에서 누락된 상태를 추가합니다.

   <pre>또는:2:상태=NES<br>또는:2:상태_Mod=in</pre>

1. **적용**&#x200B;을 클릭한 다음 **새 이름으로 저장**&#x200B;을 클릭합니다.

   목록에는 그룹 A의 상태가 &quot;신규 상태&quot;이고 그룹 B의 상태가 &quot;신규 상태&quot;인 작업이 모두 표시됩니다.
