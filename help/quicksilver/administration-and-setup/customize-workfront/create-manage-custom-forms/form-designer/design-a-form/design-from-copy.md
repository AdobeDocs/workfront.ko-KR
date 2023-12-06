---
title: 양식 디자이너를 사용하여 사본에서 양식 디자인
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 양식 디자이너를 사용하여 사본에서 사용자 정의 양식을 디자인할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# 양식 디자이너를 사용하여 사본에서 양식 디자인

기존 양식을 기반으로 하는 새 사용자 정의 양식을 디자인할 수 있습니다. 다른 Workfront 개체에 사용자 정의 양식을 첨부하여 해당 개체에 대한 데이터를 캡처할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>
   <p>새 플랜: 표준</p>
   <p>또는</p>
   <p>현재 플랜: 플랜</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">사용자에게 특정 영역에 대한 관리 액세스 권한 부여</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 정의 양식을 복사하여 새 양식 만들기

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms.**
1. 새 사용자 정의 양식의 기반으로 사용할 사용자 정의 양식을 선택한 다음 를 클릭합니다 **복사**.
1. 다음에서 **사용자 정의 양식 복사** 나타나는 상자에 다음 정보를 입력합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">양식 이름</td> 
      <td>복사된 양식의 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">양식 유형 </p> </td> 
      <td> <p>다음에서 <b>양식 유형</b> 상자에서 사용자 정의 양식을 사용할 객체 유형을 선택하고 제거할 유형 옆의 X를 클릭합니다. 양식과 이미 연결되어 있는 유형은 목록에서 비활성화됩니다.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>양식은 하나 이상의 개체 유형과 연결되어 있어야 합니다.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **양식 복사**.

   원래 양식에서 계산된 필드가 새 양식에 추가하는 오브젝트 유형과 호환되지 않는 필드를 참조하는 경우, 해당 필드의 계산을 변경하라는 메시지가 표시됩니다.

   마찬가지로 원본 양식의 섹션 구분에 대한 액세스 옵션이 새 양식에 추가하는 오브젝트 유형과 호환되지 않으면 옵션을 조정하라는 메시지가 표시됩니다.

1. 방금 복사한 양식을 선택한 다음 **편집**.
1. 다음 섹션에 설명된 대로 양식을 변경합니다. [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) 문서:

* [다른 사용자 정의 양식에서 이미 사용된 기존 필드 또는 위젯 재사용](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [텍스트 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [라디오 버튼, 확인란 그룹 및 드롭다운 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [자동 완성 및 날짜 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [이미지, PDF 및 비디오 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Adobe XD 파일 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (선택 사항) **저장+닫기**&#x200B;에 설명된 대로 양식을 사용하려는 오브젝트에 첨부합니다 [오브젝트에 사용자 정의 양식 추가](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
