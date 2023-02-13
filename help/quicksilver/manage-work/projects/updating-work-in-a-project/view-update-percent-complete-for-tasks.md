---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업에 대한 완료율 보기 및 갱신
description: 작업 완료율을 업데이트하여 작업 완료율을 완료하기 위한 작업 진행 상황을 나타낼 수 있습니다.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 작업에 대한 완료율 보기 및 갱신

작업 완료율을 업데이트하여 작업 완료율을 완료하기 위한 작업 진행 상황을 나타낼 수 있습니다.

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

작업을 수동으로 업데이트하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.


## 작업 완료율을 업데이트할 수 있는 영역

다음 영역 중 하나에서 작업에 대한 완료율을 업데이트할 수 있습니다.

* **작업 목록에서**: 완료 퍼센트 열이 표시되면 작업의 완료 비율을 업데이트할 수 있습니다.\
   인라인 편집에 대한 자세한 내용은 [Adobe Workfront의 목록에서 인라인 편집 항목](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **이정표 보기에서**: 프로젝트 목록이나 프로젝트 보고서에서 이정표 보기를 사용할 때 작업 완료율을 업데이트할 수 있습니다. 자세한 내용은 [이정표 보기 사용](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **작업을 업데이트할 때**: 작업에 업데이트를 추가할 때 작업의 완료율 옵션을 업데이트할 수 있습니다.

   >[!IMPORTANT]
   >
   >이 옵션은 완료 퍼센트 표시 옵션을 활성화한 후에만 표시됩니다.\
   >작업에 대한 전체 업데이트 비율 창을 활성화하려면 다음을 수행하십시오.
   >
   >1. 로 이동합니다. **기본** 메뉴>이름>**자세히** 아이콘 옆에 있는 이름 >**편집** > 선택 **업데이트 상태에 완료 비율 표시**.\
      >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >


* **작업 헤더에서**: 작업 헤더에서 작업 완료율을 업데이트할 수 있습니다. 자세한 내용은 [작업 편집](../../tasks/manage-tasks/edit-tasks.md).

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## 작업 완료율 업데이트

1. Workfront의 다음 영역으로 이동합니다.

   * 작업 목록
   * 프로젝트 목록 및 이정표 보기 적용
   * 작업 페이지에 액세스하여 작업
1. 을(를) 찾습니다 **완료율** 갱신하려는 완료율이 포함된 작업의 필드입니다.
1. 완료 퍼센트 필드 내부를 클릭하고 0에서 100 사이의 숫자를 입력합니다

   또는

   을(를) 클릭하고 **완료율** 필요한 번호에 대한 표시줄을 입력하여 완료된 작업의 양을 나타냅니다.

   >[!NOTE]
   >
   >작업의 100%가 완료되었음을 나타내는 경우 작업의 상태도 완료됨으로 업데이트됩니다.


1. 키보드에서 Enter 키를 눌러 완료율을 저장합니다.

