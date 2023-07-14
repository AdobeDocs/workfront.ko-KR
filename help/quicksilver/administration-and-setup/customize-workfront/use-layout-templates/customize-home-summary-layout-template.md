---
title: 레이아웃 템플릿을 사용하여 홈 및 요약 맞춤화
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 레이아웃 템플릿을 사용하여 사용자가 홈 및 요약에서 작업 또는 문제를 클릭할 때 표시되는 내용을 구성할 수 있습니다. 아래 단계를 사용하여 구성하는 각 내용은 홈 영역과 요약 패널에 동일한 방식으로 영향을 줍니다. 이러한 사용자 지정은 문서 요약 패널에 적용되지 않습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 2%

---

# 레이아웃 템플릿을 사용하여 홈 및 요약 맞춤화

레이아웃 템플릿을 사용하여 사용자가 홈 및 요약에서 작업 또는 문제를 클릭할 때 표시되는 내용을 구성할 수 있습니다. 아래 단계를 사용하여 구성하는 각 내용은 홈 영역과 요약 패널에 동일한 방식으로 영향을 줍니다. 이러한 사용자 지정은 문서 요약 패널에 적용되지 않습니다.

다음을 구성할 수 있습니다.

* 세부 정보 영역에 작업 또는 문제에 대해 표시되는 필드 및 순서
* 선택한 작업 또는 문제에 대한 업데이트, 기록된 시간, 첨부 문서 및 타임스탬프가 표시되는지 여부

사용자가 할당된 프로젝트 승인, 문서 승인 또는 문서 버전 승인을 클릭할 때 홈 영역에 표시되는 필드를 사용자 지정할 수도 있습니다.

홈 영역에 대한 자세한 내용은 [홈 영역 사용](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). 요약 패널에 대한 자세한 내용은 [요약 개요](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md).

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가적인 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 레이아웃 템플릿을 사용하여 홈 및 요약 맞춤화

1. 에 설명된 대로 레이아웃 템플릿에서 작업 시작 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. 아래쪽 화살표 클릭 ![](assets/dropdown-arrow.png) 아래에 **사용자에게 표시되는 항목 맞춤화**&#x200B;을 클릭한 다음 을 클릭합니다 **홈 및 요약**.

1. 왼쪽에 나타나는 목록에서 개체 유형(**작업**, **문제**, **프로젝트**, **문서**, 또는 **문서 버전**)을 클릭하여 홈 및 요약에서 사용자 지정할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">작업</td> 
      <td> <p>홈에서 이 설정에 대한 구성은 사용자가 작업을 클릭할 때 작업 오른쪽의 영역에 영향을 줍니다. 또한 작업 목록에서 사용자가 작업을 선택한 다음 요약 열기 아이콘을 클릭할 때 페이지 오른쪽에 표시되는 요약 패널에 영향을 줍니다 <img src="assets/summary-panel-icon.png">.</p> <p>예를 들어 사용자가 홈에서 작업을 선택할 때 세부 정보 영역에 표시되는 필드를 결정할 수 있습니다.</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>요약에서 작업을 선택하는 경우:</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">문제</td> 
      <td> <p>홈에서 이 설정에 대한 구성은 사용자가 문제를 클릭할 때 문제의 오른쪽 영역에 영향을 줍니다.</p> <p>문제 목록에서 이 설정은 사용자가 문제를 선택한 다음 요약 열기 아이콘을 클릭할 때 페이지 오른쪽에 표시되는 요약 패널에 영향을 줍니다 <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">프로젝트</td> 
      <td>홈에서 사용자가 자신에게 할당된 프로젝트 승인을 클릭하면 이 설정에 대한 구성이 승인 오른쪽 영역에 영향을 줍니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">문서</td> 
      <td>홈에서 사용자가 자신에게 할당된 문서 승인을 클릭하면 이 설정에 대한 구성이 승인 오른쪽 영역에 영향을 줍니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">문서 버전</td> 
      <td>홈에서 사용자가 특정 버전의 문서에 대해 할당된 승인을 클릭하면 이 설정에 대한 구성이 승인 오른쪽 영역에 영향을 줍니다.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >작업이 할당 해제된 경우 레이아웃 템플릿에 할당된 사용자에게 요약에 필드 사용자 지정이 표시되지 않습니다.

1. (조건부) 이전 단계에서 작업 또는 문제를 클릭한 경우 사용자 지정할 작업 또는 문제의 범주를 선택합니다.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (조건부) **기본 작업 단추 설정** 드롭다운 메뉴가 나타납니다(선택하는 경우). **작업** 또는 **문제** 왼쪽 목록에서 기본 작업(**완료** 또는 **상태**) 홈 영역에서 사용자가 작업 또는 문제를 볼 때 요약 패널에서 사용할 수 있도록 하려는 경우.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. 추가 ![](assets/add-item-plus-in-circle-blue.png) 또는 숨기기 ![](assets/close-or-hide---x.png) 선택한 객체 유형에 대한 필드입니다.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. 다른 객체 유형에 대해 홈 영역 및 요약 패널을 사용자 정의하려면 3-6단계를 반복합니다.
1. 클릭 **전역 설정**&#x200B;을 클릭하고 왼쪽 하단 모서리 근처에서 홈 및 요약의 Adobe Workfront 오브젝트와 관련하여 다음 옵션 중 하나를 활성화하거나 비활성화합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">작업 업데이트 보기</td> 
      <td>홈 또는 요약에서 선택한 작업 또는 문제에 대한 모든 업데이트를 표시합니다. 여기에는 시스템 업데이트와 사용자가 수행한 업데이트가 모두 포함됩니다. 에 설명된 대로 사용자는 여전히 시스템 업데이트를 필터링할 수 있습니다. <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">시스템 업데이트 활성화 또는 비활성화</a> 위치: <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">작업 업데이트</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업에 대한 시간 기록</td> 
      <td>작업 또는 문제를 선택할 때 작업에 대해 시간 기록 옵션을 표시하여 사용자가 홈 및 요약 영역에서 직접 작업 항목에 시간을 기록할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업과 연결된 문서 보기</td> 
      <td>작업 또는 문제를 선택하면 홈 및 요약에 문서 영역을 표시하고 작업 또는 문제에 첨부된 모든 문서를 나열합니다. 사용자는 문서를 클릭하여 미리보기 창에서 볼 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임스탬프 숨기기</td> 
      <td>홈 및 요약의 다음 날짜 필드에 대한 타임스탬프를 숨깁니다.
       <ul>
        <li>계획된 완료 일자</li>
        <li>커밋 일자</li>
        <li><p>제출 날짜</p></li>
       </ul><p><b>참고</b>: 이 옵션을 활성화하면 기한이 경과된 작업 항목이 시간이 아닌 날짜만을 기준으로 홈 작업 목록에서 지연 그룹화로 이동됩니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장**.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
