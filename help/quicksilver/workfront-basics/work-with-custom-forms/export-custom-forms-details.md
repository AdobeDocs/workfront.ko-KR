---
title: 사용자 지정 양식 및 개체 세부 정보 내보내기
description: 사용자 지정 양식 및 개체 세부 정보 내보내기
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# 사용자 지정 양식 및 개체 세부 정보 내보내기

개체의 세부 정보 섹션에서 개요 및 사용자 지정 양식 정보를 PDF 파일로 내보낼 수 있습니다. 그런 다음 PDF을 인쇄하거나 다른 사용자와 공유할 수 있습니다.

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
>레이아웃 템플릿을 사용하여 Workfront 또는 그룹 관리자가 제거한 세부 정보 섹션의 필드는 표시되지 않습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront 라이선스*</p> </td> 
   <td> <p>문제에 대한 요청 이상</p> <p>프로젝트 및 작업에 대한 검토 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>프로젝트, 작업 및 문제에 대한 보기 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>개체 권한</p> </td> 
   <td> <p>양식을 내보낼 프로젝트, 작업 또는 문제에 대한 권한 보기 또는 그 이상의 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에 다음을 모두 포함해야 합니다.

1. 내보낼 특정 객체에 대해 사용자 지정 양식을 만듭니다.
1. 개체에 사용자 지정 양식을 첨부합니다.

   또는

   사용자 지정 양식을 첨부하고 양식의 정보를 편집할 수 있는 올바른 액세스 권한이 있습니다.

사용자 지정 양식 만들기에 대한 내용은 [사용자 지정 양식 만들기 또는 편집](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

객체에 양식을 첨부하는 방법에 대한 내용은 [개체에 사용자 지정 양식 추가](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 세부 정보 섹션에서 정보 내보내기

개체의 세부 정보 섹션에서 정보를 내보내는 것은 지원되는 모든 개체에 대해 동일합니다.

1. 보기 권한이 있는 프로젝트, 작업, 포트폴리오, 프로그램 또는 문제로 이동합니다.
1. 을(를) 클릭합니다. **&quot;세부 정보&quot; 항목** 예를 들어 왼쪽 패널에서 **작업 세부 사항**.
1. (선택 사항) 개체에 첨부된 사용자 지정 양식이 없는 경우 **사용자 지정 양식 필드 추가**&#x200B;를 클릭한 다음 목록에 나타나면 클릭합니다.

   최대 10개의 양식을 추가할 수 있습니다.

1. (선택 사항) 세부 정보 섹션에서 정보를 업데이트한 다음 **변경 내용 저장**.
1. 을(를) 클릭합니다. **내보내기** 오른쪽 위 모서리에 있는 드롭다운 메뉴에서 **개요**&#x200B;또는 내보낼 양식을 클릭한 다음 **내보내기**.

   선택할 수도 있습니다 **모두 선택** 개요 영역과 모든 사용자 지정 양식을 내보내려면

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >다음 시나리오가 있을 수 있습니다.
   >
   >   
   >   
   >   * 그룹 또는 Workfront 관리자가 개요 영역의 모든 필드를 선택 취소하고 개체에 사용자 지정 양식이 첨부된 경우 개요 섹션이 표시되지 않습니다.
   >   * 그룹 또는 Workfront 관리자가 개요 영역의 모든 필드를 선택 취소하고 개체에 첨부된 사용자 지정 양식이 없으면 내보내기 드롭다운 메뉴가 표시되지 않습니다.
   >   * 개체에 첨부된 사용자 지정 양식이 없으면 개요 영역만 내보낼 수 있습니다.
   >   * 논리를 포함하고 양식에 표시되지 않는 사용자 지정 필드는 내보내지지 않습니다. 사용자 지정 양식에 논리를 추가하는 방법에 대한 자세한 내용은 [표시 논리를 추가하고 논리를 사용자 지정 양식에 건너뜁니다](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   PDF 파일이 생성되고 컴퓨터에 다운로드됩니다. PDF 파일에는 다음 정보가 포함됩니다.

   * 양식이 첨부된 개체의 이름입니다
   * PDF을 내보낸 사용자의 이름입니다
   * PDF 생성 날짜 및 시간
   * 내보낸 양식의 이름
   * 양식에 완료된 필드의 정보
