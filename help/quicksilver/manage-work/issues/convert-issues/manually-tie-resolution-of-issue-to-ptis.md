---
product-area: projects
navigation-topic: convert-issues
title: 문제 해결을 다른 문제, 작업 또는 프로젝트에 수동으로 연결
description: 문제를 변환하지 않고 문제 해결을 프로젝트, 작업 또는 문제 해결에 수동으로 연결할 수 있습니다. 이 문제는 선택한 프로젝트, 작업 또는 문제의 해결 가능 객체 중 하나가 됩니다. 이렇게 하면 프로젝트, 작업 또는 문제 상태의 변경이 원래 문제의 상태 변경을 트리거합니다.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: ea430157da539507c11a559a4dce6b24aca9e5a6
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 1%

---

# 문제 해결을 다른 문제, 작업 또는 프로젝트에 수동으로 연결

문제를 변환하지 않고 문제 해결을 프로젝트, 작업 또는 문제 해결에 수동으로 연결할 수 있습니다. 이 문제는 선택한 프로젝트, 작업 또는 문제의 해결 가능 객체 중 하나가 됩니다. 이렇게 하면 프로젝트, 작업 또는 문제 상태의 변경이 원래 문제의 상태 변경을 트리거합니다.

>[!TIP]
>
>문제 해결을 다른 객체의 해결에 연결하면 더 이상 원래 문제의 상태를 수동으로 편집할 수 없습니다.

해결 가능한 개체 해결 및 해결에 대한 자세한 내용은 [해결 가능한 객체 해결 및 해결 방법 개요](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제, 작업, 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>다른 문제, 작업 또는 프로젝트에 연결하는 문제에 대한 권한을 관리합니다</p> <p>기존 문제에 추가하는 문제, 작업 또는 프로젝트에 대한 권한 보기 또는 그 이상의 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* 다른 문제, 작업 또는 프로젝트의 해결에 연결할 해결 방법을 찾는 문제가 있습니다

* 추가 문제, 작업 또는 프로젝트 있음

## 문제 해결을 다른 문제, 작업 또는 프로젝트의 해결에 연결

1. 다른 문제 해결 또는 작업 또는 프로젝트의 해결에 연결할 해결 방법으로 이동합니다.
1. 을(를) 클릭합니다. **문제 세부 정보** > **개요** 영역.

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. 로 이동합니다. **개요** 의 영역 **문제 세부 정보** 섹션을 참조하십시오.
1. 을(를) 클릭합니다. **해결자** 필드를 선택하고 다음과 같은 객체 유형 중에서 선택합니다.

   * **프로젝트**
   * **작업**
   * **문제**

   선택한 객체에 따라 다음 필드가 표시됩니다.

   * **프로젝트 해결 중**
   * **해결 중인 작업**
   * **해결 중 문제**


1. 에 특정 프로젝트, 작업 또는 문제의 이름을 입력합니다. **프로젝트 해결**, **작업**, 또는 **문제** 필드를 클릭한 다음 목록에 나타나면 클릭합니다.

   >[!NOTE]
   >
   >문제 해결 방법을 문제 또는 문제가 있는 프로젝트에 연결할 수 없습니다. 문제의 작업 또는 프로젝트가 [해결 작업] 또는 [해결 작업] 필드에 표시되지 않습니다.


1. 클릭 **변경 내용 저장**.

   원래 문제는 4단계 및 5단계에서 선택한 프로젝트, 작업 또는 문제에 대한 해결 가능한 개체가 됩니다. 즉, 개체(프로젝트, 작업 또는 연결된 문제)가 해결되면 원래 문제가 완료됩니다.

   >[!NOTE]
   >
   >하나의 프로젝트, 작업 또는 문제에 해결 가능한 개체 같은 여러 문제가 있을 수 있습니다.
