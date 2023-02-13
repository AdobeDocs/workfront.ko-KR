---
title: 사용자 지정 양식에서 이미지 또는 기타 자산 위젯을 추가하거나 편집합니다
description: 이미지, 비디오, PDF 파일 및 Adobe XD 파일과 같은 다음 자산 위젯의 속성을 사용자 지정 양식에 추가하거나 편집할 수 있습니다. 이 기능은 브랜딩 이미지, 교육용 비디오 또는 디자인하는 앱의 대화형 프로토타입과 같은 시각적 컨텐츠를 포함해야 할 경우에 유용합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: eeff0c8a3f7cbccd942c978d771d24f4cf9c425d
workflow-type: tm+mt
source-wordcount: '1325'
ht-degree: 1%

---

# 사용자 지정 양식에서 이미지 또는 기타 자산 위젯을 추가하거나 편집합니다

사용자 지정 양식에서 다음 자산 위젯의 속성을 추가하거나 편집할 수 있습니다.

* 이미지
* 비디오
* PDF 파일
* Adobe XD 파일

이 기능은 브랜딩 이미지, 교육용 비디오 또는 디자인하는 앱의 대화형 프로토타입과 같은 시각적 컨텐츠를 포함해야 할 경우에 유용합니다.

위젯이 포함된 사용자 지정 양식이 개체에 첨부된 경우 개체를 사용하여 작업하는 사용자는 다음 영역에서 위젯을 볼 수 있습니다.

* 객체의 세부 정보 영역(예: 프로젝트의 경우 프로젝트 세부 정보 영역)
* 객체에 대한 편집 상자(예: 프로젝트 편집 및 작업 편집 상자)가 새 Adobe Workfront 경험 모양과 느낌

현재 사용자는 다음 영역에서 위젯을 볼 수 &#x200B; 없습니다.

* 목록 및 보고서
* 홈 및 요약
* 개체의 편집 상자에 새 Adobe Workfront 경험 모양과 느낌(예: 비용 편집 상자)이 없는 경우
* Workfront 모바일 앱


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;보유한 계획, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 지정 양식에서 자산 위젯 추가 또는 편집

1. 에 설명된 대로 사용자 지정 양식 작업을 시작합니다. [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 사용 **필드 추가** 탭을 열고 다음 중 하나를 수행합니다.

   * 새 위젯을 추가하는 경우 **이미지**, **PDF**, 또는 **비디오** 양식 맨 아래에 추가하거나 양식에서 원하는 위치로 드래그합니다.

      ![](assets/add-widget.png)


   * 이미 다른 사용자 지정 양식에 추가된 위젯을 추가하려면 을 클릭합니다 **필드 라이브러리**&#x200B;를 클릭한 다음 표시되는 목록에서 위젯 이름을 클릭합니다. 자세한 내용은 [사용자 지정 양식에서 사용자 지정 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * 사용자 지정 양식에 이미 추가된 위젯을 편집하는 경우 해당 위젯을 선택합니다.

1. 위젯에 대해 다음 속성 중 하나를 입력하거나 편집합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 위젯 위에 표시할 수사적 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 이 레이블에서 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 시스템이 위젯을 식별하는 방법입니다.</p> <p>처음으로 위젯을 구성하고 레이블을 입력하면 이름 필드가 자동으로 채워져서 일치하는 항목을 찾습니다. 그러나 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에서 표시되는 이름을 변경하지 않고도 사용자가 보는 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 가능하지만 사용자나 다른 사용자가 위젯에서 사용자 지정 양식을 사용하기 시작한 후에는 이 이름을 변경하지 않는 것이 좋습니다. 그럴 경우 시스템은 이제 Workfront의 다른 영역에서 참조할 수 있는 위젯을 더 이상 인식하지 못합니다. </p> <p>각 위젯 이름은 조직의 Workfront 인스턴스에서 고유해야 합니다. 이렇게 하면 다른 사용자 지정 양식에 대해 이미 생성된 양식을 다시 사용할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(필수) 위젯이 인터넷에 저장되는 URL을 입력하거나 붙여넣습니다.</p> 
      <p>비디오 위젯을 추가하는 경우 현재 URL 상자에 다음을 추가하여 추가할 수 있습니다.</p> 
      <ul> 
      <li> <p>YouTube 또는 Vimeo 링크</p> </li> 
      <li> <p>Google Drive 비디오 링크</p> </li> 
      <li> <p>MP4 및 MOV 확장을 사용하여 비디오에 연결</p> </li> 
      <li> <p>Workfront 인스턴스의 문서 영역에 이미 업로드된 비디오에 대한 링크입니다. 자세한 내용은 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">문서 영역에서 사용자 지정 양식에 비디오 위젯을 추가합니다</a> 참조하십시오.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>위젯에 대한 추가 정보를 입력합니다. 사용자가 사용자 지정 양식을 작성하면 물음표 아이콘을 마우스로 가리키면 여기에 입력하는 정보가 포함된 도구 설명이 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">크기</td> 
      <td>필요에 따라 위젯의 표시 크기를 변경합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **적용**.
1. 사용자 지정 양식을 다른 방식으로 계속 빌드하려면 다음 문서 중 하나를 계속 진행합니다.

   * [사용자 지정 양식에 사용자 지정 필드 및 위젯을 배치합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 지정 양식에 사용자 지정 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [사용자 지정 양식에서 사용자 지정 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 지정 양식에서 기존의 계산된 사용자 지정 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [표시 논리를 추가하고 논리를 사용자 지정 양식에 건너뜁니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 지정 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## 사용자 지정 양식에 XD 파일 추가

1. 에 설명된 대로 사용자 지정 양식 작업을 시작합니다. [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 사용 **필드 추가** 탭을 열고, **Adobe XD**.
1. 위젯에 대해 다음 속성 중 하나를 입력하거나 편집합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 위젯 위에 표시할 수사적 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 이 레이블에서 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 시스템이 위젯을 식별하는 방법입니다.</p> <p>처음으로 위젯을 구성하고 레이블을 입력하면 이름 필드가 자동으로 채워져서 일치하는 항목을 찾습니다. 그러나 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에서 표시되는 이름을 변경하지 않고도 사용자가 보는 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 가능하지만 사용자나 다른 사용자가 위젯에서 사용자 지정 양식을 사용하기 시작한 후에는 이 이름을 변경하지 않는 것이 좋습니다. 그럴 경우 시스템은 이제 Workfront의 다른 영역에서 참조할 수 있는 위젯을 더 이상 인식하지 못합니다. </p> <p>각 위젯 이름은 조직의 Workfront 인스턴스에서 고유해야 합니다. 이렇게 하면 다른 사용자 지정 양식에 대해 이미 생성된 양식을 다시 사용할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(필수) 유효한 XD 프로토타입 링크를 입력하거나 붙여넣습니다.</p> 
      <p>참고: Adobe XD의 공유 탭에 있는 링크 액세스 설정은 링크가 있는 모든 사람으로 설정되어야 합니다. 그렇지 않으면 사용자가 프로토타입을 볼 수 없습니다. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>(선택 사항) 위젯에 대한 추가 정보를 입력합니다. 사용자가 사용자 지정 양식을 작성하면 물음표 아이콘을 마우스로 가리키면 여기에 입력하는 정보가 포함된 도구 설명이 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">크기</td> 
      <td>(선택 사항) 필요에 따라 위젯의 표시 크기를 변경합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 사용자 지정 양식을 다른 방식으로 계속 빌드하려면 다음 문서 중 하나를 계속 진행합니다.

   * [사용자 지정 양식에 사용자 지정 필드 및 위젯을 배치합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 지정 양식에 사용자 지정 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [사용자 지정 양식에서 사용자 지정 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 지정 양식에서 기존의 계산된 사용자 지정 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [표시 논리를 추가하고 논리를 사용자 지정 양식에 건너뜁니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 지정 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 문서 영역에서 사용자 지정 양식에 비디오 위젯을 추가합니다 {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>이러한 방식으로 사용자 지정 양식에 비디오를 추가할 때는 사용자가 문서 영역에서 비디오에 설정된 권한이 아니라 개체의 양식에 액세스할 때 사용자 지정 양식에 대해 설정된 권한만 비디오에 적용됩니다.

1. Documents 영역의 비디오로 이동하여 다음에 설명된 대로 증명을 생성합니다. [웹 사이트 또는 기타 웹 컨텐츠에 대한 대화형 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 증명을 엽니다.
1. 비디오의 아무 곳이나 마우스 오른쪽 단추로 클릭한 다음 을 선택합니다 **비디오 주소 복사**.
1. 비디오 위젯을 추가할 사용자 지정 양식에서 복사한 주소를 **URL** 상자.
