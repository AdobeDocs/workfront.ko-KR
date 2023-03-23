---
product-area: projects;user-management
keywords: 첨부,적용
navigation-topic: work-with-custom-forms
title: 개체에 사용자 지정 양식 추가
description: 아래 나열된 개체 중 하나에 기존 사용자 지정 양식을 추가할 수 있습니다. 사용자 지정 양식에는 개체에 대한 정보를 저장할 수 있는 사용자 지정 필드가 포함되어 있습니다.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: addcff71ff067be22e9ee80f997af545293fa5db
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# 개체에 사용자 지정 양식 추가

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 환경의 모든 고객과 프로덕션 환경의 고객 선택 그룹에 대해 사용할 수 있습니다.</span>

아래 나열된 개체 중 하나에 기존 사용자 지정 양식을 추가할 수 있습니다. 사용자 지정 양식에는 개체에 대한 정보를 저장할 수 있는 사용자 지정 필드가 포함되어 있습니다.

* 프로젝트(비즈니스 사례 포함)
* 작업
* 문제
* 회사
* 포트폴리오
* 프로그램
* 문서
* 사용자
* 반복
* 경비
* 청구 레코드

양식을 만든 개체 형식에만 사용자 지정 양식을 추가할 수 있습니다.

## 액세스 요구 사항

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>사용자 지정 양식을 관리하는 개체에 대한 액세스 편집</p> <p><b>메모</b></p>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>사용자 지정 양식을 첨부할 개체에 대한 권한을 관리합니다.</p> <p>사용자 지정 양식에 대한 권한을 보고 <b>사용자 지정 데이터에 첨부</b> 객체(프로젝트, 작업 및 문제) 자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">사용자 지정 양식 공유</a>.</p> <p>중요 사항: 사용자 지정 Forms에 대한 관리자 액세스 권한이 있는 계획 라이센스가 없는 경우 다음에 설명된 대로 사용자 지정 양식을 볼 특정 권한이 있어야 합니다. <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">사용자 지정 양식 공유</a>. 이러한 권한은 양식이 시스템 전체에 걸쳐 표시되는 경우에도 사용자에게 부여되어야 합니다. </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

Workfront 관리자나 사용자 지정 양식에 대한 계획 라이선스 및 관리 액세스 권한이 있는 사용자는 사용자 정의 양식을 만든 후에 객체에 추가할 수 있습니다. 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 개체에 사용자 지정 양식 추가

다음 두 가지 방법으로 개체에 사용자 지정 양식을 추가할 수 있습니다.

* [개체를 편집하여 개체에 사용자 지정 양식 추가](#add-a-custom-form-to-an-object-by-editing-the-object)
* [세부 정보 영역에서 개체에 사용자 지정 양식 추가](#add-a-custom-form-to-an-object-from-the-details-area)

### 개체를 편집하여 개체에 사용자 지정 양식 추가 {#add-a-custom-form-to-an-object-by-editing-the-object}

1. 사용자 지정 양식을 추가할 개체로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집** ![](assets/edit-icon.png).
1. 클릭 **사용자 지정 Forms** > **Forms 추가**&#x200B;을 선택한 다음 드롭다운 메뉴에서 최대 10개의 양식을 선택합니다.

1. (선택 사항) 사용자 지정 양식의 편집 가능한 필드에서 정보를 업데이트합니다.

   추가한 양식에서 필수 필드를 모두 업데이트해야 합니다.

1. **저장**&#x200B;을 클릭합니다.

### 세부 정보 영역에서 개체에 사용자 지정 양식 추가 {#add-a-custom-form-to-an-object-from-the-details-area}

1. 사용자 지정 양식을 추가할 개체로 이동합니다.
1. 을(를) 클릭합니다. **`<Object type>`세부 사항** 왼쪽 패널의 섹션에 있습니다. 예를 들어 **프로젝트 세부 사항** 프로젝트에 사용자 지정 양식을 추가하려면 **문제 세부 정보** 문제에 사용자 지정 양식을 추가하려면
1. 을(를) 클릭합니다. **사용자 지정 양식 추가** 오른쪽 상단 모서리의 필드를 선택한 다음 표시되는 목록에서 최대 10개의 사용자 지정 양식을 선택합니다.

   양식에 필수 필드(빨간색 별표로 표시됨)가 포함되어 있는 경우, 지금은 완료하지 않아도 됩니다.

   선택한 양식이 개체에 자동으로 첨부됩니다.

1. (선택 사항) 양식의 사용자 지정 필드에서 정보를 업데이트한 다음 를 클릭합니다 **변경 내용 저장**.

## 개체의 여러 사용자 지정 양식

특정 개체에 최대 10개의 사용자 지정 양식을 추가할 수 있으므로, 일부 사용자가 필드를 사용할 수 있도록 하거나, 다른 사용자가 사용할 수 없도록 하거나, 여러 프로젝트의 양식 요구 사항을 더 잘 충족할 수 있습니다.

**예:** 기존 프로젝트에 사용자 지정 양식이 이미 있고 다른 사용자 지정 양식에 있는 사용자 지정 필드가 더 필요한 경우 해당 필드가 이 프로젝트에만 필요한 경우 기존 사용자 지정 양식에 필드를 추가하는 대신 추가 필드가 있는 프로젝트에 두 번째 양식을 추가할 수 있습니다.

## 여러 개체에 사용자 지정 양식 일괄 추가

사용자 지정 양식을 목록에서 선택하여 여러 개체에 추가할 수 있습니다.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">미리 보기 환경에서 프로젝트에 사용자 지정 양식을 대량으로 추가하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md)</span>.


1. 개체 목록으로 이동합니다.
1. 목록에서 여러 개체를 선택합니다.

1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)를 클릭한 다음 **편집** 아이콘  ![](assets/edit-icon.png)를 클릭하거나 **편집** 아이콘 ![](assets/edit-icon.png).
1. 클릭 **사용자 지정 Forms** 왼쪽 패널에 표시됩니다.
1. 에서 선택한 모든 개체와 연결할 양식을 선택합니다 **선택** 드롭다운 메뉴
   >[!NOTE]
   >
   >드롭다운 메뉴에서 양식을 찾을 수 없으면 하나 이상의 개체가 이미 연결된 양식을 가지고 있음을 의미합니다. 양식을 나머지 객체에 추가하기 전에 해당 객체를 결정하고 선택 항목에서 제거합니다.

1. 클릭 **변경 내용 저장**.

   양식에 필수 필드(빨간색 별표로 표시됨)가 포함되어 있는 경우, 지금은 완료하지 않아도 됩니다.
