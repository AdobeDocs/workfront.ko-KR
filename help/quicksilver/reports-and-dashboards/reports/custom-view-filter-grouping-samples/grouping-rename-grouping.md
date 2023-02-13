---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 그룹 ''에서 표시 이름 편집'
description: 그룹화를 사용자에게 더 친숙한 이름으로 변경할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 그룹화: 그룹에서 표시 이름 편집

그룹화를 사용자에게 더 친숙한 이름으로 변경할 수 있습니다.

예를 들어 표준 Portfolio 이름 그룹을 프로젝트 목록에 적용하면 그룹화의 이름이 *Portfolio: 이름:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

읽기 쉬운 이름을 표시하려면 텍스트 모드를 사용하여 이 그룹을 수정할 수 있습니다.

![](assets/grouping-edited-name-350x160.png)

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

## 그룹에서 표시 이름 편집

프로젝트 그룹의 표시 이름을 변경하려면

1. 프로젝트 목록으로 이동합니다.
1. 에서 **그룹화**&#x200B;드롭다운 메뉴에서 **새 그룹화**.

1. 클릭 **그룹화 추가**&#x200B;를 클릭하고, **먼저:** 필드를 선택한 다음 목록에 표시될 때 선택합니다.

1. 클릭 **텍스트 모드로 전환**.
1. 다음 중 하나를 수행합니다.

   * 다음 코드를 **보고서 그룹화** 상자:

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      또는, 이 경우:

      ```
      group.0.displayname=Portfolio
      ```

   * 그룹화의 텍스트 모드 인터페이스에서 &quot;name&quot;이라는 단어가 포함된 줄을 모두 제거한 다음 줄을 추가합니다.

      ```
      group.0.name=Your Value
      ```

      또는, 이 경우:

      ```
      group.0.name=Portfolio
      ```

      또한

      ```
      group.0.name
      ```

      라인 공백. 이 경우 그룹화는 그룹화할 값의 이름을 표시합니다.

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. 클릭 **완료**, 그런 다음 **그룹화 저장**.
