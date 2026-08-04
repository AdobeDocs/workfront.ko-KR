---
user-type: administrator
product-area: system-administration;setup
title: 변경 내역에서 추적할 필드 구성
description: Workfront 관리자는 Workfront이 추적하는 오브젝트 필드 및 작업을 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 6%

---

# 변경 내역에서 추적할 필드 구성

{{highlighted-preview-article-level}}

Adobe Workfront은 다음 이벤트를 기록하기 위해 자동 시스템 업데이트를 생성합니다.

* 사용자가 오브젝트 필드에서 변경한 사항
* 사용자가 객체에 대해 수행하는 작업

이러한 시스템 업데이트에는 다음 유형의 정보가 포함됩니다.

* 변경된 내용
* 변경한 사용자의 이름
* 변경 시간 및 날짜

Workfront 관리자는 Workfront이 추적하는 오브젝트 필드 및 작업을 구성할 수 있습니다.

예를 들어 Workfront에서 사용자가 시스템 전체에서 문제 이름에 적용한 모든 변경 사항을 추적할 수 있습니다. 그러면 모든 문제 이름 변경 사항이 변경 기록 로그에 항목으로 나타납니다. 자세한 내용은 [변경 내용 보기 및 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>시스템 관리자</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 필드 추적 제한

추적할 수 있는 필드 수에 대한 제한은 Workfront 패키지에 의해 정의됩니다.

| Workfront 패키지 | 추적된 최대 필드 수 |
|---------|----------|
| 선택 | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| 워크플로 선택 | 1000 |
| 워크플로 프라임 | 5000 |
| 워크플로 얼티밋 | 무제한 |

## 추적할 필드 추가

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적 > 구성**&#x200B;을 클릭합니다.
1. 구성 화면에서 **필드 추가**&#x200B;를 클릭합니다.
1. **필드 추가** 상자에서 개체를 선택합니다. 개체 이름을 입력한 다음 목록에 표시될 때 선택할 수 있습니다.
1. 그런 다음 해당 객체에 대해 추적할 필드 이름을 선택합니다. 필드 이름을 입력한 다음 목록에 나타날 때 필드 이름을 선택할 수 있습니다.

   사용자 정의 필드와 기본 필드는 모두 오브젝트에 사용할 수 있습니다.
   이미 추적 중인 필드가 목록에서 선택된 상태로 표시됩니다.

   ![변경 내용 추적을 위한 필드 추가](assets/change-history-config-add-fields.png)

1. 추적할 모든 필드를 선택한 후 **추가**&#x200B;를 클릭합니다.

   필드가 추적된 필드 목록에 추가됩니다.

## 더 이상 추적하지 않을 필드 제거

Workfront 인터페이스 전체에서 특정 유형의 개체에 대해 시스템에서 추적하지 않으려는 필드를 제거할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적 > 구성**&#x200B;을 클릭합니다.
1. 구성 화면에서 추적을 중지할 필드를 선택합니다.

   동일한 필드 이름이 두 번 이상 표시될 수 있습니다. 필드는 정확한 필드를 찾을 수 있도록 오브젝트별로 그룹화됩니다. 화면 상단의 검색 상자를 사용할 수도 있습니다.

1. 화면 하단의 작업 표시줄에서 **삭제**&#x200B;를 선택합니다.
1. 확인 메시지에서 **제거**&#x200B;를 클릭합니다.

   필드는 추적된 필드 목록에서 제거됩니다.


