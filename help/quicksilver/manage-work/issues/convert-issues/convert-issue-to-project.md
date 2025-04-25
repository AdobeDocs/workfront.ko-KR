---
product-area: projects
navigation-topic: convert-issues
title: Adobe Workfront에서 문제를 프로젝트로 전환
description: Adobe Workfront에서 문제를 프로젝트로 전환
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1975'
ht-degree: 1%

---

# Adobe Workfront에서 문제를 프로젝트로 전환

<!--Audited: 01/2024-->

문제가 제출된 후 문제를 완료하기 위해 추가 작업을 수행해야 하는 경우 문제를 프로젝트로 전환할 수 있습니다.

문제를 새 프로젝트로 전환하거나 템플릿을 사용하여 프로젝트로 전환할 수 있습니다. 이 문서에서는 문제를 프로젝트로 변환하는 두 가지 방법에 대해 설명합니다.

>[!IMPORTANT]
>
>문제 전환에 대한 일반적인 정보를 보려면 문서 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)도 읽어보시기 바랍니다.

문제에서 프로젝트를 만들 때 프로젝트의 일부 필드가 다른 오브젝트에서 채워집니다. 자세한 내용은 문서 [프로젝트 만들기](../../../manage-work/projects/create-projects/create-project.md)의 &quot;새 프로젝트 기본 설정&quot; 섹션을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준 </p> 
    <p>현재: 플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제, 작업 및 프로젝트에 대한 액세스 편집</p> <p>재무 데이터에 대한 액세스를 편집하여 문제에서 전환된 예상 재무 정보를 업데이트합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 보기</p> <p>문제가 전환된 후 프로젝트에 대한 관리 권한을 받습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 문제를 프로젝트로 전환

문제를 빈 프로젝트로 전환할 수 있습니다.

1. 프로젝트로 이동한 다음 왼쪽 패널에서 **[!UICONTROL 문제]**&#x200B;를 클릭합니다.
1. 표시되는 문제 목록에서 다음 중 하나를 수행합니다.

   * 문제를 빈 프로젝트로 전환하려면 문제 이름을 클릭하고 문제 이름 오른쪽에 있는 **[!UICONTROL 기타]** 메뉴 ![기타 메뉴](assets/more-icon.png)를 클릭한 다음 **[!UICONTROL 빈 프로젝트로 전환]**&#x200B;을 클릭합니다.


     또는

     문제 목록에서 문제를 선택하고 목록 맨 위에 있는 **[!UICONTROL 자세히]** 메뉴 ![추가 메뉴](assets/more-icon.png)를 클릭한 다음 **[!UICONTROL 빈 프로젝트로 전환]**&#x200B;을 클릭합니다.

     >[!IMPORTANT]
     >
     >빈 프로젝트로 전환 옵션은 시스템 또는 그룹 관리자가 [!UICONTROL 설정] 영역에서 [!UICONTROL 사용자가 템플릿을 사용하지 않고 프로젝트를 만들 수 있도록 허용] 기본 설정을 사용하도록 설정한 경우에만 표시됩니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.


     문제를 전환한 후 프로젝트에 작업을 수동으로 추가하거나 프로젝트에 템플릿을 첨부해야 합니다.

     >[!TIP]
     >   
     >* 요청 대기열을 사용하여 문제를 만든 경우 새 프로젝트가 요청 대기열의 그룹을 상속합니다.
     >* 문제를 프로젝트의 문제 섹션에 추가하여 만든 경우 새 프로젝트가 문제의 프로젝트 그룹을 상속합니다.

     >[!TIP]
     >
     >문제가 승인 프로세스와 연결되어 있거나 이미 해결 중인 오브젝트와 연결되어 있는 경우 Workfront은 프로젝트로 전환 상자 맨 위에 경고를 표시하여 승인이 제거되거나 전환 중 해결 중인 오브젝트가 덮어쓰기됨을 알립니다. 자세한 내용은 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)를 참조하십시오.

1. (선택 사항 및 조건부) 왼쪽 패널에서 [!UICONTROL **옵션**]&#x200B;을 클릭한 다음 사용할 수 있는 옵션 중에서 선택합니다.

   * [!UICONTROL **원래 문제를 유지하고 해결 방법을 이 프로젝트에 연결**]

     선택을 취소하면 원래 문제가 삭제됩니다.

     >[!NOTE]
     >
     >문제를 삭제할 수 있는 액세스 또는 권한이 없는 사용자는 이 설정의 상태에 관계없이 문제를 전환할 때 문제를 삭제할 수 없습니다. 문제에 대한 액세스 및 권한에 대한 자세한 내용은 다음을 참조하십시오.
     >
     >* [문제에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [문제 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **이 프로젝트에 액세스할 수 있도록 허용**]

     선택하지 않으면 문제의 [!UICONTROL 기본 담당자]에게 새 작업에 대한 액세스 권한이 없습니다.

     >[!NOTE]
     >
     >여기에서 사용할 수 있는 옵션은 Workfront 관리자가 시스템의 모든 사용자 또는 그룹에 대해 구성한 방법에 따라 다릅니다. 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.
     >
     >
     >또는 조직의 최상위 그룹이 그룹을 별도로 구성한 경우 여기에서 사용할 수 있는 옵션은 6단계에서 새 프로젝트에 대해 선택한 그룹에 따라 다릅니다. 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)을 참조하십시오.

1. [!UICONTROL **사용자 지정 Forms**]&#x200B;을(를) 클릭하고 다음 중 하나를 수행합니다.

   * 문제에 첨부된 사용자 정의 양식을 검토하십시오. 프로젝트 사용자 정의 양식인 경우 새 프로젝트로 전송됩니다.
   * 더 많은 사용자 정의 양식 추가
   * 모든 필수 필드에 유효한 정보가 있는지 확인하십시오.
   * 사용자 정의 양식을 원하는 위치로 ![드래그 아이콘](assets/drag-object-icon.png)하여 다시 정렬합니다.
   * 프로젝트로 전송하지 않을 양식 오른쪽의 **x** 아이콘을 클릭합니다. 이렇게 하면 프로젝트에서 양식이 제거됩니다.
   * 필요한 경우 문제의 사용자 정의 양식 정보를 프로젝트로 전송합니다.

     >[!TIP]
     >
     >* 문제에 첨부된 다중 오브젝트 사용자 정의 양식이 문제와 프로젝트 모두에서 사용하도록 구성된 경우 해당 문제의 필드와 프로젝트의 사용자 정의 양식 둘 다에 필드가 있는 경우 전환할 때 양식에 저장된 모든 정보가 유지됩니다.
     >* 계산된 필드가 있는 다중 오브젝트 사용자 정의 양식이 문제 및 프로젝트에 첨부된 경우 문제 및 프로젝트는 양식의 계산된 사용자 정의 필드에서 참조되는 모든 필드와 호환되어야 합니다. 비호환성이 있는 경우 조정할 것을 알리는 메시지가 표시됩니다. 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)의 &quot;다중 개체 사용자 정의 양식의 계산된 사용자 정의 필드&quot; 섹션을 참조하십시오.

1. [!UICONTROL **프로젝트로 전환**]&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >원래 문제를 삭제하기로 했다면 이제 문제가 프로젝트가 됩니다.
   >   
   >또는
   >  
   >원래 문제를 유지하기로 결정한 경우 문제가 이제 새 프로젝트에 연결되며 프로젝트가 완료되면 완료됩니다.
   >
   >전환 중에 변경하지 않은 경우 일부 문제 필드의 정보가 프로젝트로 전송됩니다.

1. (선택 사항) 필요에 따라 추가 프로젝트 세부 &#x200B; 정보(프로젝트 소유자, 프로젝트 날짜) 및 작업을 설정합니다.
1. [!UICONTROL **프로젝트로 전환**]&#x200B;을 클릭합니다.

   이제 문제가 프로젝트로 전환됩니다. 프로젝트 페이지가 표시됩니다.

## 템플릿을 사용하여 문제를 프로젝트로 전환

템플릿을 사용하여 문제를 프로젝트로 전환할 수 있습니다.

1. 프로젝트로 이동한 다음 왼쪽 패널에서 **[!UICONTROL 문제]**&#x200B;를 클릭합니다.
1. 표시되는 문제 목록에서 문제 이름을 클릭하고 문제 이름 오른쪽에 있는 **[!UICONTROL 자세히]** 메뉴 ![추가 메뉴](assets/more-icon.png)를 클릭한 다음 **템플릿에서 프로젝트로 전환**&#x200B;을 클릭하고 **템플릿 검색** 상자에 템플릿 이름을 입력한 다음 목록에 표시될 때 템플릿 이름을 클릭합니다. 3단계를 계속 진행합니다.

   >[!TIP]
   >
   >즐겨찾기 목록에 템플릿을 추가한 경우 [!UICONTROL **즐겨찾기 템플릿**] 메뉴 위로 마우스를 가져간 후 사용할 템플릿을 클릭할 수 있습니다.

   템플릿의 새 프로젝트 상자가 표시됩니다.

   ![템플릿의 새 프로젝트](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* 문제가 승인 프로세스와 연결되어 있거나 이미 해결 중인 오브젝트와 연결되어 있는 경우 Workfront은 프로젝트로 전환 상자 맨 위에 경고를 표시하여 승인이 제거되거나 전환 중 해결 중인 오브젝트가 덮어쓰기됨을 알립니다. 자세한 내용은 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)를 참조하십시오.
   >   
   >* 요청 대기열을 사용하여 문제를 만든 경우 새 프로젝트가 요청 대기열의 그룹을 상속합니다.
   >* 문제를 프로젝트의 문제 섹션에 추가하여 만든 경우 새 프로젝트가 문제의 프로젝트 그룹을 상속합니다.

1. 오른쪽의 템플릿 세부 사항을 검토합니다.

   템플릿 세부 정보에는 다음 항목이 포함됩니다.

   * 템플릿 기간
   * 템플릿 소유자
   * 상위 3개 작업의 이름을 포함하는 최상위 작업 수
   * 템플릿의 모든 작업 수
   * 템플릿 사용자 정의 양식의 이름

1. (선택 사항) 템플릿 이름 위로 마우스를 가져간 후 **즐겨찾기** 아이콘 ![즐겨찾기](assets/favorites-icon-small.png)를 클릭하여 나중에 사용할 수 있도록 즐겨찾기로 표시합니다.

   >[!TIP]
   >
   >최대 40개의 Workfront 항목을 즐겨찾기로 표시할 수 있습니다. 여기에는 템플릿 및 기타 항목이 포함됩니다.

1. 템플릿을 선택하려면 [!UICONTROL **템플릿 사용**]&#x200B;을 클릭하세요.

   [!UICONTROL 프로젝트로 전환] 상자가 열립니다.

   ![프로젝트로 전환](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. 템플릿에 필드가 이미 채워져 있으면 [!UICONTROL 프로젝트로 전환] 상자에서 필드가 미리 채워집니다. 프로젝트와 더 잘 일치하도록 미리 채워진 값을 편집할 수 있습니다. 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

   >[!TIP]
   >
   >* 시스템 또는 그룹 관리자는 [!UICONTROL 레이아웃 템플릿]에서 프로젝트 세부 정보를 업데이트하여 [!UICONTROL 프로젝트로 전환]의 필드를 추가하거나 제거할 수 있습니다.
   >
   >* [!UICONTROL 프로젝트로 전환] 상자에서 [!UICONTROL 재무] 섹션의 필드를 업데이트하려면 액세스 수준에서 [!UICONTROL 재무 데이터]에 대한 [!UICONTROL 편집] 액세스 권한이 있어야 합니다. 액세스 수준에서 [!UICONTROL 재무 데이터]에 대한 [!UICONTROL 보기] 액세스 권한이 있는 경우 템플릿의 모든 재무 정보가 새 프로젝트로 전송되며 문제를 전환하는 동안 이를 편집할 수 없습니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 및 [템플릿 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)를 참조하십시오.

1. (선택 사항 및 조건부) 왼쪽 패널에서 [!UICONTROL **옵션**]&#x200B;을 클릭한 다음 사용할 수 있는 옵션 중에서 선택합니다.

   * [!UICONTROL **원래 문제를 유지하고 해결 방법을 이 프로젝트에 연결**]

     선택을 취소하면 원래 문제가 삭제됩니다.

     >[!NOTE]
     >
     >문제를 삭제할 수 있는 액세스 또는 권한이 없는 사용자는 이 설정의 상태에 관계없이 문제를 전환할 때 문제를 삭제할 수 없습니다. 문제에 대한 액세스 및 권한에 대한 자세한 내용은 다음을 참조하십시오.
     >
     >* [문제에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [문제 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **이 프로젝트에 액세스할 수 있도록 허용**]

     선택하지 않으면 문제의 [!UICONTROL 기본 담당자]에게 새 작업에 대한 액세스 권한이 없습니다.

     >[!NOTE]
     >
     >여기에서 사용할 수 있는 옵션은 Workfront 관리자가 시스템의 모든 사용자 또는 그룹에 대해 구성한 방법에 따라 다릅니다. 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.
     >
     >
     >또는 조직의 최상위 그룹이 그룹을 별도로 구성한 경우 여기에서 사용할 수 있는 옵션은 6단계에서 새 프로젝트에 대해 선택한 그룹에 따라 다릅니다. 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)을 참조하십시오.

   1. [!UICONTROL **사용자 지정 Forms**]&#x200B;을(를) 클릭하고 다음 중 하나를 수행합니다.

      * 템플릿에 첨부된 사용자 정의 양식을 검토하십시오. 그들은 새 프로젝트로 이전할 것이다.
      * 문제에 첨부된 사용자 정의 양식을 검토하십시오. 프로젝트 양식인 경우 프로젝트로 전송됩니다.
      * 모든 필수 필드에 유효한 정보가 있는지 확인하십시오.
      * 사용자 정의 양식을 원하는 위치로 ![드래그 아이콘](assets/drag-object-icon.png)하여 다시 정렬합니다.
      * 프로젝트로 전송하지 않을 양식 오른쪽의 **x** 아이콘을 클릭합니다.
      * 필요한 경우 문제의 사용자 정의 양식 정보를 프로젝트로 전송합니다.

        >[!TIP]
        >
        >* 문제에 첨부된 다중 오브젝트 사용자 정의 양식이 문제와 프로젝트 모두에서 사용하도록 구성된 경우 해당 문제의 필드와 프로젝트의 사용자 정의 양식 둘 다에 필드가 있는 경우 전환할 때 양식에 저장된 모든 정보가 유지됩니다.
        >* 계산된 필드가 있는 다중 오브젝트 사용자 정의 양식이 문제 및 프로젝트에 첨부된 경우 문제 및 프로젝트는 양식의 계산된 사용자 정의 필드에서 참조되는 모든 필드와 호환되어야 합니다. 비호환성이 있는 경우 조정할 것을 알리는 메시지가 표시됩니다. 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.
        >* 템플릿에 첨부된 사용자 정의 양식에 문제에 첨부된 사용자 정의 양식에서도 사용자 정의 필드가 포함된 경우 문제의 필드 값이 새 프로젝트에 사용됩니다. 하지만, 해당 문제에 대한 사용자 정의 필드가 비어 있는 경우, 템플릿의 값이 사용됩니다.

1. (선택 사항) 필요에 따라 추가 프로젝트 세부 &#x200B; 정보(프로젝트 소유자, 프로젝트 날짜) 및 작업을 설정합니다.

   1. [!UICONTROL **프로젝트로 전환**]&#x200B;을 클릭합니다.

      >[!TIP]
      >
      >원래 문제를 삭제하기로 했다면 이제 문제가 프로젝트가 됩니다.
      >   
      >또는
      >  
      >원래 문제를 유지하기로 결정한 경우 문제가 이제 새 프로젝트에 연결되며 프로젝트가 완료되면 완료됩니다.
      >
      >일부 문제 필드가 프로젝트로 전송됩니다. 이전 단계에서 변경하지 않은 경우 템플릿에 정의된 대부분의 필드가 새로 생성된 프로젝트로 자동으로 전송됩니다. 자세한 내용은 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)를 참조하십시오.

   이제 문제가 프로젝트로 전환됩니다. 프로젝트 페이지가 표시됩니다.
