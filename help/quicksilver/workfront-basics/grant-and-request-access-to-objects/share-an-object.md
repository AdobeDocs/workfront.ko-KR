---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 개체 공유
description: Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 개체를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 객체에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 사용자 정의 액세스 수준 만들기 또는 수정을 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: 27a1beb9-e83a-4ef6-bf5f-ad52575a993c
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%

---

# 개체 공유

<!--Audited: 01/2024-->

Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 개체를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 객체에 대한 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

사용자에게 부여되는 액세스 수준과 함께 작성했거나 공유할 수 있는 액세스 권한이 있는 특정 개체를 보거나 편집할 수 있는 권한을 부여할 수도 있습니다. 액세스 수준 및 권한에 대한 자세한 내용은 [액세스 수준 및 권한이 함께 작동하는 방식](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

개체에 대한 공유 권한에 대한 자세한 내용은 [오브젝트에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아닌 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

이 문서에서는 다음 오브젝트를 공유하는 방법에 대해 설명합니다.

* 프로젝트, 작업, 문제
* Portfolio, 프로그램
* 문서

Workfront의 다른 모든 개체를 공유하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* 템플릿의 경우 다음을 참조하십시오. [프로젝트 템플릿 공유](../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* 증명의 경우 다음을 참조하십시오. [Workfront Proof에서 증명 공유](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).
* 보고서, 대시보드 및 달력의 경우 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 보고서 공유](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [대시보드 공유](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [캘린더 보고서 공유](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

  또한 다음을 참조하십시오. [보고서, 대시보드 및 캘린더 공유](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) 보고서, 대시보드 및 캘린더 공유에 대한 일반 정보.

* 필터, 보기 및 그룹화에 대해서는 [필터, 보기 또는 그룹화 공유](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* 문서 폴더의 경우 [문서 폴더 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).
* 플랜의 경우 다음을 참조하십시오. [시나리오 플래너에서 계획 공유](../../scenario-planner/share-a-plan.md).

  이를 위해서는 추가 라이센스가 필요합니다.

* 목표에 대해서는 다음을 참조하십시오. [Workfront 목표에서 목표 공유](../../workfront-goals/workfront-goals-settings/share-a-goal.md). 이를 위해서는 추가 라이센스가 필요합니다.

## 액세스 요구 사항

객체를 공유하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새 라이선스: Standard</p> 
   또는
   <p>현재 라이선스: 작업 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>공유할 개체에 대한 액세스 이상의 보기</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>공유할 개체에 대한 권한 이상 보기</p></td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 단일 개체 공유 {#share-a-single-object}

1. 공유할 개체로 이동합니다.

   공유할 수 있는 객체에 대한 자세한 내용은 [오브젝트에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
1. 프로젝트, 작업 및 문제의 경우:

   다음을 클릭합니다. **공유** 객체 이름 옆에 있는 단추입니다.

   ![](assets/new-share-button.png)

   또는

   문서, 포트폴리오 및 프로그램의 경우:

   다음을 클릭합니다. **자세히** 아이콘 ![](assets/more-icon.png)객체 이름 옆에 있는 을(를) 클릭한 다음 을(를) 클릭합니다 **공유** 또는 **공유.**

   ![](assets/share-a-document-350x160.png)

1. 다음에서 **&lt; 객체 이름 > 액세스 권한 부여** 상자(문서, 포트폴리오 및 프로그램용) 또는 **&lt; 객체 이름 > 액세스 권한 부여** 상자(프로젝트, 작업 및 문제)에서 객체를 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.

   예를 들어 프로젝트를 공유하는 경우 **프로젝트 액세스 권한 부여 대상** 필드.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 객체를 공유할 수 있습니다.

   ![](assets/nwe-project-sharing-modal-350x456.png)

   >[!TIP]
   >
   >이름이 비슷한 여러 엔티티가 있는 경우 해당 유형 아래에 모두 나열됩니다. 엔티티의 이름은 알파벳순으로 나타납니다. 그러나 엔티티 유형이 나타나는 순서는 임의입니다.
   >
   >
   >![](assets/sharing-entities-named-similarly-in-sharing-box-350x179.png)   >
   >

1. (선택 사항) 객체에 대한 액세스 권한을 부여할 각 사용자, 팀, 역할 또는 그룹에 대해 3단계를 반복합니다.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: esnure this stays accurate; in the editor it looks like step 4 but one step is conditioned entirely for one version or another)
   </MadCap:conditionalText>
   -->

1. 드롭다운 메뉴를 클릭한 다음 부여할 권한 수준을 선택하여 3단계에서 추가한 각 사용자, 팀, 역할, 그룹 또는 회사에 대한 권한을 지정합니다.

   개체에서 권한을 제거하려면 다음을 참조하십시오. [오브젝트에서 권한 제거](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   다음 옵션을 사용할 수 있습니다.

   * **보기:** 사용자는 항목을 검토하고 공유할 수 있습니다.
   * **참여**: 사용자는 업데이트, 정보 기록, 간단한 편집, 공유 및 모든 보기 권한을 수행할 수 있습니다.

     >[!TIP]
     >
     >다음 개체에만 Contribute 권한을 부여할 수 있습니다.
     >
     >   
     >   
     >   * 프로젝트
     >   * 작업
     >   * 문제
     >   
     >

   * **관리:** 사용자는 액세스 수준에서 부여된 관리 권한 없이 객체에 대한 전체 액세스 권한을 갖습니다. 또한 모든 보기 및 기여 권한도 있습니다.

     >[!NOTE]
     >
     >Workfront 관리자 또는 개체 작성자는 이러한 엔티티에서 권한을 제거할 수 있습니다.

     ![](assets/screen-shot-2013-12-04-at-1.13.11-pm.png)

1. (선택 사항) **고급 옵션** 을 클릭하여 개체에 대한 특정 권한을 구성합니다.

   보기, 관리 및 기여는 선택한 객체에 따라 다른 고급 옵션이 있습니다.\
   권한 수준에 대한 자세한 내용은 [오브젝트에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

   ![](assets/screen-shot-2013-12-04-at-1.14.11-pm.png)

1. (선택 사항) 이 객체를 시스템의 모든 사용자가 사용할 수 있도록 하려면 **톱니바퀴** 아이콘 ![](assets/gear-icon-settings-with-dn-arrow.jpg) 을 클릭한 다음 드롭다운 메뉴에서 을(를) 클릭합니다 **시스템 전체에 표시**.

   모든 사용자는 사용자가 설정한 권한에 따라 개체를 볼 수 있습니다.

1. (선택 사항 및 조건부) 프로젝트를 공유할 때 **톱니바퀴** 아이콘 ![](assets/gear-icon-settings-with-dn-arrow.jpg)을 클릭한 다음 드롭다운 메뉴에서 을(를) 클릭합니다 **내 프로젝트 액세스 템플릿으로 설정** 사용 권한을 템플릿으로 설정합니다.\
   한 프로젝트에 대한 권한을 정의한 후에는 다음에 프로젝트를 처음부터 만들 때 이와 동일한 권한이 자동으로 적용됩니다.

   >[!NOTE]
   >
   >프로젝트 액세스 템플릿은 액세스 수준의 Workfront 관리자가 부여한 공유 기본값을 무시합니다.\
   >액세스 수준에서 프로젝트에 대한 공유 기본값을 지정하는 방법에 대한 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->

   템플릿을 공유할 때 템플릿에서 만들 프로젝트에 대한 권한을 지정할 수 있습니다. 자세한 내용은 [프로젝트 템플릿 공유](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. (선택 사항) 객체를 공개로 만들려면 **외부 사용자에게 공개하기**.

   >[!TIP]
   >
   >일부 객체에는 이 옵션을 사용할 수 없습니다.

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png)

1. (조건부) 객체를 외부 사용자에게 공개하도록 한 경우 **링크 복사**&#x200B;를 클릭한 다음 링크를 외부 사용자에게 배포합니다.\
   링크가 있는 모든 사용자는 개체를 볼 수 있습니다.

   >[!CAUTION]
   >
   >외부 사용자와 기밀 정보가 포함된 오브젝트를 공유할 때는 주의하는 것이 좋습니다. 이를 통해 Workfront 사용자 또는 조직의 일부가 아니더라도 정보를 볼 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

## 개체를 일괄적으로 공유

객체 목록에서 다른 사용자, 팀, 그룹, 작업 역할 또는 회사와 여러 객체를 한 번에 공유할 수 있습니다.

>[!IMPORTANT]
>
>개체를 대량으로 공유할 때 개별 개체에 대한 사용 권한이 있는 엔터티의 이름이 표시되지 않습니다. 개체를 일괄적으로 공유할 때 공유 목록에 추가한 엔티티가 선택한 개체에 추가됩니다. 개별 객체와 연관된 엔티티는 재정의하지 않습니다.

객체를 벌크로 공유하려면 다음을 수행합니다.

1. 객체 목록으로 이동합니다.
1. 목록에서 개체를 두 개 이상 선택합니다.
1. 다음을 클릭합니다. **공유** 아이콘 ![](assets/share-icon.png).\
   이미 오브젝트에 대한 액세스 권한이 있는 사용자는 벌크 공유 시 사용할 수 있는 것으로 나열되지 않습니다.

   >[!NOTE]
   >
   >선택한 개체를 공유할 수 있는 권한이 없는 경우 **공유** 단추가 표시되지 않습니다.

1. 다음에서 **편집 &lt; 객체 이름 > 액세스 대상** 필드에서는 권한을 부여할 사용자, 팀, 그룹, 작업 역할 또는 회사의 이름을 입력합니다.

   예를 들어 프로젝트를 공유하는 경우 **프로젝트 액세스 권한 부여 대상** 필드.

   ![](assets/share-multiple-projects-people-box-nwe-350x480.png)

1. 섹션에서 4-9단계에 설명된 대로 선택한 객체를 계속 공유합니다. [단일 개체 공유](#share-a-single-object) 이 문서에서.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure these steps stay accurate; always look at them in the viewer; because of condiitoning, the steps numbers in the editor are different!!!!!!*****)
   </MadCap:conditionalText>
   -->

1. **저장**&#x200B;을 클릭합니다.
