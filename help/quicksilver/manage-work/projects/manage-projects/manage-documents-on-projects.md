---
product-area: projects
navigation-topic: manage-projects
title: 프로젝트 및 관련 객체에 대한 문서 관리 개요
description: Workfront 관리자가 스토리지 환경 설정 기본값을 선택하는지 여부에 따라 문서를 기존 Workfront 스토리지 또는 Adobe 엔터프라이즈 스토리지에 저장할 수 있습니다. 이 문서에서는 프로젝트, 포트폴리오, 프로그램, 템플릿, 작업 및 문제에 대한 문서를 관리하는 방법에 대해 설명합니다.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 5c4ffeabf710374b14a2335b47342be4c393a7c8
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# 프로젝트 및 관련 오브젝트에 대한 문서 관리 개요

Adobe Workfront 관리자는 조직의 저장소 환경 설정에 대한 기본값을 정의하여 Workfront에서 문서가 저장되는 위치를 나타낼 수 있습니다.

Workfront 관리자는 다음 옵션 중 하나를 선택할 수 있습니다.

* Workfront 스토리지
* Adobe 엔터프라이즈 스토리지

이 환경 설정을 사용하면 사용 가능한 저장소 위치 중 하나에 Workfront 개체에 첨부된 문서를 자동으로 저장할 수 있습니다.

>[!IMPORTANT]
>
>모든 고객이 Workfront과 Adobe 스토리지를 모두 액세스할 수 있는 것은 아닙니다. 일부 고객은 기본적으로 Workfront에만 액세스할 수 있고 다른 고객은 Adobe 엔터프라이즈 스토리지에만 액세스할 수 있습니다. Workfront 스토리지에 액세스하지 않는 고객은 구성이 필요하지 않습니다.

Workfront 관리자는 다음 중 하나를 수행할 수 있습니다.

* 두 스토리지 옵션 중 하나를 조직의 기본값으로 선택합니다.
* 다음 객체 중 하나를 생성할 때 사용할 저장소를 선택할 수 있습니다.

   * 프로젝트
   * 포트폴리오
   * 템플릿

Workfront의 저장소 환경 설정 지정에 대한 자세한 내용은 [조직의 Adobe 엔터프라이즈 저장소 사용](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)을 참조하세요.

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
* Adobe Enterprise 스토리지만 시스템 환경 설정 의 스토리지 환경 설정 영역이 없습니다.
* Workfront 스토리지 및 Adobe 엔터프라이즈 스토리지 Workfront 관리자는 다음 중 하나를 선택할 수 있습니다.

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


Workfront 스토리지의 객체에 저장된 문서는 Adobe 엔터프라이즈 스토리지의 저장소와 다르게 관리됩니다.

자세한 내용은 [Adobe 엔터프라이즈 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

다음 섹션에서는 Workfront 및 Adobe 엔터프라이즈 스토리지 옵션이 모두 있는 경우 문서 스토리지가 Workfront 객체에 대해 작동하는 방식을 설명합니다.

### 프로젝트에 대한 문서 관리

프로젝트를 사용할 때는 다음 사항을 고려하십시오.

* Adobe 엔터프라이즈 스토리지 프로젝트를 만들면 Workfront에서 문서가 저장된 프로젝트의 문서 섹션에 폴더를 만듭니다. 폴더 이름은 프로젝트와 동일한 이름입니다. 폴더를 삭제하거나 수동으로 이름을 바꿀 수 없습니다. 프로젝트의 새 이름과 일치하도록 프로젝트의 이름을 변경하면 폴더의 이름이 변경됩니다.
* Adobe-enterprise 스토리지 프로젝트를 만들거나 기존 Workfront 스토리지 포트폴리오 또는 프로그램으로 이동하면 포트폴리오 또는 프로그램이 자동으로 Adobe 엔터프라이즈 스토리지 개체로 변환됩니다.
* Adobe 엔터프라이즈 스토리지 포트폴리오 또는 프로그램에 대해 Workfront 스토리지 프로젝트를 만들 수 없습니다.

### 포트폴리오를 위한 문서 관리

포트폴리오 작업 시 다음 사항을 고려하십시오.

* Adobe 엔터프라이즈 스토리지 포트폴리오를 만들면 Workfront은 포트폴리오의 문서 섹션에 문서를 저장할 폴더를 만듭니다. 폴더 이름은 포트폴리오와 동일한 이름입니다. 폴더를 삭제하거나 수동으로 이름을 바꿀 수 없습니다. 포트폴리오의 새 이름과 일치하도록 포트폴리오의 이름을 변경하면 폴더의 이름이 변경됩니다.
* Adobe-enterprise 스토리지 프로젝트를 생성하거나 기존 Workfront-storage 포트폴리오로 이동하면 포트폴리오가 자동으로 Adobe 엔터프라이즈 스토리지 객체로 변환됩니다.
* 전환된 포트폴리오에 이전에 첨부된 문서가 있는 경우, Workfront 스토리지에 계속 저장됩니다. 새 문서는 Workfront 저장소에도 저장됩니다.
* 변환된 포트폴리오에 Workfront 스토리지에 첨부된 문서가 없는 경우 새 문서가 Adobe 엔터프라이즈 스토리지에 저장됩니다.

### 프로그램에 대한 문서 관리

프로그램 작업 시 다음 사항을 고려하십시오.

* Adobe 엔터프라이즈 스토리지 프로그램을 만들면 Workfront에서 문서가 저장된 프로그램의 문서 섹션에 폴더를 만듭니다. 폴더 이름은 프로그램과 동일한 이름입니다. 폴더를 삭제하거나 수동으로 이름을 바꿀 수 없습니다. 프로그램의 새 이름과 일치하도록 프로그램의 이름을 변경하면 폴더의 이름이 바뀝니다.
* Adobe-enterprise 스토리지 프로젝트를 생성하거나 기존 Workfront-storage 포트폴리오로 이동하면 포트폴리오가 자동으로 Adobe 엔터프라이즈 스토리지 객체로 변환됩니다.
* 전환된 프로그램에 이전에 첨부된 문서가 있으면 Workfront 저장소에 계속 저장됩니다. 새 문서는 Workfront 저장소에도 저장됩니다.
* 변환된 프로그램에 Workfront 스토리지에 첨부된 문서가 없는 경우 새 문서가 Adobe 엔터프라이즈 스토리지에 저장됩니다.

### 작업을 위한 문서 관리

작업 시 다음 사항을 고려하십시오.

* 작업은 프로젝트에서 저장소 유형을 상속합니다.
* Adobe 스토리지 프로젝트의 작업에 문서를 업로드하면 Workfront에서 작업의 문서 섹션에 폴더를 자동으로 생성합니다. 폴더 이름은 작업과 동일합니다.
* Adobe 엔터프라이즈 스토리지 작업에서 문서 폴더의 이름을 바꾸고 삭제할 수 있으며, 이 경우 폴더의 문서도 삭제됩니다. 작업에 새 문서를 추가하면 폴더가 자동으로 다시 만들어집니다. 삭제된 문서는 폴더에 다시 배치되지 않습니다.
* Adobe 엔터프라이즈 스토리지 프로젝트의 경우 작업의 문서 폴더가 프로젝트에 대해 자동으로 생성된 문서 폴더의 하위 폴더로 표시됩니다.
* Workfront 스토리지 프로젝트에서 Adobe 스토리지 프로젝트로 작업을 복사하거나 이동할 수 없습니다. 그 반대도 불가능합니다.

### 문제에 대한 문서 관리

문제 작업 시 다음 사항을 고려하십시오.

* 문제는 프로젝트에서 저장소 유형을 상속합니다.
* Adobe 스토리지 프로젝트의 문제에 문서를 업로드하면 Workfront에서 문제의 문서 섹션에 폴더를 자동으로 생성합니다. 폴더 이름은 문제와 같습니다.
* Adobe 엔터프라이즈 스토리지 문제에서 문서 폴더의 이름을 바꾸고 삭제할 수 있으며, 이 경우 폴더의 문서도 삭제됩니다. 문제에 새 문서를 추가하면 폴더가 자동으로 다시 생성됩니다. 삭제된 문서는 폴더에 다시 배치되지 않습니다.
* Adobe 엔터프라이즈 스토리지 프로젝트의 경우 문제에 있는 문서 폴더가 프로젝트에 대해 자동으로 생성된 문서 폴더의 하위 폴더로 표시됩니다.
* Workfront 스토리지 프로젝트에서 Adobe 스토리지 프로젝트로 문제를 복사하거나 이동할 수 없습니다. 그 반대도 불가능합니다.

### 프로젝트 템플릿을 위한 문서 관리

템플릿 작업 시 다음 사항을 고려하십시오.

* Adobe 엔터프라이즈 스토리지 템플릿을 만들면 Workfront에서 문서가 저장된 템플릿의 문서 섹션에 폴더를 생성합니다. 폴더 이름은 프로그램과 동일한 이름입니다. 폴더를 삭제하거나 수동으로 이름을 바꿀 수 없습니다. 템플릿의 새 이름과 일치하도록 템플릿 이름을 변경하면 폴더 이름이 변경됩니다.
* Workfront-storage 템플릿을 사용하여 Workfront-storage 프로젝트를 만들 수 있습니다. Adobe-storage 템플릿을 사용하여 Adobe-storage 프로젝트를 만들 수 있습니다.
* Workfront 스토리지 템플릿을 Adobe 스토리지 프로젝트에 첨부할 수 있으며, 이 경우 프로젝트의 스토리지 위치는 변경되지 않습니다.
* Adobe 스토리지 템플릿을 Workfront 스토리지 프로젝트에 첨부할 수 있으며, 이 경우 프로젝트의 스토리지 위치는 변경되지 않습니다.

### 템플릿 작업을 위한 문서 관리

템플릿 작업을 사용할 때는 다음 사항을 고려하십시오.

* 템플릿 작업은 템플릿에서 저장소 유형을 상속합니다.
* Adobe 스토리지 템플릿의 템플릿 작업에 문서를 업로드하면 템플릿 작업의 문서 섹션에 Workfront에서 자동으로 폴더를 생성합니다. 폴더 이름은 템플릿 작업과 동일합니다.
* Adobe 엔터프라이즈 스토리지 템플릿 작업에서 문서 폴더의 이름을 바꾸고 삭제할 수 있으며, 이 경우 폴더의 문서도 삭제됩니다. 템플릿 작업에 새 문서를 추가하면 폴더가 자동으로 다시 만들어집니다. 삭제된 문서는 폴더에 다시 배치되지 않습니다.
* Adobe 엔터프라이즈 스토리지 템플릿의 경우 템플릿 작업의 문서 폴더가 템플릿에 대해 자동으로 생성된 문서 폴더의 하위 폴더로 표시됩니다.
* 템플릿 작업을 Workfront-storage 템플릿에서 Adobe-storage 템플릿으로 복사하거나 이동할 수 없습니다. 그 반대도 불가능합니다.
* Adobe 스토리지와 연결된 요청 대기열에 제출한 문제에 문서를 첨부하면 문서가 저장된 제출된 각 문제에 대해 폴더가 생성됩니다. 또한 이 폴더는 요청 대기열에서 자동으로 생성된 프로젝트 폴더에 하위 폴더로 추가됩니다.
