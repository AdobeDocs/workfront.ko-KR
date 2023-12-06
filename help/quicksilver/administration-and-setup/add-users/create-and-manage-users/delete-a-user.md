---
title: 사용자 삭제
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 사용자가 조직을 떠나면 Workfront에서 해당 사용자를 제거할 수 있지만 삭제하는 대신 비활성화하는 것이 좋습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# 사용자 삭제

사용자가 조직을 떠나면 Adobe Workfront에서 해당 사용자를 제거할 수 있습니다.

>[!IMPORTANT]
>
>* 시스템에서 사용자를 삭제하면 유지할 사용자와 관련된 정보도 삭제됩니다. 사용자를 삭제하는 대신 비활성화하는 것이 좋습니다. 자세한 내용은 [사용자 비활성화 또는 재활성화](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* 이 페이지에 설명된 절차는 아직 Admin Console에 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩된 경우 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>에서 사용자 삭제 [!DNL Adobe Admin Console] 에서 사용자 비활성화 [!DNL Workfront]에서 삭제하지는 않습니다. [!DNL Workfront].
>
>  Adobe Admin Console에서 사용자를 삭제하는 방법에 대한 지침은 문서의 &quot;사용자 영구 삭제&quot; 섹션을 참조하십시오 [개별적으로 사용자 관리](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 또는 Adobe Admin Console 관리자에게 문의하십시오.
>
>  조직이 Adobe Admin Console에 온보딩되었는지 여부에 따라 달라지는 절차 목록은 을 참조하십시오. [플랫폼 기반 관리의 차이점(Adobe Workfront/Adobe 비즈니스 플랫폼)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>

## 액세스 요구 사항

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
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>. </p> </li> 
     <li> <p><b>사용자</b> 액세스 수준의 설정이 다음으로 구성됨 <b>편집</b> 액세스, 사용 <b>만들기</b> 그리고 둘 중 하나 이상은 <b>사용자 관리자</b> 아래에 옵션 활성화됨 <b>설정 미세 조정</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>다음 두 옵션 중 사용자 <b>관리자(그룹 사용자)</b> 이(가) 활성화되어 있으면 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> <p>에 대한 자세한 내용은 <b>사용자</b> 액세스 수준에서 을(를) 설정합니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 삭제 및 비활성화

사용자를 비활성화하면 다음과 같은 일이 발생합니다.

* Workfront 증명 구성 요소가 Workfront 계정과 연결된 경우 Workfront 및 Workfront 증명 모두에 대한 사용자 라이선스를 제거합니다. Workfront 증명에 대한 자세한 내용은 [Workfront 증명: 문서 색인](../../../workfront-proof/workfront-proof.md).
* 사용자에게 더 이상 작업을 할당할 수 없습니다.
* 사용자는 더 이상 업데이트에 추가할 수 없습니다.
* 사용자를 더 이상 팀이나 그룹에 추가할 수 없습니다.
* 개체를 더 이상 사용자와 공유할 수 없습니다.
* 다음 개체와의 연관성이 그대로 유지됩니다.

   * 작업, 문제, 프로젝트, 포트폴리오
   * 대시보드

     >[!NOTE]
     >
     >사용자를 비활성화하고 더 이상 사용자와 연결된 보고서나 대시보드를 볼 수 없는 경우 **다음의 액세스 권한으로 이 보고서 실행:** 필드.\
     >자세한 내용은 [비활성화된 사용자가 소유한 보고서에 액세스할 수 없는 이유는 무엇입니까?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) 의 섹션 [보고서 FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 기사.

   * 문서
   * 업데이트
   * 시간

* 문서를 체크 아웃한 경우 비활성화하면 문서가 체크 아웃된 상태로 유지됩니다. Workfront 관리자만 다시 체크인할 수 있습니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md).

사용자를 삭제하면 다음과 같은 일이 발생합니다.

* Workfront Proof 구성 요소가 Workfront 계정과 연결된 경우 Workfront 및 Workfront Proof 모두에 대한 사용자 라이선스를 제거합니다. Workfront 증명에 대한 자세한 내용은 [Workfront 증명: 문서 색인](../../../workfront-proof/workfront-proof.md).
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
     >자세한 내용은 [삭제된 사용자가 소유한 보고서가 포함된 대시보드에 액세스하려면 어떻게 합니까?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) 의 섹션 [보고서 FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 기사.

   * 업데이트
   * 시간

     >[!NOTE]
     >
     >이러한 오브젝트는 Workfront에 남아 있지만 오브젝트 소유자는 비어 있습니다.

* 사용자가 전역 탐색 막대의 문서 영역 아래에 있는 문서를 업로드한 경우 해당 문서도 삭제됩니다.
* 사용자가 소유한 문서를 체크아웃하고 기본 메뉴에서 액세스할 수 있는 기본 문서 영역에 문서를 업로드하면 문서가 사용자와 함께 삭제됩니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md).

사용자 비활성화에 대한 자세한 내용은 [사용자 비활성화 또는 재활성화](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

한 번에 하나씩 사용자를 영구적으로 삭제하거나 여러 사용자를 동시에 영구적으로 삭제할 수 있습니다. 개별 사용자를 삭제하는 경우 Workfront의 다른 활동으로 이동하기 전에 삭제 프로세스가 완료될 때까지 기다려야 합니다. 여러 사용자를 삭제하는 프로세스는 동시에 백그라운드 프로세스로 실행되므로 사용자가 삭제될 때 Workfront을 계속 사용할 수 있습니다.

## 한 명 이상의 사용자 삭제

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront 오른쪽 상단에 있습니다.

1. 클릭 **사용자**.
1. 삭제할 사용자를 한 명 이상 선택하고 기타 메뉴를 클릭합니다 ![](assets/more-icon.png)을 클릭한 다음 을 클릭합니다 **삭제**.
1. 표시되는 상자에서 **삭제** 삭제 확인.

   사용자 삭제 프로세스는 백그라운드 프로세스로 실행되므로 사용자가 삭제될 때 Workfront을 계속 사용할 수 있습니다.

   삭제하는 사용자 수에 따라 프로세스는 몇 분 또는 몇 시간이 걸릴 수 있습니다.

   Workfront에서 사용자가 삭제되었다는 확인을 받은 후 백그라운드에서 삭제 프로세스가 완료될 때까지 시스템에 해당 사용자가 계속 표시될 수 있습니다.

   나중에 한 명 이상의 사용자가 성공적으로 삭제되지 않은 경우 한 번에 하나씩 삭제해 보십시오.
