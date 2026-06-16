---
product-area: projects
navigation-topic: manage-projects
title: 프로젝트 및 관련 객체에 대한 문서 관리 개요
description: Workfront 관리자가 스토리지 환경 설정 기본값을 선택하는지 여부에 따라 문서를 기존 Workfront 스토리지 또는 Adobe 클라우드 스토리지에 저장할 수 있습니다. 이 문서에서는 프로젝트, 포트폴리오, 프로그램, 템플릿, 작업 및 문제에 대한 문서를 관리하는 방법에 대해 설명합니다.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 397e5e36632872bb7be3f4e219b36e33b44136e9
workflow-type: tm+mt
source-wordcount: '2037'
ht-degree: 0%

---

# 프로젝트 및 관련 오브젝트에 대한 문서 관리 개요

Adobe Workfront 관리자는 조직의 저장소 환경 설정에 대한 기본값을 정의하여 Workfront에서 문서가 저장되는 위치를 나타낼 수 있습니다.

Workfront 관리자는 다음 옵션 중 하나를 선택할 수 있습니다.

* Workfront 스토리지
* Adobe 클라우드 스토리지

이 환경 설정을 사용하면 사용 가능한 저장소 위치 중 하나에 Workfront 개체에 첨부된 문서를 자동으로 저장할 수 있습니다.

>[!IMPORTANT]
>
>Workfront 인스턴스는 Workfront 및 Adobe 스토리지 모두에 액세스하지 못할 수 있습니다. 일부 Workfront 인스턴스는 Workfront에만 액세스할 수 있고, 다른 인스턴스는 기본적으로 Adobe 클라우드 스토리지에만 액세스할 수 있습니다. 한 가지 유형의 스토리지만 액세스하는 고객은 구성이 필요하지 않습니다.

Workfront 관리자는 다음 중 하나를 수행할 수 있습니다.

* 두 스토리지 옵션 중 하나를 조직의 기본값으로 선택합니다.
* 다음 객체 중 하나를 생성할 때 사용할 저장소를 선택할 수 있습니다.

   * 프로젝트
   * 포트폴리오
   * 템플릿

Workfront의 저장소 환경 설정 지정에 대한 자세한 내용은 [조직에 Adobe 클라우드 저장소 사용](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)을 참조하세요.

이 문서에서는 프로젝트, 포트폴리오, 프로그램, 작업, 문제, 템플릿 및 템플릿 작업에 대한 문서를 관리하는 방법에 대해 설명합니다.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## 문서 저장소 개요

고객은 다음 문서 스토리지 기능 중 하나에 액세스할 수 있습니다.

* Workfront 스토리지만 시스템 환경 설정 의 스토리지 환경 설정 영역이 없습니다.
* Adobe 클라우드 스토리지만. 시스템 환경 설정 의 스토리지 환경 설정 영역이 없습니다.
* Workfront 스토리지 및 Adobe 클라우드 스토리지 둘 다. Workfront 관리자는 다음 중 하나를 선택할 수 있습니다.

   * 향후 문서 처리 방법에 대한 기본 스토리지 환경을 선택합니다.
   * 사용자가 다음 객체를 생성할 때 선택할 스토리지를 선택할 수 있습니다.

      * 프로젝트
      * 포트폴리오
      * 템플릿

  >[!NOTE]
  >
  >* 작업 및 문제는 프로젝트에서 저장소 유형을 상속합니다.
  >* 템플릿 작업은 템플릿에서 저장소 유형을 상속합니다.
  >* 프로그램은 포트폴리오에서 저장소 유형을 상속합니다.


Workfront 스토리지의 객체에 저장된 문서는 Adobe 클라우드 스토리지에 저장된 문서와 다르게 관리됩니다.

자세한 내용은 [Adobe 클라우드 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

다음 섹션에서는 Workfront 및 Adobe 클라우드 스토리지 옵션이 동일한 환경에 있을 때 Workfront 객체에 대해 문서 저장이 작동하는 방식을 설명합니다.

### 프로젝트에 대한 문서 관리

프로젝트를 사용할 때는 다음 사항을 고려하십시오.

* Adobe 클라우드 스토리지 프로젝트를 만들면 Workfront은 프로젝트의 문서 섹션에 문서가 저장되는 폴더를 만듭니다. 폴더 이름은 프로젝트와 동일한 이름입니다. 폴더를 삭제하거나 수동으로 이름을 바꿀 수 없습니다. 프로젝트의 새 이름과 일치하도록 프로젝트의 이름을 변경하면 폴더의 이름이 변경됩니다.
* Adobe 클라우드 스토리지 프로젝트를 기존 Workfront 스토리지 포트폴리오 또는 프로그램으로 만들거나 이동할 때, 포트폴리오 또는 프로그램에 프로젝트를 추가하기 전에 문서가 첨부되어 있지 않은 경우 포트폴리오 또는 프로그램은 자동으로 Adobe 클라우드 스토리지 객체로 변환됩니다.
* Adobe 클라우드 스토리지 포트폴리오 또는 프로그램에 대한 레거시 Workfront 스토리지 프로젝트는 생성할 수 없습니다.
* MS Project에서 프로젝트를 가져오면 Workfront 관리자가 Workfront 클라우드 스토리지를 시스템의 기본값으로 설정한 경우에도 Workfront은 레거시 Adobe 스토리지 프로젝트를 만듭니다.
* Workfront Planning 자동화를 사용하여 프로젝트를 만들 때 Workfront에서는 프로젝트에 대한 시스템의 기본 스토리지 환경 설정을 사용합니다. Workfront Planning에 액세스하려면 Planning 패키지를 구매해야 합니다.

자세한 내용은 이 문서의 [프로젝트 템플릿에 대한 문서 관리](#document-management-for-project-templates) 섹션을 참조하십시오.

### 포트폴리오를 위한 문서 관리

포트폴리오 작업 시 다음 사항을 고려하십시오.

* Adobe 클라우드 스토리지 포트폴리오를 만들면 Workfront은 포트폴리오의 문서 섹션에 문서를 저장할 폴더를 만듭니다. 폴더 이름은 포트폴리오와 동일한 이름입니다. 폴더를 삭제하거나 수동으로 이름을 바꿀 수 없습니다. 포트폴리오의 새 이름과 일치하도록 포트폴리오의 이름을 변경하면 폴더의 이름이 변경됩니다.

* 기존 Adobe 스토리지 포트폴리오에 Workfront 클라우드 스토리지 프로젝트를 추가하고 포트폴리오에 첨부된 문서가 없으면 포트폴리오가 Adobe 클라우드 스토리지 포트폴리오로 변환됩니다.
* 기존 Adobe 스토리지 포트폴리오에 Workfront 클라우드 스토리지 프로젝트를 추가하고 포트폴리오에 문서가 첨부되어 있으면 포트폴리오 문서 스토리지는 Workfront 스토리지에 유지됩니다. 그러나 포트폴리오 ![레거시 Workfront 저장소 아이콘](assets/legacy-storage-project-icon.png)에 대한 레거시 포트폴리오 저장소 아이콘이 포트폴리오에서 제거되었습니다.
* Adobe 클라우드 스토리지 프로젝트를 레거시 스토리지 포트폴리오에 추가하거나 레거시 스토리지 프로젝트를 Adobe 스토리지 포트폴리오에 추가할 수 없습니다.
* 관리자는 설정의 시스템 환경 설정 영역에서 레거시 스토리지 포트폴리오를 Adobe 클라우드 스토리지로 변환할 수 있습니다. 모든 하위 개체(프로그램, 프로젝트 및 문서)는 기존 저장소에 남아 있습니다. 새 프로젝트는 Adobe 클라우드 스토리지를 사용합니다. 포트폴리오에 추가된 새 문서는 레거시 스토리지에 계속 저장됩니다.
자세한 내용은 [시스템 환경 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.

* Workfront Planning 자동화를 사용하여 포트폴리오를 생성하는 경우 Workfront에서는 포트폴리오에 대한 시스템의 기본 스토리지 환경 설정을 사용합니다. Workfront Planning에 액세스하려면 Planning 패키지를 구매해야 합니다.


### 프로그램에 대한 문서 관리

프로그램 작업 시 다음 사항을 고려하십시오.

* Adobe 클라우드 스토리지 프로그램을 만들면 Workfront은 문서가 저장되는 프로그램의 문서 섹션에 폴더를 만듭니다. 폴더 이름은 프로그램 이름과 같습니다. 폴더를 삭제하거나 수동으로 이름을 바꿀 수 없습니다. 프로그램의 새 이름과 일치하도록 프로그램의 이름을 변경하면 폴더의 이름이 바뀝니다.

* 기존 Workfront 스토리지 프로젝트를 Adobe 클라우드 스토리지 프로그램에 추가할 수 없습니다.

* Adobe 클라우드 스토리지 프로그램을 레거시 스토리지 포트폴리오에 추가하거나 레거시 프로그램을 Adobe 클라우드 스토리지 포트폴리오에 추가할 수 없습니다.
* 레거시 스토리지 프로그램의 Adobe 클라우드 스토리지 템플릿에서 프로젝트를 생성할 수 없습니다.
* Adobe 클라우드 스토리지 프로그램의 레거시 스토리지 템플릿에서 프로젝트를 만들 수 있지만 템플릿의 문서 및 폴더는 새 프로젝트에 추가되지 않습니다. 프로젝트는 Adobe 클라우드 스토리지를 받습니다.
* Workfront Planning 자동화를 사용하여 프로그램을 생성하는 경우 Workfront에서는 해당 프로그램에 대한 시스템의 기본 스토리지 기본 설정을 사용합니다. Workfront Planning에 액세스하려면 Planning 패키지를 구매해야 합니다.

### 작업을 위한 문서 관리

작업 시 다음 사항을 고려하십시오.

* 작업은 프로젝트에서 저장소 유형을 상속합니다.
* Adobe 클라우드 스토리지 프로젝트의 작업에 문서를 업로드하면 Workfront에서 작업의 문서 섹션에 폴더를 자동으로 생성합니다. 폴더 이름은 작업과 동일합니다.
* 폴더의 문서도 삭제하는 Adobe 클라우드 스토리지 작업에서 문서 폴더의 이름을 바꾸고 삭제할 수 있습니다. 작업에 새 문서를 추가하면 폴더가 자동으로 다시 만들어집니다. 삭제된 문서는 폴더에 다시 배치되지 않습니다.
* Adobe 클라우드 스토리지 프로젝트의 경우 작업의 문서 폴더가 프로젝트에 대해 자동으로 생성된 문서 폴더의 하위 폴더로 표시됩니다.
* 기존 Workfront 스토리지 프로젝트에서 Adobe 클라우드 스토리지 프로젝트로 작업을 복사하거나 이동할 수 없습니다. 그 반대도 불가능합니다.
* 작업을 프로젝트로 전환할 때 다음과 같은 시나리오가 존재합니다. <!--this info also duplicated in Convert tasks to projects-->
   * 기존 Workfront 스토리지 작업은 기존 Workfront 스토리지 프로젝트를 만듭니다.
   * Adobe 클라우드 스토리지 작업은 Adobe 클라우드 스토리지 프로젝트를 만듭니다.
   * 기존 Workfront 스토리지 템플릿을 사용하여 Adobe 클라우드 스토리지 작업을 전환하면 Adobe 클라우드 스토리지 프로젝트가 만들어집니다.
   * Adobe 클라우드 스토리지 템플릿을 사용하여 기존 Workfront 스토리지 작업을 전환하면 기존 Workfront 스토리지 프로젝트가 만들어집니다.
* 요약 패널에서 Adobe 클라우드 스토리지 작업에 문서를 추가할 수 없습니다.

### 문제에 대한 문서 관리

문제 작업 시 다음 사항을 고려하십시오.

* 문제는 프로젝트에서 저장소 유형을 상속합니다.
* Adobe 클라우드 스토리지 프로젝트의 문제에 문서를 업로드하면 Workfront에서 문제의 문서 섹션에 폴더를 자동으로 생성합니다. 폴더 이름은 문제와 같습니다.
* 폴더의 문서도 삭제되는 Adobe 클라우드 스토리지 문제에서 문서 폴더의 이름을 바꾸고 삭제할 수 있습니다. 문제에 새 문서를 추가하면 폴더가 자동으로 다시 생성됩니다. 삭제된 문서는 폴더에 다시 배치되지 않습니다.
* Adobe 클라우드 스토리지 프로젝트의 경우 문제에 있는 문서 폴더가 프로젝트에 대해 자동으로 생성된 문서 폴더의 하위 폴더로 표시됩니다.
* 기존 Workfront 스토리지 프로젝트에서 Adobe 클라우드 스토리지 프로젝트로 문제를 복사하거나 이동할 수 없습니다. 그 반대도 불가능합니다.
* 문제를 프로젝트로 전환할 때 다음과 같은 시나리오가 존재합니다. <!--this info also duplicated in Convert an issue to a project-->
   * 이전 Workfront 스토리지 문제로 이전 Workfront 스토리지 프로젝트가 생성되었습니다.
   * Adobe 클라우드 스토리지 문제로 Adobe 클라우드 스토리지 프로젝트가 생성되었습니다.
   * 기존 Workfront 스토리지 템플릿을 사용하여 Adobe 클라우드 스토리지 문제를 전환하면 Adobe 클라우드 스토리지 프로젝트가 생성됩니다.
   * Adobe 클라우드 스토리지 템플릿을 사용하여 기존 Workfront 스토리지 문제를 전환하면 기존 Workfront 스토리지 프로젝트가 만들어집니다.
* 요약 패널에서 Adobe 클라우드 스토리지 문제에 문서를 추가할 수 없습니다.

### 요청에 대한 문서 관리

* 요청 대기열로 작동하는 레거시 Workfront 스토리지 프로젝트에 문서가 첨부된 Workfront 요청을 제출하면 시스템 스토리지 기본 설정이 Adobe 클라우드 스토리지이더라도 요청의 문서 영역에 프로젝트의 스토리지 유형을 사용하여 문서가 표시됩니다.
* Adobe 스토리지와 연결된 요청 대기열에 제출한 문제에 문서를 첨부하면 문서가 저장된 제출된 각 문제에 대해 폴더가 생성됩니다. 또한 이 폴더는 요청 대기열 프로젝트에서 자동으로 생성된 프로젝트 폴더에 하위 폴더로 추가됩니다.

### 프로젝트 템플릿을 위한 문서 관리

템플릿 작업 시 다음 사항을 고려하십시오.

* Adobe 클라우드 스토리지 템플릿을 만들면 Workfront은 문서가 저장된 템플릿의 문서 섹션에 폴더를 생성합니다. 폴더 이름은 프로그램과 동일한 이름입니다. 폴더를 삭제하거나 수동으로 이름을 바꿀 수 없습니다. 템플릿의 새 이름과 일치하도록 템플릿 이름을 변경하면 폴더 이름이 변경됩니다.
* 레거시 Workfront 스토리지 템플릿을 사용하여 레거시 Workfront 스토리지 프로젝트를 생성할 수 있습니다. Adobe 클라우드 스토리지 템플릿을 사용하여 Adobe 클라우드 스토리지 프로젝트를 생성할 수 있습니다.

* 포트폴리오 또는 프로그램의 템플릿을 사용하여 프로젝트를 만들 때 다음과 같은 시나리오가 있습니다.
   * 레거시 Workfront 스토리지 포트폴리오 또는 프로그램의 Adobe 클라우드 스토리지 템플릿을 사용하여 프로젝트를 생성할 수는 없습니다.
   * 레거시 스토리지 템플릿을 사용하여 Adobe 스토리지 포트폴리오나 프로그램에 대한 Adobe 클라우드 스토리지 프로젝트를 생성할 수 있습니다. 템플릿 문서 및 폴더는 새 프로젝트에 첨부되지 않습니다.

* 레거시 Workfront 스토리지 템플릿을 Adobe 클라우드 스토리지 프로젝트에 첨부할 수 있으며, 프로젝트에 있는 문서의 스토리지 위치는 변경되지 않습니다.
* Adobe 클라우드 스토리지 템플릿을 기존 Workfront 스토리지 프로젝트에 첨부할 수 있으며, 이 경우 프로젝트에 있는 문서의 스토리지 위치는 변경되지 않습니다. 템플릿에 대한 Adobe 클라우드 스토리지 폴더의 문서는 폴더 없이 프로젝트에 직접 추가되지만 템플릿 작업 폴더의 문서는 작업의 문서 섹션에서 프로젝트의 작업에 첨부된 폴더에 추가됩니다.
* 프로젝트를 템플릿으로 저장하면 Workfront 관리자가 시스템의 스토리지 환경 설정에 대해 설정한 내용과 관계없이 프로젝트의 스토리지 유형이 템플릿으로 전송됩니다.


### 템플릿 작업을 위한 문서 관리

템플릿 작업을 사용할 때는 다음 사항을 고려하십시오.

* 템플릿 작업은 템플릿에서 저장소 유형을 상속합니다.
* Adobe 클라우드 스토리지 템플릿의 템플릿 작업에 문서를 업로드하면 템플릿 작업의 문서 섹션에 Workfront에서 자동으로 폴더를 생성합니다. 폴더 이름은 템플릿 작업과 동일합니다.
* 폴더의 문서도 삭제하는 Adobe 클라우드 스토리지 템플릿 작업에서 문서 폴더의 이름을 바꾸고 삭제할 수 있습니다. 템플릿 작업에 새 문서를 추가하면 폴더가 자동으로 다시 만들어집니다. 삭제된 문서는 폴더에 다시 배치되지 않습니다.
* Adobe 클라우드 스토리지 템플릿의 경우 템플릿 작업의 문서 폴더가 템플릿에 대해 자동으로 생성된 문서 폴더의 하위 폴더로 표시됩니다.
* 템플릿 작업을 기존 Workfront 스토리지 템플릿에서 Adobe 클라우드 스토리지 템플릿으로 복사하거나 이동할 수 없습니다. 그 반대도 불가능합니다.

