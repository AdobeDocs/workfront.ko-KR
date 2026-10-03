---
title: 사용자 정의 양식 공유
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 사용자 정의 양식에 대한 액세스 권한을 구성하여 해당 양식을 보고, 공유하고, 편집할 수 있는 사용자를 제어할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
TQID: 'https://experienceleague.adobe.com/gpJQedqcdtjaxvhVuWKgJVpfAPAT2ICSgO6nRFLvimM'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ecee8b1aadd804a45ff0830e04e77981a3269cff
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 2%
---
# 사용자 정의 양식 공유

사용자 정의 양식에 대한 액세스 권한을 구성하여 개인, 역할, 그룹, 팀, 회사, 비즈니스 프로필 등 해당 양식을 보고, 공유하고, 편집할 수 있는 사용자를 제어할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr>  
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 양식에 액세스 {#access-to-custom-forms}

기본적으로 새 사용자 정의 양식을 만들어 다른 사용자가 오브젝트에 첨부하면 해당 오브젝트에 할당된 모든 사용자가 양식을 보고 작성할 수 있습니다. 여기에는 기여자 또는 요청 라이선스를 가진 사용자와 외부 사용자가 포함됩니다.

하지만 사용자 정의 양식이 아직 첨부되지 않은 객체에서는 다음 중 하나가 참이 아니면 사용자가 사용자 정의 Forms 드롭다운 메뉴에서 첨부할 수 없습니다(표준 또는 플래너 액세스 수준이 있는 경우에도).

* 누군가 사용자 정의 양식을 &quot;시스템의 모든 사용자가 보고 첨부할 수 있음&quot;으로 공유했습니다.
* 누군가 사용자 정의 데이터에 첨부 가 선택된 상태로 보기 이상의 권한을 부여한 사용자 또는 해당 팀, 작업 역할, 그룹, 회사 또는 비즈니스 프로필과 사용자 정의 양식을 공유했습니다
* 사용자는 Standard 또는 Plan 라이선스를 보유하고 있으며 액세스 수준을 통해 사용자 정의 양식에 대한 관리자 액세스 권한을 부여받습니다

## 사용자 정의 양식 공유

사용자 정의 양식을 기본 공유 상태([사용자 정의 양식에 대한 액세스](#access-to-custom-forms)에서 설명)로 두는 대신 특정 사용자, 작업 역할, 그룹, 팀, 회사 및 비즈니스 프로필에 대해 양식에 대한 특정 액세스 수준을 구성할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 목록에서 사용자 정의 양식을 선택한 다음 ![공유 아이콘](assets/share-icon.png)을 클릭합니다.

   또는

   사용자 정의 양식을 열거나 새 사용자 정의 양식을 만듭니다. 그런 다음 양식 디자이너의 오른쪽 상단에서 **공유**&#x200B;를 클릭합니다.

1. 공유 상자의 **사용자 정의 양식 액세스 권한 부여**&#x200B;에서 사용자 정의 양식을 공유할 사용자, 팀, 작업 역할, 그룹, 회사 또는 비즈니스 프로필의 이름을 입력한 다음 이름이 표시되면 **Enter**&#x200B;를 누릅니다.
1. 방금 추가한 사용자, 팀, 작업 역할, 그룹, 회사 또는 비즈니스 프로필에 대한 액세스를 조정하려면 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 사용 가능한 다음 옵션 중 하나와 고급 설정을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">보기</td> 
      <td> <p>이 옵션은 개체에서 사용자 정의 양식을 보고 작성하는 기능을 제공합니다. 개체 수준에서 사용자는 <strong>사용자 정의 양식 편집</strong> 고급 설정을 사용하는 적어도 Contribute 액세스 권한을 가지고 있어야 합니다. 예를 들어 양식이 프로젝트에 첨부된 경우 사용자는 해당 프로젝트에 대한 기여 액세스 권한이 있어야 합니다. 그렇지 않으면 양식을 작성할 수 없습니다.</p>

   <p><b>참고</b>: Light 및 Contributor 라이선스가 있는 사용자(또는 작업, 검토 및 요청 라이선스)의 경우 이 옵션을 사용할 수 있습니다.</p> <p>다음을 허용할지 여부를 지정하려면 <strong>고급 설정</strong>을 클릭하십시오.</p> 
       <ul> 
        <li><strong>사용자 정의 데이터에 첨부</strong>: 관리 액세스 권한이 있는 프로젝트, 작업 및 문제에 사용자 정의 양식을 첨부할 수 있습니다.</li> 
        <li> <p><strong>공유</strong>: 사용자 정의 양식을 시스템의 다른 사용자와 공유하는 기능</p> <p>라이트 또는 기여자 라이선스(또는 작업, 검토 또는 요청 라이선스)가 있는 사용자는 API 또는 사용자 정의 양식 보고서를 통해서만 사용자 정의 양식을 공유할 수 있습니다.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리</td> 
      <td> <p>이 옵션은 Standard 또는 Plan 라이선스가 있는 사용자만 사용할 수 있습니다. </p> <p>편집할 수 있는 액세스 권한이 있는 오브젝트에 양식을 추가할 수 있을 뿐만 아니라 필드를 추가, 편집 및 삭제하는 등 사용자 정의 양식을 완전히 편집할 수도 있습니다.</p> <p>다음을 허용할지 여부를 지정하려면 <strong>고급 설정</strong>을 클릭하십시오.</p> 
       <ul> 
        <li> <p><strong>사용자 정의 데이터에 첨부</strong>: 관리 액세스 권한이 있는 프로젝트, 작업 및 문제에 사용자 정의 양식을 첨부할 수 있습니다.</p> </li> 
        <li><strong>삭제</strong>: 시스템에서 사용자 정의 양식을 삭제합니다.</li> 
        <li><strong>공유</strong>: 사용자 정의 양식을 시스템의 다른 사용자와 공유합니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 4-5단계를 반복하여 목록에 다른 이름을 추가하고 해당 옵션을 구성합니다.
1. (선택 사항) 이전 단계에서 지정한 사용자 정의 양식에 대한 액세스를 제한하려면 **액세스 권한이 있는 사용자**&#x200B;의 드롭다운 화살표를 클릭한 다음 **초대된 사용자만 액세스할 수 있음**&#x200B;을 선택합니다.

   마음이 바뀌면 **시스템의 모든 사용자가 볼 수 있음**&#x200B;을 선택할 수 있습니다.

   >[!NOTE]
   >
   >* 사용자 정의 양식을 시스템 전체에 표시할 때 사용자는 다른 오브젝트에 첨부하지 않고 할당된 오브젝트에 대해서만 보고 채울 수 있습니다. 5단계에서 설명한 &quot;사용자 정의 데이터에 첨부&quot; 옵션을 사용하여 사용자 정의 양식을 오브젝트에 첨부할 수 있는 기능을 부여할 수 있습니다.
   >* 대부분의 조직에서는 시스템에서 작업 중인 오브젝트에 사용자 정의 양식을 첨부하고 보고서에서 해당 데이터를 볼 때 모든 사용자가 사용자 정의 양식을 작성할 수 있도록 하고자 합니다. 조직에 대해 true인 경우 **시스템의 모든 사용자가 볼 수 있음**&#x200B;을 사용하는 것이 좋습니다.
   >* **시스템의 모든 사용자가 보고 첨부할 수 있습니다**&#x200B;를 선택하면 모든 사용자가 양식을 다른 개체에 첨부할 수 있습니다.
   >
   >![사용자 정의 양식 공유](assets/share-custom-forms-all-can-attach.png)
   >   
   >사용자 정의 양식을 특정 개체에 첨부할 때 사용자가 중요한 데이터를 입력할 수 있는 경우 양식 자체에 대한 액세스를 제한하는 것보다 해당 *개체*&#x200B;에 대한 공유를 제한하는 것이 더 효과적일 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

## 사용자 정의 양식에 대한 액세스 제거

{{step-1-to-setup}}

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 목록에서 사용자 정의 양식을 선택한 다음 ![공유 아이콘](assets/share-icon.png)을 클릭합니다.
1. 공유 상자에서 양식에 더 이상 액세스하지 않으려는 사용자, 팀, 역할, 그룹, 회사 또는 비즈니스 프로필 이름 오른쪽에 있는 드롭다운 메뉴를 클릭하고 **제거**&#x200B;를 선택합니다.
1. (선택 사항) 제거할 다른 이름에 대해 이전 단계를 반복합니다.
1. **저장**&#x200B;을 클릭합니다.

