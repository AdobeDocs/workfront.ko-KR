---
title: 사용자 지정 양식 공유
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 사용자 정의 양식에 대한 액세스를 구성하여 개인, 역할, 그룹, 팀, 회사 등의 사용자가 보고, 공유하고 편집할 수 있도록 제어할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 1%

---

# 사용자 지정 양식 공유

사용자 정의 양식에 대한 액세스를 구성하여 개인, 역할, 그룹, 팀, 회사 등의 사용자가 보고, 공유하고 편집할 수 있도록 제어할 수 있습니다.

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
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유한 계획, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 지정 양식에 대한 액세스 {#access-to-custom-forms}

기본적으로 새 사용자 지정 양식을 만들고 다른 사용자가 객체에 첨부하면 객체에 할당된 모든 사용자가 양식을 보고 작성할 수 있습니다. 여기에는 라이선스 요청 및 외부 사용자가 포함됩니다.

그러나 사용자 정의 양식이 아직 첨부되어 있지 않은 객체에서는 다음 중 하나가 true가 아니면 사용자(계획자 액세스 레벨이 있는 경우에도) 사용자 정의 Forms 드롭다운 메뉴에서 이를 첨부할 수 없습니다.

* 사용자 지정 양식을 사용자 또는 해당 팀, 작업 역할, 그룹 또는 회사와 공유했으며, 사용자 지정 데이터에 첨부 를 선택한 상태로 보기 권한 이상을 부여합니다
* 사용자에게 계획 라이센스가 있고 액세스 수준에서는 사용자 지정 양식에 대한 관리자 액세스를 허용합니다

## 사용자 지정 양식 공유

사용자 지정 양식을 기본 공유 상태(에 설명)로 두지 않고 [사용자 지정 양식에 대한 액세스](#access-to-custom-forms) (이 문서에서) 특정 사용자, 작업 역할, 그룹, 팀 및 회사에 대해 양식에 대한 특정 액세스 수준을 구성할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **사용자 지정 Forms**.
1. 사용자 지정 양식을 선택한 다음 **공유**.
1. 표시되는 상자에서 다음을 수행합니다 **사용자 지정 양식 액세스 권한 제공**&#x200B;를 클릭하고 사용자 지정 양식을 공유할 사용자, 팀, 작업 역할, 그룹 또는 회사의 이름을 입력한 다음 키를 누릅니다 **Enter 키** 가 표시되는 경우입니다.
1. 방금 추가한 사용자, 팀, 작업 역할, 그룹 또는 회사에 대한 액세스를 조정하려면 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 사용 가능한 다음 옵션 중 하나와 고급 설정 중 하나를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">보기</td> 
      <td> <p>개체에서 사용자 지정 양식을 보고 채우는 기능</p> <p><b>참고</b>: 작업, 검토 및 요청 라이선스가 있는 사용자의 경우 이 옵션이 가장 높은 옵션입니다.</p> <p>클릭 <strong>고급 설정</strong> 다음을 허용할지 여부를 지정합니다.</p> 
       <ul> 
        <li><strong>사용자 지정 데이터에 첨부</strong>: 사용자 정의 양식을 프로젝트, 작업 및 관리 액세스 권한이 있는 문제에 연결할 수 있습니다</li> 
        <li> <p><strong>공유</strong>: 시스템의 다른 사용자와 사용자 지정 양식을 공유하는 기능</p> <p>작업, 검토 또는 요청 라이센스가 있는 사용자는 API 또는 사용자 지정 양식 보고서를 통해서만 사용자 지정 양식을 공유할 수 있습니다. 자세한 내용은 를 참조하십시오.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리함</td> 
      <td> <p>계획 라이센스가 있는 사용자만 사용할 수 있습니다. </p> <p>사용자가 편집할 수 있는 액세스 권한이 있는 개체에 양식을 추가할 수 있을 뿐만 아니라 필드 추가, 편집 및 삭제 등 사용자 지정 양식을 완전히 편집할 수도 있습니다.</p> <p>클릭 <strong>고급 설정</strong> 다음을 허용할지 여부를 지정합니다.</p> 
       <ul> 
        <li> <p><strong>사용자 지정 데이터에 첨부</strong>: 사용자 정의 양식을 프로젝트, 작업 및 관리 액세스 권한이 있는 문제에 연결할 수 있습니다</p> </li> 
        <li><strong>삭제</strong>: 시스템에서 사용자 지정 양식 삭제</li> 
        <li><strong>공유</strong>: 시스템의 다른 사용자와 사용자 지정 양식을 공유합니다</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 4-5단계를 반복하여 목록에 다른 이름을 추가하고 해당 옵션을 구성합니다.
1. (선택 사항) 사용자 지정 양식(첨부 객체)에 대한 액세스를 이전 단계에서 지정한 양식으로 제한하려면 톱니바퀴 아이콘을 클릭합니다 ![](assets/gear-icon-settings-with-dn-arrow.jpg) 공유 상자의 오른쪽 상단 모서리에서 을(를) 클릭하고 **시스템 전체 액세스 제거**.

   마음이 바뀌면 **시스템 전체에 표시** (기본 옵션)

   >[!NOTE]
   >
   >* 사용자 정의 양식을 시스템 전체에 표시할 때 사용자는 다른 객체에 첨부하지 않고 할당된 객체를 보고 채울 수만 있습니다. 5단계에서 설명한 &quot;사용자 지정 데이터에 첨부&quot; 옵션을 사용하여 개체에 사용자 지정 양식을 첨부하는 기능을 부여할 수 있습니다.
   >* 대부분의 조직에서는 시스템 내의 모든 사용자가 사용자 정의 양식을 작성하면서 작업 중인 객체에 연결하여 보고서에서 해당 데이터를 볼 수 있도록 해야 합니다. 조직에 대해 true인 경우에는 &quot;**시스템 전체에 표시**.&quot; 이 방법으로 옵션을 구성하면 대화 상자에 &quot;Visible System-Wide&quot;가 표시됩니다.

   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >특정 객체에 첨부된 경우 사용자가 중요한 데이터를 입력할 수 있는 사용자 지정 양식이 걱정되는 경우 해당 객체에 대한 공유를 제한합니다 *개체* 양식 자체에 대한 액세스를 제한하는 것보다 더 나을 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

## 사용자 지정 양식에 대한 액세스 제거

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **사용자 지정 Forms**.
1. 사용자 지정 양식을 선택한 다음 **공유**.
1. 표시되는 상자에서 더 이상 양식에 액세스할 수 없는 사용자, 팀, 역할, 그룹 또는 회사 이름의 오른쪽에 있는 X를 클릭합니다.
1. (선택 사항) 제거할 다른 이름에 대해 이전 단계를에 반복합니다.
1. **저장**&#x200B;을 클릭합니다.
