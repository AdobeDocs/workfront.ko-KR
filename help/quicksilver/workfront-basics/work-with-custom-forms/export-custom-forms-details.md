---
title: 사용자 정의 양식 및 개체 세부 정보 내보내기
description: 사용자 정의 양식 및 개체 세부 정보 내보내기
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 1%

---

# 사용자 정의 양식 및 개체 세부 정보 내보내기

<!--Audited: 10/2025-->

오브젝트의 세부 정보 섹션에서 개요 및 사용자 정의 양식 정보를 PDF 파일로 내보낼 수 있습니다. 그런 다음 PDF을 인쇄하거나 다른 사용자와 공유할 수 있습니다.

이 기능은 다음 개체에 대해 지원됩니다.

* 프로젝트
* 작업
* 문제
* 포트폴리오
* 프로그램

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Workfront 또는 그룹 관리자가 레이아웃 템플릿을 사용하여 제거한 세부 정보 섹션의 필드가 표시되지 않습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 패키지</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 라이선스</p> </td> 
   <td><p>문제의 경우:</p>
   <ul><li><p>기여자 이상</p></li>
   <li><p>요청자 이상</p> </li></ul>
   <p>프로젝트 및 작업의 경우:</p>
   <ul><li><p>밝거나 높음</p></li>
   <li><p>검토자 이상</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트, 작업 및 문제 보기 이상</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>개체 권한</p> </td> 
   <td> <p>양식을 내보내려는 프로젝트, 작업 또는 문제에 대한 이상의 권한 보기</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Request or higher for issues</p> <p>Review or higher for projects and tasks</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher for Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 전제 조건

시작하기 전에 다음을 모두 수행해야 합니다.

1. 내보낼 특정 개체에 대해 사용자 정의 양식을 만들어야 합니다.
1. 사용자 정의 양식을 오브젝트에 첨부합니다.

   또는

   올바른 액세스 권한을 가지고 사용자 정의 양식을 첨부하고 양식의 정보를 편집할 수 있습니다.

사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

개체에 양식을 첨부하는 방법에 대한 자세한 내용은 [개체에 사용자 정의 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

## 세부 정보 섹션의 정보 내보내기

객체의 세부내용 섹션에서 정보를 내보내는 것은 객체가 지원되는 모든 객체에 대해 동일합니다.

1. 보기 이상의 권한이 있는 프로젝트, 작업, 포트폴리오, 프로그램 또는 문제로 이동합니다.
1. 왼쪽 패널의 **&quot;세부 정보&quot; 항목**&#x200B;을 클릭합니다(예: **작업 세부 정보**).
1. (선택 사항) 개체에 첨부된 사용자 정의 양식이 없는 경우 **사용자 정의 양식 필드 추가**&#x200B;에서 사용자 정의 양식 이름을 입력한 다음 목록에 나타나면 클릭합니다.

   최대 10개의 양식을 추가할 수 있습니다.

1. (선택 사항) 세부 정보 섹션에서 정보를 업데이트한 다음 **변경 내용 저장**&#x200B;을 클릭합니다.
1. 오른쪽 상단의 **내보내기** 드롭다운 메뉴를 클릭하고, **개요** 또는 내보낼 양식을 선택한 다음 **내보내기**&#x200B;를 클릭합니다.

   개요 영역과 모든 사용자 정의 양식을 내보내려면 **모두 선택**&#x200B;을 선택할 수도 있습니다.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >다음과 같은 시나리오가 있을 수 있습니다.
   >
   >   * 그룹 또는 Workfront 관리자가 개요 영역에서 모든 필드를 선택 취소하고 오브젝트에 사용자 정의 양식이 첨부되어 있는 경우 개요 섹션이 표시되지 않습니다.
   >   * 그룹 또는 Workfront 관리자가 개요 영역에서 모든 필드를 선택 취소하고 오브젝트에 사용자 정의 양식이 첨부되어 있지 않은 경우 내보내기 드롭다운 메뉴가 표시되지 않습니다.
   >   * 오브젝트에 사용자 정의 양식이 첨부되어 있지 않은 경우 개요 영역만 내보낼 수 있습니다.
   >   * 논리보다 뒤처져 양식에 표시되지 않는 사용자 정의 필드는 내보낼 수 없습니다. 사용자 정의 양식에 논리를 추가하는 방법에 대한 자세한 내용은 [사용자 정의 양식 및 필드에 논리 규칙 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)를 참조하십시오.

   PDF 파일이 생성되고 컴퓨터에 다운로드됩니다. PDF 파일에는 다음 정보가 포함되어 있습니다.

   * 양식이 첨부된 개체의 이름입니다.
   * PDF을 내보낸 사용자의 이름
   * PDF이 생성된 날짜 및 시간입니다
   * 내보낸 양식의 이름
   * 양식에 작성된 필드의 정보
