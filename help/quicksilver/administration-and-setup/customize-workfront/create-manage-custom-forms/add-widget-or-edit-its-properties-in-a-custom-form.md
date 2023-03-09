---
title: 기존 양식 빌더를 사용하여 사용자 정의 양식의 이미지 또는 기타 에셋 위젯 추가 또는 편집
description: 이미지, 비디오, PDF 파일 및 Adobe XD 파일과 같은 다음 에셋 위젯의 속성을 사용자 정의 양식에 추가하거나 편집할 수 있습니다. 이 기능은 디자인하는 앱에 대한 브랜딩 이미지, 지침 비디오 또는 대화형 프로토타입과 같은 시각적 콘텐츠를 포함해야 할 때 유용합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '1344'
ht-degree: 1%

---

# 기존 양식 빌더를 사용하여 사용자 정의 양식의 이미지 또는 기타 에셋 위젯 추가 또는 편집

사용자 정의 양식에서 다음 에셋 위젯의 속성을 추가하거나 편집할 수 있습니다.

* 이미지
* 비디오
* PDF 파일
* Adobe XD 파일

이 기능은 디자인하는 앱에 대한 브랜딩 이미지, 지침 비디오 또는 대화형 프로토타입과 같은 시각적 콘텐츠를 포함해야 할 때 유용합니다.

위젯이 포함된 사용자 정의 양식을 오브젝트에 첨부할 때 오브젝트로 작업하는 사용자는 다음 영역에서 해당 양식을 볼 수 있습니다.

* 객체의 세부 정보 영역(예: 프로젝트의 경우 프로젝트 세부 정보 영역)
* 새로운 Adobe Workfront 경험 모양과 느낌이 있는 객체의 편집 상자(예: 프로젝트 편집 및 작업 편집 상자)

현재 사용자는 다음 영역에서 위젯을 볼 수 없습니다&#x200B;.

* 목록 및 보고서
* 홈 및 요약
* 새로운 Adobe Workfront 경험 룩앤필이 없는 객체의 편집 상자(예: 경비 편집 상자)입니다
* Workfront 모바일 앱


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">사용자에게 특정 영역에 대한 관리 액세스 권한 부여</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 정의 양식에서 에셋 위젯 추가 또는 편집

1. 에 설명된 대로 사용자 정의 양식 작업을 시작합니다. [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 포함 **필드 추가** 탭을 열고 다음 중 하나를 수행합니다.

   * 새 위젯을 추가하는 경우 **이미지**, **PDF**, 또는 **비디오** 을 클릭하여 폼의 맨 아래에 추가하거나, 폼에서 원하는 위치로 끕니다.

      ![](assets/add-widget.png)


   * 다른 사용자 정의 양식에 이미 추가된 위젯을 추가하려면 **필드 라이브러리**&#x200B;을 클릭한 다음 표시되는 목록에서 위젯 이름을 클릭합니다. 자세한 내용은 [사용자 정의 양식에서 사용자 정의 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * 사용자 정의 양식에 이미 추가된 위젯을 편집하는 경우에는 해당 위젯을 선택합니다.

1. 위젯에 대해 다음 속성 중 하나를 입력하거나 편집합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 위젯 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 이 레이블에는 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 이 이름은 시스템이 위젯을 식별하는 방법입니다.</p> <p>위젯을 처음 구성하는 경우 레이블을 입력하면 이름 필드가 위젯과 일치하도록 자동으로 채워집니다. 그러나 레이블 및 이름 필드는 동기화되지 않으므로 시스템에서 볼 수 있는 이름을 변경하지 않고도 사용자가 볼 수 있는 레이블을 자유롭게 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 사용자 또는 다른 사용자가 위젯에서 사용자 정의 양식을 사용하기 시작한 후에는 이 이름을 변경하지 않는 것이 좋습니다. 그렇게 하면 시스템은 이제 Workfront의 다른 영역에서 참조될 수 있는 위젯을 더 이상 인식하지 않습니다. </p> <p>각 위젯 이름은 조직의 Workfront 인스턴스에서 고유해야 합니다. 이렇게 하면 다른 사용자 정의 양식에 대해 이미 만들어진 파일을 다시 사용할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(필수) 인터넷에서 저장된 위젯의 URL을 입력하거나 붙여넣습니다.</p> 
       <p><strong>중요 사항</strong>: 의 URL은 공개 URL이어야 합니다. </p>
      <p>비디오 위젯을 추가하는 경우 현재 URL 상자에 다음을 추가하여 추가할 수 있습니다.</p> 
      <ul> 
      <li> <p>YouTube 또는 Vimeo 링크</p> </li> 
      <li> <p>Google 드라이브 비디오 링크</p> </li> 
      <li> <p>MP4 및 MOV 확장으로 비디오에 연결</p> </li> 
      <li> <p>Workfront 인스턴스의 문서 영역에 이미 업로드된 비디오에 대한 링크입니다. 자세한 내용은 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">문서 영역에서 사용자 정의 양식에 비디오 위젯 추가</a> 이 문서에서.</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>위젯에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">크기</td> 
      <td>필요에 따라 위젯의 표시 크기를 변경합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **적용**.
1. 다른 방법으로 사용자 정의 양식을 계속 작성하려면 다음 문서 중 하나를 계속 진행하십시오.

   * [사용자 정의 양식에 사용자 정의 필드 및 위젯 배치](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [사용자 정의 양식에서 사용자 정의 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [사용자 정의 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 정의 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## 사용자 정의 양식에 XD 파일 추가

1. 에 설명된 대로 사용자 정의 양식 작업을 시작합니다. [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 포함 **필드 추가** 탭을 열고 다음을 선택합니다 **Adobe XD**.
1. 위젯에 대해 다음 속성 중 하나를 입력하거나 편집합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 위젯 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 이 레이블에는 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 이 이름은 시스템이 위젯을 식별하는 방법입니다.</p> <p>위젯을 처음 구성하는 경우 레이블을 입력하면 이름 필드가 위젯과 일치하도록 자동으로 채워집니다. 그러나 레이블 및 이름 필드는 동기화되지 않으므로 시스템에서 볼 수 있는 이름을 변경하지 않고도 사용자가 볼 수 있는 레이블을 자유롭게 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 사용자 또는 다른 사용자가 위젯에서 사용자 정의 양식을 사용하기 시작한 후에는 이 이름을 변경하지 않는 것이 좋습니다. 그렇게 하면 시스템은 이제 Workfront의 다른 영역에서 참조될 수 있는 위젯을 더 이상 인식하지 않습니다. </p> <p>각 위젯 이름은 조직의 Workfront 인스턴스에서 고유해야 합니다. 이렇게 하면 다른 사용자 정의 양식에 대해 이미 만들어진 파일을 다시 사용할 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(필수) 유효한 XD 프로토타입 링크를 입력하거나 붙여넣습니다.</p> 
      <p>참고: Adobe XD의 공유 탭에 있는 링크 액세스 설정은 링크가 있는 모든 사용자에게 설정되어야 합니다. 그렇지 않으면 사용자가 프로토타입을 볼 수 없습니다. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>(선택 사항) 위젯에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">크기</td> 
      <td>(선택 사항) 필요한 경우 위젯의 표시 크기를 변경합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 다른 방법으로 사용자 정의 양식을 계속 작성하려면 다음 문서 중 하나를 계속 진행하십시오.

   * [사용자 정의 양식에 사용자 정의 필드 및 위젯 배치](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 정의 양식에 사용자 정의 필드 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [사용자 정의 양식에서 사용자 정의 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [사용자 정의 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 정의 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 문서 영역에서 사용자 정의 양식에 비디오 위젯 추가 {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>이러한 방식으로 사용자 정의 양식에 비디오를 추가하면 사용자가 오브젝트의 양식에 액세스할 때 사용자 정의 양식에 대해 설정된 권한만 비디오에 적용되고 문서 영역의 비디오에 대해 설정된 권한은 적용되지 않습니다.

1. 에 설명된 대로 문서 영역에서 비디오로 이동하여 증명을 생성합니다 [웹 사이트 또는 기타 웹 콘텐츠에 대한 대화형 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 증명을 엽니다.
1. 비디오에서 아무 곳이나 마우스 오른쪽 버튼으로 클릭한 다음 를 선택합니다. **비디오 주소 복사**.
1. 비디오 위젯을 추가하는 사용자 정의 양식에서 복사한 주소를 **URL** 상자.
