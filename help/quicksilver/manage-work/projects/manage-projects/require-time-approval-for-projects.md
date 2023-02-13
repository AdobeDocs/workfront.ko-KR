---
product-area: projects
navigation-topic: manage-projects
title: 프로젝트 승인 시간 필요
description: 프로젝트 승인 시간 필요
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 프로젝트 승인 시간 필요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

프로젝트에 대해 기록된 시간이 프로젝트 소유자가 승인하도록 프로젝트를 구성할 수 있습니다. 이러한 방식으로 구성된 경우 청구 레코드에 사용할 수 있으려면 먼저 프로젝트 소유자가 시간을 승인해야 합니다.\
청구 레코드에 대한 자세한 내용은 문서를 참조하십시오 [청구 레코드 만들기](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>이 옵션을 활성화해도 작업표에서 시간을 승인할 수 있는 승인자의 기능이 제거되지 않습니다. 프로젝트 소유자가 시간을 승인하거나 거부하지 않는 경우 작업표 승인자가 작업표의 시간을 계속 승인할 수 있습니다.

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
   <td> <p>프로젝트에 대해 승인해야 하는 시간 계획</p>
   <p>프로젝트에 로그온한 시간을 승인하려면 더 이상 검토</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 이상에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 이상에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">추가 액세스</td> 
   <td> <p>프로젝트에 대한 시간을 승인하려면 다음 조건 중 하나 이상을 충족해야 합니다.</p> 
    <ul> 
     <li>위에 지정된 액세스 및 권한을 가진 프로젝트 소유자입니다. 이 경우 아래 조건 중 하나가 있으면 다음 작업을 수행할 수 있습니다. 
      <ul>
       <li>프로젝트에 대한 관리 권한이 있는 경우 다른 사용자가 프로젝트에 로그온한 시간을 승인하거나 거부할 수 있습니다.</li>
       <li> 프로젝트에 대한 Contribute 또는 View 액세스 권한이 있는 경우 사용자가 로그인한 시간만 승인하거나 거부할 수 있으며 사용자가 이 시간을 보고하면 사용자가 이 작업을 승인하거나 거부할 수 있습니다.<br></li>
      </ul></li> 
     <li>작업표 및 시간에 대한 관리자 액세스 권한이 있는 계획 라이센스가 있습니다. 이 경우:
      <ul>
       <li>프로젝트에 대해 최소 보기 권한이 있는 시간을 승인하거나 거부할 수 있습니다. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 프로젝트 승인 시간 필요

프로젝트에서 몇 시간 동안 프로젝트 관리자의 승인을 요청하려면

1. 몇 시간 동안 승인이 필요한 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 아이콘 ![](assets/more-icon.png) 프로젝트 이름의 오른쪽에 있는 를 클릭한 다음 **편집**.\
   프로젝트 편집 대화 상자가 표시됩니다.

1. 에서 **프로젝트 설정** 섹션, **이 프로젝트에 대한 승인 시간 필요**.
1. **저장**&#x200B;을 클릭합니다.\
   이제 시간이 기록되고 승인되면 해당 시간이 잠기고 프로젝트 또는 작업표에 입력한 사용자가 변경할 수 없습니다. Workfront 관리자만 기록된 시간을 조정할 수 있습니다.

## 프로젝트의 시간 승인 및 거부

프로젝트 관리자는 작업, 문제 또는 프로젝트에 대해 기록된 시간을 승인하거나 거부할 수 있습니다.

프로젝트 수준에서 시간을 승인해도 시간을 기록한 사용자의 작업표에 영향을 주지 않습니다. 예를 들어, 프로젝트 관리자가 프로젝트의 시간을 승인할 수 있지만, 사용자 또는 작업표 승인자가 작업표를 아직 승인하지 않았습니다. 

로그된 시간에 대한 승인이 필요한 프로젝트를 설정하는 경우, 프로젝트 관리자는 해당 시간을 사용하여 해당 프로젝트에 대한 청구 레코드에 포함시킬 수 있도록 해야 합니다. 청구 레코드 생성에 대한 자세한 내용은 문서를 참조하십시오 [청구 레코드 만들기](../../../manage-work/projects/project-finances/create-billing-records.md).

프로젝트에 대한 시간을 승인하거나 거부하려면

1. 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **시간** 왼쪽 패널의 영역. 이 위치는 **자세히 표시** 영역.

1. 문제, 작업 및 프로젝트에 대해 기록된 시간이 표시되므로 상태가 다음과 같아야 합니다 **제출됨**.\
   시간 항목의 왼쪽에 있는 상자를 클릭하여 승인할 시간을 선택합니다.

1. 클릭 **승인**.\
   시간 상태가 로 변경됩니다 **승인됨**.\
   나중에 승인된 시간을 거부하면 시간 상태가 로 변경됩니다 **승인되지 않음**.\
   승인 시간을 청구 레코드에 포함하면 시간 상태가 **청구됨 및 승인됨**. 청구 레코드에 추가된 시간은 삭제할 수 없습니다. 청구 레코드 생성에 대한 자세한 내용은 문서를 참조하십시오 [청구 레코드 만들기](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (선택 사항) **거부** 프로젝트의 시간 항목을 거부하려면 다음을 수행하십시오.\
   시간 상태가 로 변경됩니다 **거부됨**.
