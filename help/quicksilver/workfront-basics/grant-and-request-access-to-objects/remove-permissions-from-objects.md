---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: 개체에서 권한 제거
description: 공유 액세스 권한이 있는 개체에 대한 다른 사용자의 권한을 제거할 수 있습니다. 객체에서 사용 권한을 제거하는 것은 공유할 수 있는 모든 객체에 대해 동일합니다.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# 개체에서 권한 제거

공유 액세스 권한이 있는 개체에 대한 다른 사용자의 권한을 제거할 수 있습니다. 객체에서 사용 권한을 제거하는 것은 공유할 수 있는 모든 객체에 대해 동일합니다. 

객체 공유와 유사한 고려 사항은 객체에서 사용 권한을 제거하는 데 적용됩니다. 자세한 내용은 섹션을 참조하십시오 [개체 공유에 대한 고려 사항](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) 기사 [개체에 대한 권한 공유 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or  
   <p>Legacy license: Request or higher</p>
   <p><b>NOTE</b></p>

   <p>Some objects require a higher access than Request. </p>
   
   <p>For example, for the current license, a Contributor can share issues, but only Standard-license users can share a project.</p>
   
   <p>For the legacy license, a Requestor can share issues, but only Workers or Planners can share a project.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>Manage permissions to remove inherited permissions on objects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

객체를 공유하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 라이선스*</td> 
   <td> <p>요청 이상</p>
   <p><b>메모</b></p>

일부 개체에는 요청보다 높은 액세스 권한이 필요합니다. 예를 들어 요청자는 문제를 공유할 수 있지만 작업자 또는 계획자만 프로젝트를 공유할 수 있습니다.

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>공유할 개체에 대한 액세스 이상의 보기</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>공유할 개체에 대한 권한 보기 이상</p> <p>객체에 대한 상속된 권한을 제거하는 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 개체의 공유 목록에서 엔티티를 제거합니다 {#remove-entities-from-the-sharing-list-of-an-object}

개체의 공유 목록에서 엔터티(사용자, 작업 역할, 팀, 그룹, 회사)를 제거할 수 있습니다. 그러면 객체에 대한 사용 권한이 제거됩니다.

1. 공유할 개체로 이동합니다.

   공유할 수 있는 객체에 대한 자세한 내용은 [개체에 대한 권한 공유 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 을(를) 클릭합니다. **자세히** 아이콘 ![](assets/more-icon.png)개체 이름 옆에 있는 를 클릭한 다음 **공유** 또는&#x200B;**공유.**

   ![](assets/share-a-document-350x160.png)

1. 을(를) 클릭합니다. **x** 객체 액세스 상자에서 제거할 사용자, 팀, 그룹, 회사, 작업 역할 이름 옆에 있습니다.

   ![](assets/remove-permissions-on-project-nwe-350x479.png)

1. 에서 `<User Name>`이 드롭다운 메뉴에서 의 Workfront 액세스가 제거되고, 선택한 객체에서만 해당 액세스를 제거할지 또는 해당 액세스와 연관된 모든 하위 객체에서 제거할지 선택합니다.\
   다음 시나리오가 있습니다.

   * 객체에서만 엔티티를 제거하면 해당 엔티티가 객체에 대한 사용 권한을 상실하고 자식 객체에 대한 상속된 사용 권한을 잃게 됩니다. 이전에 1차 하위 구성요소 항목에 대한 권한을 개별적으로 부여받은 경우, 이 옵션을 선택하면 1차 하위 구성요소 객체와 연관된 모든 1차 하위 구성요소 객체에 대해 동일한 권한을 유지합니다. 
   * 개체와 모든 하위 개체에서 엔티티를 제거하면 이전에 각 하위 개체에 대해 개별 권한이 부여된 경우에도 해당 엔티티는 개체와 모든 하위 개체에 대한 사용 권한을 잃게 됩니다. 

1. **저장**&#x200B;을 클릭합니다.

## 여러 개체에서 권한을 일괄적으로 제거합니다

목록에서 항목을 벌크 선택할 때 여러 객체에서 엔티티(사용자, 작업 역할, 팀, 그룹, 회사)를 제거할 수 있습니다. 

>[!NOTE]
>
>일괄 선택할 때 선택한 모든 객체에 대해 액세스 엔티티를 볼 수 없습니다. 사용 권한을 제거하기 전에 선택한 개체의 공유에서 제거할 엔터티를 알고 있어야 합니다.

1. 공유할 개체 목록으로 이동합니다.

   공유할 수 있는 객체에 대한 자세한 내용은 [개체에 대한 권한 공유 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 목록에서 여러 개체를 선택한 다음 **공유** 아이콘 ![](assets/share-icon.png)를 클릭합니다.
1. 에서 액세스를 제거할 사용자, 역할, 팀, 그룹 또는 회사의 이름을 입력합니다 **편집 `<Object Name>` 액세스** 필드.
1. 액세스 드롭다운 메뉴에서 **액세스 권한 없음**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. 에서 `<User Name>`이 드롭다운 메뉴에서 의 Workfront 액세스가 제거되고, 선택한 객체에서만 해당 액세스를 제거할지 또는 해당 액세스와 연결된 다른 모든 하위 객체에서 제거할지 선택합니다.\
   다음 시나리오가 있습니다.

   * 객체에서만 엔티티를 제거하면 해당 엔티티가 객체에 대한 사용 권한을 상실하고 자식 객체에 대한 상속된 사용 권한을 잃게 됩니다. 이전에 1차 하위 구성요소 항목에 대한 권한을 개별적으로 부여받은 경우, 이 옵션을 선택하면 1차 하위 구성요소 객체와 연관된 모든 1차 하위 구성요소 객체에 대해 동일한 권한을 유지합니다. 
   * 개체와 모든 하위 개체에서 엔티티를 제거하면 이전에 각 하위 개체에 대해 개별 권한이 부여된 경우에도 해당 엔티티는 개체와 모든 하위 개체에 대한 사용 권한을 잃게 됩니다.

   **예:** 목록에서 선택한 작업에 대한 사용 권한을 제거할지, 작업에 첨부된 문제 및 문서에 대해서도 제거 여부를 선택합니다.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (선택 사항) 여러 객체에 대한 권한을 일괄적으로 변경하려면 선택한 엔티티에 대해 다른 공유 레벨을 선택합니다.

   예를 들어, 관리자 권한이 있는 경우 대신 Contribute 또는 보기를 선택합니다.

1. **저장**&#x200B;을 클릭합니다.

## 상속된 권한 제거

상속된 권한은 객체에서 제거될 수 있으므로, 사용자는 상위 객체에 대한 사용자의 액세스와 관계없이 하위 객체에 액세스할 사용자를 구체적으로 식별할 수 있습니다.

>[!IMPORTANT]
>
>관리 권한이 있는 사용자만 상속된 권한을 제거할 수 있습니다.

상속된 권한을 제거하려면

1. 관리 권한이 있는 개체로 이동합니다. 예를 들어 작업으로 이동합니다.
1. 에 설명된 대로 개체 액세스 상자로 이동합니다. [개체의 공유 목록에서 엔티티를 제거합니다](#remove-entities-from-the-sharing-list-of-an-object) 섹션에 자세히 설명되어 있습니다.
1. 을(를) 선택합니다 **x** 다음 **상속된 권한** 공유 상자에 나열된 모든 사용자를 제거합니다.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   따라서 상위 개체(예: 프로젝트)에 대한 권한을 부여받은 사람은 기본적으로 이 작업에 대한 권한을 가지고 있지 않습니다. 작업에 대한 권한을 부여하려면 작업의 공유 목록에 개별 개체를 나열해야 합니다.

   >[!TIP]
   >
   >상속된 권한 목록에서 개별 엔티티를 제거할 수 없습니다. 나열된 모든 엔티티에 대해 상속된 권한만 비활성화할 수 있습니다.

1. 클릭 **저장**. 

## 개체를 비공개로 만들기

객체 시스템 전체를 공유했거나, 객체 시스템을 공개하여 외부 사용자와 공유한 경우 시스템 전체 또는 공용 권한을 제거하여 다시 비공개로 만들 수 있습니다. 

객체 사용 가능 또는 공개에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

객체를 비공개로 만들려면

1. 비공개로 만들 개체로 이동합니다.\
   예를 들어, 보고서로 이동합니다.
1. 클릭 **보고서 작업**, 그런 다음 **공유**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. 클릭 **공개 액세스 제거** 보고서를 볼 외부 사용자의 액세스를 제거하려면 다음을 수행하십시오.
1. 클릭 **시스템 전체 액세스 제거** 모든 Workfront 사용자와의 공유를 중지하려면 다음을 수행하십시오. 
1. **저장**&#x200B;을 클릭합니다.
