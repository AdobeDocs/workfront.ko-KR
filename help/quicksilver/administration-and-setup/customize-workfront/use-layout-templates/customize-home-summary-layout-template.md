---
title: 레이아웃 템플릿을 사용하여 요약 패널 사용자 정의
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 레이아웃 템플릿을 사용하여 사용자가 요약에서 작업 또는 문제를 클릭할 때 표시되는 내용을 구성할 수 있습니다. 아래 단계를 사용하여 수행하는 각 구성은 요약 패널에 영향을 줍니다. 이러한 사용자 지정은 문서 요약 패널에 적용되지 않습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 4%

---

# 레이아웃 템플릿을 사용하여 요약 패널 사용자 정의

<!--Audited: 11/2024-->

레이아웃 템플릿을 사용하여 사용자가 작업 또는 문제를 클릭할 때 요약 패널에 표시되는 내용을 구성할 수 있습니다. 아래 단계를 사용하여 수행하는 각 구성은 요약 패널에 영향을 줍니다. 이러한 사용자 지정은 문서 요약 패널에 적용되지 않습니다.

다음을 구성할 수 있습니다.

* 세부 정보 영역에 작업 또는 문제에 대해 표시되는 필드 및 순서
* 선택한 작업 또는 문제에 대한 업데이트, 기록된 시간, 첨부 문서 및 타임스탬프가 표시되는지 여부

사용자가 할당된 프로젝트 승인, 문서 승인 또는 문서 버전 승인을 클릭할 때 홈 영역에 표시되는 필드를 사용자 지정할 수도 있습니다.

요약 패널에 대한 자세한 내용은 [요약 개요](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)를 참조하십시오.

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.</p>
        <p>그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레이아웃 템플릿을 사용하여 요약 패널 사용자 정의

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.

1. ![사용자에게 표시되는 항목 사용자 지정](assets/dropdown-arrow.png)에서 아래쪽 화살표 **아래쪽 화살표**&#x200B;를 클릭한 다음 **요약 패널**&#x200B;을 클릭합니다.

1. 아래에 표시되는 목록에서 요약 패널을 사용자 지정할 객체 유형을 클릭합니다.

   아래 표에서는 각 객체에 대해 사용자 정의할 수 있는 내용을 설명합니다

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">작업</td> 
      <td> <p>작업 목록에서 이 설정은 사용자가 작업을 선택한 다음 요약 열기 아이콘 <img src="assets/summary-panel-icon.png">을(를) 클릭할 때 페이지 오른쪽에 표시되는 요약 패널에 영향을 줍니다.</p>

   <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문제</td> 
      <td><p>문제 목록에서 이 설정은 사용자가 문제를 선택한 다음 요약 열기 아이콘 <img src="assets/summary-panel-icon.png">을(를) 클릭할 때 페이지 오른쪽에 표시되는 요약 패널에 영향을 줍니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

<!--These were removed with the new Home: 

<tr> 
      <td role="rowheader">Projects</td> 
      <td><ul><li><p>In Home, when a user clicks a project approval assigned to them, your configuration for this setting affects the area to the right of the approval.</p>
      <p><b>IMPORTANT:</b> </p><p>This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td>
     <ul><li><p>In Home, when a user clicks a document approval assigned to them, your configuration for this setting affects the area to the right of the approval.</p>
      <p><b>IMPORTANT:</b> </p><p> This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Document Versions</td> 
      <td><ul><li><p>In Home, when a user clicks an approval assigned to them for a particular version of a document, your configuration for this setting affects the area to the right of the approval.</p>
      <p><p><b>IMPORTANT:</b></p> This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul>
      </td> 
     </tr> -->


>[!IMPORTANT]
>
>작업이 할당 해제된 경우 레이아웃 템플릿에 할당된 사용자에게 요약에 필드 사용자 지정이 표시되지 않습니다.

1. (조건부) 이전 단계에서 작업 또는 문제를 클릭한 경우 사용자 지정할 작업 또는 문제의 범주를 선택합니다.

   ![사용자 지정할 범주 선택](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (조건부) **기본 작업 설정 단추** 드롭다운 메뉴가 나타나면(왼쪽 목록에서 **작업** 또는 **문제**&#x200B;를 선택한 경우) 작업 또는 문제를 볼 때 요약 패널에서 사용자가 사용할 수 있는 기본 작업(**완료** 또는 **상태**)을 클릭합니다.

   ![기본 작업 설정](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. 선택한 개체 형식에 대해 ![항목 추가](assets/add-item-plus-in-circle-blue.png)를 추가하거나 ![항목 숨기기](assets/close-or-hide---x.png) 필드를 숨깁니다.

   ![필드 추가 및 숨기기](assets/lt-home-add-hide-fields-adobe-branding.png)

1. 다른 객체 유형에 대해 요약 패널을 사용자 정의하려면 3-6단계를 반복합니다.
1. 왼쪽 아래 모서리 근처에서 **전역 설정**&#x200B;을 클릭한 다음 요약에서 Adobe Workfront 개체와 관련된 다음 옵션을 활성화하거나 비활성화합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">작업 업데이트 보기</td> 
      <td>요약 패널에서 선택한 작업 또는 문제에 대한 모든 업데이트를 표시합니다. 여기에는 시스템 업데이트와 사용자가 수행한 업데이트가 모두 포함됩니다. 사용자는 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">작업 업데이트</a>의 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">시스템 업데이트 사용 또는 사용 안 함</a>에 설명된 대로 시스템 업데이트를 계속 필터링할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업에 대한 시간 기록</td> 
      <td>작업 또는 문제를 선택할 때 작업에 대해 시간 기록 옵션을 표시하여 사용자가 홈 및 요약 영역에서 직접 작업 항목에 시간을 기록할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업과 연결된 문서 보기</td> 
      <td>작업 또는 문제를 선택할 때 요약 패널에 문서 영역을 표시하고 작업 또는 문제에 첨부된 모든 문서를 나열합니다. 사용자는 문서를 클릭하여 미리보기 창에서 볼 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임스탬프 숨기기</td> 
      <td>요약 패널에서 다음 날짜 필드에 대한 타임스탬프를 숨깁니다.
       <ul>
        <li>계획된 완료 일자 기준</li>
        <li>커밋 일자</li>
        <li>제출 날짜</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. 레이아웃 템플릿을 계속 사용자 지정합니다. 언제든지 **적용**&#x200B;을 클릭하여 진행 상황을 저장할 수 있습니다.

   또는

   사용자 지정을 마쳤으면 **저장 후 닫기**&#x200B;를 클릭합니다.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.
