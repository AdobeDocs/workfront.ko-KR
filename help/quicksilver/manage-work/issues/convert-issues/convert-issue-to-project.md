---
product-area: projects
navigation-topic: convert-issues
title: Adobe Workfront에서 문제를 프로젝트로 변환
description: Adobe Workfront에서 문제를 프로젝트로 변환
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# Adobe Workfront에서 문제를 프로젝트로 변환

문제를 제출한 후 문제를 완료하기 위해 추가 작업을 수행해야 하는 경우 문제를 프로젝트로 변환할 수 있습니다.

문제를 새 프로젝트로 변환하거나 템플릿을 사용하여 프로젝트로 변환할 수 있습니다. 이 문서에서는 문제를 프로젝트로 변환하는 두 방법에 대해 설명합니다.

문제 변환에 대한 일반적인 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제, 작업 및 프로젝트에 대한 액세스 편집</p> <p>재무 데이터에 대한 액세스를 편집하여 문제와 변환된 예상 재무 정보를 갱신합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 보기</p> <p>문제가 변환된 후 프로젝트에 대한 관리 권한을 받습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 문제를 프로젝트로 변환

템플릿을 사용하여 문제를 빈 프로젝트로 변환하거나 문제를 프로젝트로 변환할 수 있습니다.

1. 프로젝트로 이동하여 를 클릭합니다 **[!UICONTROL 문제]** 왼쪽 패널에 표시됩니다.
1. 표시되는 문제 목록에서 다음 중 하나를 수행합니다.

   * 문제를 빈 프로젝트로 변환하려면 문제 이름을 클릭하고 **[!UICONTROL 자세히]** 메뉴 ![](assets/more-icon.png) 문제 이름의 오른쪽에 있는 를 클릭한 다음 **[!UICONTROL 빈 프로젝트로 변환]**.


      또는

      문제 목록에서 문제를 선택하고 **[!UICONTROL 자세히]** 메뉴 ![](assets/more-icon.png) 목록의 맨 위에서 을 클릭합니다. **[!UICONTROL 빈 프로젝트로 변환]**.

      >[!IMPORTANT]
      >
      >빈 프로젝트로 변환 옵션은 시스템 또는 그룹 관리자가 [!UICONTROL 템플릿을 사용하지 않고 프로젝트를 만들 수 있도록 허용] 기본 설정 [!UICONTROL 설정] 영역. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


      문제를 변환한 후 프로젝트에 작업을 수동으로 추가하거나 템플릿을 프로젝트에 첨부해야 합니다.

      아래의 3e 단계를 계속 진행합니다.

      <!--
     Is this accurate?
     -->

      >[!TIP]
      >   
      >* 요청 큐를 사용하여 문제를 만든 경우 새 프로젝트는 요청 큐의 그룹을 상속합니다.
      >* 프로젝트의 Issues 섹션에 해당 문제를 추가하여 만든 경우 새 프로젝트는 문제의 프로젝트가 있는 경우 Group을 상속합니다.


   * 템플릿을 사용하여 문제를 프로젝트로 변환하려면 다음 중 하나를 수행합니다.

      * 문제 이름을 클릭한 다음 [!UICONTROL **자세히**] 메뉴 ![](assets/more-icon.png) 문제 이름의 오른쪽에 있습니다.

         ![](assets/issue-more-menu-expanded-with-convert-to-project-options-nwe-350x213.png)

         또는

      * 문제 목록, 보고서 또는 대시보드에서 문제를 선택합니다. **자세히** 메뉴 ![](assets/more-icon.png) 목록의 맨 위에서 을 클릭합니다. **템플릿에서 프로젝트로 변환** 템플릿 이름을 입력한 다음 **검색 템플릿** 상자를 클릭한 다음 목록에 표시될 때 템플릿의 이름을 클릭합니다. 3단계를 계속 진행합니다.

         <!--      
        (is this accurate?)      
        -->
      >[!TIP]
      >
      >즐겨찾기 목록에 템플릿을 추가하면 [!UICONTROL **즐겨찾는 템플릿**] 메뉴를 클릭하고 사용할 템플릿을 클릭합니다.

      템플릿에서 새 프로젝트 상자가 표시됩니다.

      ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

      >[!TIP]
      >
      >문제가 승인 프로세스와 연결되어 있거나 이미 해결 객체와 연결되어 있는 경우 Workfront은 [프로젝트로 변환] 상자 맨 위에 경고를 표시하여 승인 작업이 제거되거나 변환 중에 해결 객체를 덮어쓰게 됨을 알려줍니다. 자세한 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).


1. (조건부) 템플릿을 사용하여 문제를 프로젝트로 전환하도록 선택한 경우 다음 단계를 계속 수행하십시오.

   1. 오른쪽에 있는 템플릿 세부 사항을 검토합니다.

      템플릿 세부 정보에는 다음이 포함됩니다.

      * 템플릿 기간
      * 템플릿 소유자
      * 상위 3개 작업의 이름이 포함된 최상위 수준의 작업 수입니다
      * 템플릿에 있는 모든 작업의 수입니다
      * 템플릿 사용자 지정 양식의 이름
   1. (선택 사항) 템플릿 이름 위로 마우스를 가져간 후 즐겨찾기 아이콘을 클릭합니다 ![](assets/favorites-icon-small.png) 나중에 사용하기 위해 즐겨찾기로 표시합니다.

      >[!TIP]
      >
      >최대 40개의 Workfront 항목을 즐겨찾기로 표시할 수 있습니다. 여기에는 템플릿 및 기타 항목이 포함됩니다.

   1. 클릭 [!UICONTROL **템플릿 사용**] 템플릿을 선택하려면 다음을 수행하십시오.

      다음 [!UICONTROL 프로젝트로 변환] 상자가 열립니다.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. 템플릿에 필드가 이미 채워져 있는 경우 해당 필드는에서 미리 채워집니다. [!UICONTROL 프로젝트로 변환] 상자. 미리 채워진 값을 편집하여 프로젝트와 더 잘 일치시킬 수 있습니다. 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* 시스템 또는 그룹 관리자는 [!UICONTROL 프로젝트로 변환 상자] 프로젝트 세부 사항 정보를 [!UICONTROL 레이아웃 템플릿].
      >
      >* 에서 필드를 업데이트하려면 [!UICONTROL 재무] 의 섹션 [!UICONTROL 프로젝트로 변환] 상자에 [!UICONTROL 편집] 액세스 [!UICONTROL 재무 데이터] 액세스 수준에서 만약 [!UICONTROL 보기] 액세스 [!UICONTROL 재무 데이터] 액세스 수준에서 템플릿의 모든 재무 정보가 새 프로젝트로 전송되며 문제를 변환하는 동안에는 편집할 수 없습니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 및 [템플릿 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).


   1. (선택 사항 및 조건부) [!UICONTROL **옵션**] 왼쪽 패널에서 사용 가능한 옵션 중에서 선택합니다.

      * [!UICONTROL **원래 문제를 유지하고 이 프로젝트에 해결 방법을 연결합니다**]

         선택을 취소하면 원래 문제가 삭제됩니다.

         >[!NOTE]
         >
         >문제에 대한 액세스 권한 또는 삭제 권한이 없는 사용자는 이 설정의 상태에 관계없이 변환 중인 문제를 삭제할 수 없습니다. 문제에 대한 액세스 및 권한에 대한 자세한 내용은 다음을 참조하십시오.
         >
         >* [문제에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
         > 
         >* [문제 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


      * [!UICONTROL **이 프로젝트에 액세스할 수 있도록 허용(사용자 이름)**]

         선택하지 않으면 문제가 [!UICONTROL 기본 연락처] 새 작업에 액세스할 수 없습니다.

         >[!NOTE]
         >
         >여기에서 사용할 수 있는 옵션은 Workfront 관리자가 시스템의 모든 사용자 또는 그룹에 대해 이러한 옵션을 구성한 방법에 따라 다릅니다. 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
         >
         >
         >또는 조직의 최상위 그룹이 별도로 구성한 경우 여기에서 사용할 수 있는 옵션은 6단계에서 새 프로젝트에 대해 선택한 그룹에 따라 다릅니다. 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).
   1. 클릭 [!UICONTROL **사용자 지정 Forms**] 다음을 수행합니다.

      * 템플릿에 첨부된 사용자 지정 양식을 검토합니다. 그들은 새 프로젝트로 이전할 것이다.
      * 모든 필수 필드에 올바른 정보가 있는지 확인하십시오.
      * 사용자 지정 양식을 드래그하여 다시 배치합니다 ![](assets/drag-object-icon.png) 원하는 곳에
      * 을(를) 클릭합니다. **x** 아이콘 을 클릭하여 프로젝트에 전송하지 않을 양식의 오른쪽에 있습니다.
      * 필요한 경우 문제의 사용자 지정 양식 정보를 프로젝트로 전송합니다.

         >[!TIP]
         >
         >* 문제에 첨부된 다중 개체 사용자 지정 양식이 문제와 프로젝트에서 모두 사용하도록 구성된 경우 양식에 저장된 모든 정보는 변환 시 유지됩니다.
         >
         >* 변환에 템플릿을 사용하고 템플릿에 첨부된 사용자 지정 양식에 사용자 지정 필드도 포함되어 있는 경우 문제에 첨부된 사용자 지정 양식에서도 문제 필드의 값이 새 프로젝트에 사용됩니다. 하지만 문제에 사용자 지정 필드가 비어 있으면 템플릿의 값이 사용됩니다.

   1. 클릭 [!UICONTROL **프로젝트로 변환**].

      >[!TIP]
      >
      >원래 문제를 삭제하기로 결정한 경우 이제 문제가 프로젝트입니다.
      >   
      >또는
      >  
      >원래 문제를 유지하기로 결정한 경우, 이제 문제가 새 프로젝트에 연결되며 프로젝트가 완료되면 완료됩니다.
      >
      >일부 문제 필드가 프로젝트로 전송됩니다. 템플릿에 정의된 대부분의 필드는 이전 단계에서 변경하지 않은 경우 새로 만든 프로젝트로 자동으로 전송됩니다. 자세한 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).




1. (선택 사항) 프로젝트 세부 사항&#x200B;(프로젝트 소유자, 프로젝트 날짜) 및 작업을 필요에 따라 설정합니다.
1. 클릭 [!UICONTROL **프로젝트로 변환**].

   이제 문제가 프로젝트로 변환됩니다.

1. 클릭 [!UICONTROL **프로젝트로 이동**] 내부 [!UICONTROL 성공] 페이지의 오른쪽 위 모서리에 있는 알림입니다. 그러면 프로젝트 페이지가 열립니다.
