---
title: 사용자에게 액세스 권한 부여
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront의 다른 사용자에 대한 사용자 액세스 권한을 정의할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 1%

---


# 사용자에게 액세스 권한 부여

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 액세스 수준을 사용하여 Workfront의 다른 사용자에 대한 사용자 액세스를 정의할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 사용자에 대한 액세스 구성

사용자가 만든 기본 액세스 수준 또는 사용자 지정 액세스 수준을 사용하여 다른 사용자가 보고 편집할 수 있는 정보를 관리할 수 있습니다. 기본 플랜 및 작업 라이선스가 있는 사용자는 다른 사용자의 연락처 정보를 볼 수 있습니다. 다음 사용자 중 한 명이 다른 사용자를 만들고 편집할 수 있습니다.

* Workfront 관리자.

  자세한 내용은 [사용자에게 전체 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)를 참조하십시오.

* 이 문서에 설명된 대로 사용자에게 액세스할 수 있는 기본 플랜 라이선스가 있는 사용자.

  회사 또는 기본 회사의 사용자만 볼 수 있도록 제한된 사용자는 볼 수 있는 사용자만 편집할 수 있습니다. 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

* 다른 사용자의 관리자로 지정된 기본 플랜 라이선스를 가진 사용자.

  액세스 수준의 사용자에 대한 편집 액세스 권한이 부여된 사용자는 자신에게 보고하는 사용자를 관리할 수 있습니다. 사용자 관리에 대한 자세한 내용은 [조직도 보기](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md)를 참조하십시오.

* 사용자를 생성한 기본 플랜 라이선스가 있는 사용자는 자신이 생성한 사용자를 비활성화, 삭제 또는 편집할 수 있습니다. 새 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

## 사용자 정의 액세스 수준을 사용하여 사용자 편집에 대한 사용자 액세스 구성

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 플랜 또는 작업 라이선스가 있는 사용자가 다른 사용자의 프로필을 보는 기능을 변경하려면 다음을 수행하십시오.

   1. ![](assets/gear-icon-settings.png)사용자&#x200B;**오른쪽에 있는**&#x200B;보기&#x200B;**단추의 톱니바퀴 아이콘**&#x200B;을(를) 클릭합니다.

   1. **연락처 정보 보기**&#x200B;를 사용하지 않도록 설정한 다음 X를 클릭하여 **설정 세부 조정** 상자를 닫습니다.

      ![사용자 설정 미세 조정](assets/fine-tune-users.png)

1. 플랜 라이선스 액세스 권한이 있는 사용자가 다른 사용자를 편집할 수 있는 기능을 수정하려면 ![](assets/gear-icon-settings.png)사용자&#x200B;**오른쪽에 있는**&#x200B;편집&#x200B;**단추의 톱니바퀴 아이콘**&#x200B;을(를) 클릭한 다음 부여할 기능을 선택하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>만들기</strong> </td> 
      <td> <p>사용자가 사용자를 만들 수 있습니다.<br>이 옵션은 기본적으로 사용됩니다.</p> 
     <p><b>참고</b>: 조직에서 Adobe Admin Console에 온보딩한 경우에는 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.</p>
        </td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>삭제</strong> </td> 
      <td> <p> 사용자가 직접 만든 사용자를 삭제할 수 있도록 허용합니다.<br>이 옵션은 기본적으로 사용됩니다.</p> <p><b>참고</b>: 조직에서 Adobe Admin Console에 온보딩한 경우에는 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용자 관리자(모든 사용자)</strong> </td> 
      <td> <p>사용자가 Workfront의 모든 사용자에 대해 다음 작업을 수행할 수 있습니다.</p> 
       <ul> 
        <li>사용자 편집, 삭제 또는 비활성화</li> 
        <li>사용자로 로그인<p><b>참고</b>: 시스템 관리자인 사용자로 로그인할 수 없습니다.</p></li> 
        <li>사용자 암호 재설정</li> 
       </ul> <p>이 옵션은 기본적으로 비활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용자 관리자(그룹 사용자)</strong> </td> 
      <td> <p>사용자가 관리하는 그룹의 모든 사용자에 대해 다음 작업을 수행할 수 있습니다. 
        <ul>
         <li><p>사용자 편집, 삭제 또는 비활성화</p></li>
         <li>사용자로 로그인</li>
         <li><p>사용자 암호 재설정</p><p><b>참고</b>: 그룹 관리자가 Workfront 관리자로 로그인하거나 해당 관리자의 암호를 다시 설정할 수 없습니다.</p></li>
        </ul><p>이 옵션은 기본적으로 비활성화되어 있습니다.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >그룹 관리자가 관리하는 그룹의 모든 구성원에게 액세스 권한을 부여하지 않으려면 위의 사용자 관리 옵션을 모두 비활성화하십시오. 그룹 관리자는 계속해서 Workfront에 추가하거나 Workfront에서 보고하는 그룹 멤버에 액세스할 수 있습니다.

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나를 계속 사용하십시오(예: [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)).
1. 완료되면 **저장**&#x200B;을 클릭하세요.

## 라이선스 유형별 사용자 액세스

각 액세스 수준의 사용자가 사용자를 통해 수행할 수 있는 작업에 대한 자세한 내용은 문서 [각 개체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users)의 [사용자](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md) 섹션을 참조하십시오.
