---
title: 사용자 삭제
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 사용자가 조직을 떠나면 Workfront에서 해당 사용자를 제거할 수 있지만 삭제하는 대신 비활성화하는 것이 좋습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# 사용자 삭제

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 Adobe 비즈니스 플랫폼에 온보딩되지 않은 조직에만 적용됩니다. Adobe 비즈니스 플랫폼에 온보딩한 경우 Adobe Admin Console에서 사용자를 삭제해야 합니다.
>
>조직이 Adobe 비즈니스 플랫폼에 온보딩되었는지 여부에 따라 달라지는 프로시저 목록은 [플랫폼 기반 관리 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.

사용자가 조직을 떠나면 Adobe Workfront에서 해당 사용자를 제거할 수 있습니다.

>[!IMPORTANT]
>
>시스템에서 사용자를 삭제하면 유지할 사용자와 관련된 정보도 삭제됩니다. 사용자를 삭제하는 대신 비활성화하는 것이 좋습니다. 자세한 내용은 [사용자 비활성화 또는 다시 활성화](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)를 참조하십시오.
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

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
   <td><p>새로운 기능: 표준</p><p>또는</p><p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. </li> 
     <li> <p>액세스 수준의 <b>사용자</b> 설정이 <b>편집</b> 액세스로 구성되었으며, <b>만들기</b>와 <b>설정을 미세 조정</b> <img src="assets/gear-icon-in-access-levels.png">에서 두 개의 <b>사용자 관리</b> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p>이 두 옵션 중 <b>사용자 관리자(그룹 사용자)</b>를 사용하도록 설정한 경우 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 삭제 및 비활성화

사용자를 비활성화하면 다음과 같은 일이 발생합니다.

* Workfront Proof 구성 요소가 Workfront 계정과 연결된 경우 Workfront 및 Workfront Proof 모두에 대한 사용자 라이선스를 제거합니다. Workfront Proof에 대한 자세한 내용은 [Workfront Proof: 문서 색인](../../../workfront-proof/workfront-proof.md)을 참조하세요.
* 사용자에게 더 이상 작업을 할당할 수 없습니다.
* 사용자는 더 이상 업데이트에 추가할 수 없습니다.
* 사용자를 더 이상 팀이나 그룹에 추가할 수 없습니다.
* 개체를 더 이상 사용자와 공유할 수 없습니다.
* 다음 개체와의 연관성이 그대로 유지됩니다.

   * 작업, 문제, 프로젝트, 포트폴리오
   * 대시보드

     >[!NOTE]
     >
     >사용자를 비활성화하고 사용자와 연결된 보고서나 대시보드를 더 이상 볼 수 없는 경우 **액세스 권한** 필드로 이 보고서 실행을 업데이트해야 할 수 있습니다.\
     >자세한 내용은 [비활성화된 사용자가 소유한 보고서에 액세스할 수 없는 이유는 무엇입니까?[보고서 FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 문서의 ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) 섹션.

   * 문서
   * 업데이트
   * 시간

* 문서를 체크 아웃한 경우 비활성화하면 문서가 체크 아웃된 상태로 유지됩니다. Workfront 관리자만 다시 체크인할 수 있습니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md)을 참조하십시오.

사용자를 삭제하면 다음과 같은 일이 발생합니다.

* Workfront Proof 구성 요소가 Workfront 계정과 연결된 경우 Workfront 및 Workfront Proof 모두에 대한 사용자 라이선스를 제거합니다. Workfront Proof에 대한 자세한 내용은 [Workfront Proof: 문서 색인](../../../workfront-proof/workfront-proof.md)을 참조하세요.
* 사용자에게 더 이상 작업을 할당할 수 없습니다.
* 사용자는 더 이상 업데이트에 추가할 수 없습니다.
* 사용자를 더 이상 팀이나 그룹에 추가할 수 없습니다.
* 개체를 더 이상 사용자와 공유할 수 없습니다.
* 해당 사용자와 다음 객체의 연관을 삭제합니다.

   * 작업, 문제, 프로젝트, 포트폴리오
   * 대시보드

     >[!NOTE]
     >
     >또한 삭제된 사용자와 관련된 대시보드가 포함된 사용자 정의 섹션에 대한 액세스 권한을 잃게 됩니다.\
     >자세한 내용은 [삭제된 사용자가 소유한 보고서가 포함된 대시보드에 액세스하려면 어떻게 합니까?[보고서 FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 문서의 ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) 섹션.

   * 업데이트
   * 시간

     >[!NOTE]
     >
     >이러한 오브젝트는 Workfront에 남아 있지만 오브젝트 소유자는 비어 있습니다.

* 사용자가 전역 탐색 막대의 문서 영역 아래에 있는 문서를 업로드한 경우 해당 문서도 삭제됩니다.
* 사용자가 소유한 문서를 체크아웃하고 기본 메뉴에서 액세스할 수 있는 기본 문서 영역에 문서를 업로드하면 문서가 사용자와 함께 삭제됩니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md)을 참조하십시오.

사용자 비활성화에 대한 자세한 내용은 [사용자 비활성화 또는 다시 활성화](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)를 참조하세요.

한 번에 하나씩 사용자를 영구적으로 삭제하거나 여러 사용자를 동시에 영구적으로 삭제할 수 있습니다. 개별 사용자를 삭제하는 경우 Workfront의 다른 활동으로 이동하기 전에 삭제 프로세스가 완료될 때까지 기다려야 합니다. 여러 사용자를 삭제하는 프로세스는 동시에 백그라운드 프로세스로 실행되므로 사용자가 삭제될 때 Workfront을 계속 사용할 수 있습니다.

## 한 명 이상의 사용자 삭제

{{step-1-to-users}}

1. 삭제할 사용자를 한 명 이상 선택하고 기타 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **삭제**&#x200B;를 클릭합니다.
1. 표시되는 상자에서 **삭제**&#x200B;를 클릭하여 삭제를 확인합니다.

   사용자 삭제 프로세스는 백그라운드 프로세스로 실행되므로 사용자가 삭제될 때 Workfront을 계속 사용할 수 있습니다.

   삭제하는 사용자 수에 따라 프로세스는 몇 분 또는 몇 시간이 걸릴 수 있습니다.

   Workfront에서 사용자가 삭제되었다는 확인을 받은 후 백그라운드에서 삭제 프로세스가 완료될 때까지 시스템에 해당 사용자가 계속 표시될 수 있습니다.

   나중에 한 명 이상의 사용자가 성공적으로 삭제되지 않은 경우 한 번에 하나씩 삭제해 보십시오.
