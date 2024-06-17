---
product-area: projects;user-management
keywords: 첨부,적용
navigation-topic: work-with-custom-forms
title: 오브젝트에 사용자 정의 양식 추가
description: 아래 나열된 객체에 기존 사용자 정의 양식을 추가할 수 있습니다. 사용자 정의 양식에는 객체에 대한 정보를 저장할 수 있는 사용자 정의 필드가 포함되어 있습니다.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 2%

---

# 오브젝트에 사용자 정의 양식 추가

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

아래 나열된 객체에 기존 사용자 정의 양식을 추가할 수 있습니다. 사용자 정의 양식에는 객체에 대한 정보를 저장할 수 있는 사용자 정의 필드가 포함되어 있습니다.

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
* 과금 기록

사용자 정의 양식은 양식을 만든 객체 유형에만 추가할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서에 설명된 작업을 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront 라이선스</td> 
  <td> <p>새로운 기능: 기여자 이상 </p>
 <p>또는</p> 
<p>현재: 요청 이상 </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식을 관리하는 객체에 대한 액세스 편집</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>사용자 정의 양식을 첨부할 객체에 대한 권한을 관리합니다.</p> <p>에 대한 권한이 있는 사용자 정의 양식에 대한 이상의 권한을 봅니다. <b>사용자 정의 데이터에 첨부</b> 오브젝트(프로젝트, 작업 및 문제) 자세한 내용은 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">사용자 정의 양식 공유</a>.</p> <p>중요: 사용자 정의 Forms에 대한 관리 액세스 권한이 있는 플랜 라이선스가 없는 경우에서 설명한 대로 사용자 정의 양식을 적어도 볼 수 있는 특정 권한이 있어야 합니다 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">사용자 정의 양식 공유</a>. 양식이 시스템 전체에 표시되는 경우에도 이러한 권한을 부여해야 합니다. </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 전제 조건

Workfront 관리자 또는 플랜 라이선스와 사용자 정의 양식에 대한 관리 액세스 권한이 있는 사용자는 사용자 정의 양식을 오브젝트에 추가하려면 먼저 사용자 정의 양식을 만들어야 합니다. 자세한 내용은 [사용자 정의 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 오브젝트에 사용자 정의 양식 추가

다음 두 가지 방법으로 사용자 정의 양식을 오브젝트에 추가할 수 있습니다.

* [개체를 편집하여 개체에 사용자 정의 양식 추가](#add-a-custom-form-to-an-object-by-editing-the-object)
* [세부 정보 영역에서 오브젝트에 사용자 정의 양식 추가](#add-a-custom-form-to-an-object-from-the-details-area)

### 개체를 편집하여 개체에 사용자 정의 양식 추가 {#add-a-custom-form-to-an-object-by-editing-the-object}

1. 사용자 정의 양식을 추가하려는 객체로 이동합니다.
1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)을 클릭한 다음 을 클릭합니다 **편집** ![](assets/edit-icon.png).
1. 클릭 **사용자 지정 Forms** > **Forms 추가**&#x200B;을 클릭한 다음 드롭다운 메뉴에서 최대 10개의 양식을 선택합니다.

1. (선택 사항) 사용자 정의 양식의 편집 가능한 필드에서 정보를 업데이트합니다.

   추가한 양식의 모든 필수 필드를 업데이트해야 합니다.

1. **저장**&#x200B;을 클릭합니다.

### 세부 정보 영역에서 오브젝트에 사용자 정의 양식 추가 {#add-a-custom-form-to-an-object-from-the-details-area}

1. 사용자 정의 양식을 추가하려는 객체로 이동합니다.
1. 다음을 클릭합니다. **`<Object type>`세부 사항** 왼쪽 패널의 섹션입니다. 예를 들어 **프로젝트 세부 정보** 프로젝트에 사용자 정의 양식을 추가하려면 다음을 수행하십시오. **문제 세부 정보** 사용자 정의 양식을 문제에 추가합니다.
1. 다음을 클릭합니다. **사용자 정의 양식 추가** 오른쪽 위 모서리에 있는 필드를 선택한 다음 표시되는 목록에서 최대 10개의 사용자 정의 양식을 선택합니다.

   양식에 필수 필드(빨간색 별표로 표시)가 포함되어 있으면 지금 완료하지 않아도 됩니다.

   선택한 양식이 개체에 자동으로 첨부됩니다.

1. (선택 사항) 양식의 사용자 정의 필드에서 정보를 업데이트한 다음 **변경 내용 저장**.

## 오브젝트에 대한 여러 사용자 정의 양식

특정 오브젝트에 최대 10개의 사용자 정의 양식을 추가할 수 있으므로 필드를 다른 사용자가 아닌 일부 사용자가 사용할 수 있도록 하거나 여러 프로젝트의 양식 요구 사항을 보다 잘 충족할 수 있습니다.

**예:** 기존 프로젝트에 이미 사용자 정의 양식이 있고 다른 사용자 정의 양식에 있는 이 프로젝트에 더 많은 사용자 정의 필드가 필요한 경우, 기존 사용자 정의 양식에 필드를 추가하는 대신 추가 필드를 사용하여 프로젝트에 두 번째 양식을 추가할 수 있습니다.

## 여러 개체에 사용자 정의 양식 일괄 추가

목록에서 사용자 정의 양식을 선택하여 여러 객체에 추가할 수 있습니다.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>오브젝트에 사용자 정의 양식을 추가하는 것은 프로젝트를 제외한 모든 오브젝트에 대해 동일합니다.
>
>프로젝트에 사용자 정의 양식을 대량으로 추가하는 방법에 대한 자세한 내용은 문서 를 참조하십시오 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md).


1. 객체 목록으로 이동합니다.
1. 목록에서 여러 객체를 선택합니다.

1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭하고 **편집** 아이콘  ![](assets/edit-icon.png).

   또는

   다음을 클릭합니다. **편집** 아이콘 ![](assets/edit-icon.png) 목록의 맨 위에 있습니다.
1. 클릭 **사용자 지정 Forms** 왼쪽 패널에서
1. 다음에서 **선택** 드롭다운 메뉴에서 선택한 모든 객체와 연결할 양식을 선택합니다.

   >[!NOTE]
   >
   >드롭다운 메뉴에서 양식을 찾을 수 없는 경우, 하나 이상의 객체에 이미 연관된 양식이 있음을 의미합니다. 나머지 개체에 양식을 추가하기 전에 해당하는 개체를 결정하고 선택 항목에서 제거합니다.


1. **변경 내용 저장**&#x200B;을 클릭합니다.

   양식에 필수 필드(빨간색 별표로 표시)가 포함되어 있으면 지금 완료하지 않아도 됩니다.
