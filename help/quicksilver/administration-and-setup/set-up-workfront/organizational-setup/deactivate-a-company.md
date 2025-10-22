---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 회사 비활성화 또는 재활성화
description: 관련된 모든 내역 데이터를 유지하면서 더 이상 사용하지 않는 회사를 비활성화할 수 있습니다. 이미 사용 중인 회사를 시스템 어딘가에서 비활성화하면 항상 그랬던 것처럼 계속 작동합니다. 제거되거나 차단되지 않습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 2e86369ae4c8e9fe2678773c20c02f6dbf8d5247
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 1%

---

# 회사 비활성화 또는 재활성화

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

관련된 모든 내역 데이터를 유지하면서 더 이상 사용하지 않는 회사를 비활성화할 수 있습니다. 이미 사용 중인 회사를 시스템 어딘가에서 비활성화하면 항상 그랬던 것처럼 계속 작동합니다. 제거되거나 차단되지 않습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] 패키지</p> </td> 
   <td><p>임의</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스</p> </td> 
   <td><p>[!UICONTROL 계획]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>액세스 수준 구성</td> 
  <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템에서 회사를 편집할 수 있는 [!UICONTROL 시스템 관리자] 액세스 수준입니다.</p> </li> 
     <li> <p>회사 관리에 대한 관리 액세스 권한으로, 시스템에서 모든 회사를 편집할 수 있습니다.</p> </li> 
    </ul> <p><b>참고</b>:
     <ul> 
      <li> <p>그룹 관리자로 할당된 모든 그룹과 연결된 회사를 관리할 수도 있습니다.</p> </li> 
      <li> <p>[!DNL Workfront] 시스템에서 사용자를 추가하고 제거하려면 다음 중 하나가 있어야 합니다.</p> 
       <ul> 
        <li> <p>[!UICONTROL 시스템 관리자] 액세스 수준입니다. </p> </li> 
        <li> <p>액세스 수준의 <b>[!UICONTROL 사용자]</b> 설정이 <b>[!UICONTROL 편집]</b> 액세스로 구성되었으며, <b>[!UICONTROL 만들기]</b>와(과) <b>[!UICONTROL 사용자 관리]</b> <b>에서 두 개의 </b>[!UICONTROL 사용자 관리]<img src="assets/gear-icon-in-access-levels.png"> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p> <img src="assets/access-req-users.png"> </p> <p>이 두 옵션 중 <b>[!UICONTROL 사용자 관리자(그룹 사용자)]</b>이(가) 활성화된 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 회사 비활성화 또는 재활성화

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 회사]** ![회사 아이콘](assets/companies-icon-left-panel.png)을 클릭합니다.

1. 비활성화하거나 다시 활성화할 회사를 하나 이상 선택하십시오.
1. **[!UICONTROL 편집]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">(Conditional) In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>--> 클릭
1. 단일 회사의 경우 **[!UICONTROL 활성 상태임]** 옵션을 비활성화하여 비활성화하거나 옵션을 활성화하여 활성화하십시오. <!--ADD TO THE FRONT OF THIS SENTENCE In the Production environment, -->

   또는

   여러 회사의 경우 **[!UICONTROL 활성 상태임]** 드롭다운 메뉴에서 **[!UICONTROL 아니요]**&#x200B;를 선택하여 비활성화하거나 **[!UICONTROL 예]**&#x200B;를 선택하여 활성화하십시오.

1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.
