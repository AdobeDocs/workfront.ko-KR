---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 삭제
description: 조직에서 더 이상 사용하지 않는 작업 역할을 삭제할 수 있습니다. 작업 역할이 과거에 작업 항목과 연결된 경우에는 삭제하지 않는 것이 좋습니다. 작업 할당에 대한 모든 내역 정보를 유지하려면 더 이상 사용되지 않는 역할을 삭제하는 대신 비활성화하는 것이 좋습니다. 역할 비활성화에 대한 자세한 내용은 작업 역할 비활성화를 참조하십시오.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 작업 역할 삭제

조직에서 더 이상 사용하지 않는 작업 역할을 삭제할 수 있습니다. 작업 역할이 과거에 작업 항목과 연결된 경우에는 삭제하지 않는 것이 좋습니다.

작업 할당에 대한 모든 내역 정보를 유지하려면 더 이상 사용되지 않는 역할을 삭제하는 대신 비활성화하는 것이 좋습니다. 역할 비활성화에 대한 자세한 내용은 [작업 역할 비활성화](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)를 참조하십시오.

## 액세스 요구 사항

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL 계획]</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>작업 역할에 대한 관리 액세스</td>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 역할 삭제

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. **[!UICONTROL 작업 역할].**&#x200B;을 클릭합니다.
1. 삭제할 작업 역할을 선택한 다음 **[!UICONTROL 삭제].**&#x200B;를 클릭합니다
1. 작업 역할에 할당된 개체(사용자, 작업, 문제)가 있는 경우 다음 중 하나를 수행합니다.

   * **작업 역할을 다른 작업 역할로 바꾸기:** 드롭다운 목록에서 새 작업 역할을 선택합니다.

     삭제된 작업 역할과 연결된 현재 및 과거 리소스 할당은 선택한 작업 역할로 전송됩니다.

     작업 역할이 한 개만 할당된 사용자는 선택한 작업 역할에 재할당되고, 보조 작업 역할이 할당된 사용자는 선택한 작업 역할에 재할당되지 않습니다.

   * **작업 역할과 해당 리소스 할당을 삭제합니다.** 드롭다운 목록에서 **[!UICONTROL 없음]**&#x200B;을 선택합니다.

     >[!IMPORTANT]
     >
     >작업 역할을 삭제하면 모든 프로젝트에 대해 해당 작업 역할과 관련된 현재 및 과거 리소스 할당이 모두 삭제됩니다.

     예를 &#x200B; 들어 작업 또는 문제가 해당 작업 역할에만 할당된 경우 작업 역할이 삭제된 후에는 작업 또는 문제가 할당 해제됩니다.

1. **[!UICONTROL 예, 삭제]**&#x200B;를 클릭합니다.
