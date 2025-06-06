---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: 증명 및 GenStudio for Performance Marketing 통합 시작
description: 증명 및 GenStudio for Performance Marketing 통합 시작
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
source-git-commit: e67446c6fb3e90d5dc45dd446988e5d02291f775
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# 증명 및 GenStudio for Performance Marketing 통합 시작

Proofing과 GenStudio for Performance Marketing을 통합하여 다음과 같은 작업을 수행할 수 있습니다.

* Workfront 증명 템플릿을 사용하여 검토 및 승인 워크플로 정의

* 증명 뷰어에서 GenStudio 초안 콘텐츠 검토 및 승인

* 최종 승인 및 게시를 위한 GenStudio의 검토 결정 보기


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> 
   <p>임의</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>현재: 표준 </p> 
   <p>레거시: 플랜 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td> 
   <p> GenStudio for Performance Marketing이 있어야 하며 Admin Console의 사용자로 제품에 추가되어 있어야 합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## 통합 요구 사항

* Workfront 및 GenStudio for Performance Marketing을 동일한 IMS 조직에 배포해야 합니다.

* 사용자는 IMS 조직 내에서 하나의 Workfront 인스턴스에만 속할 수 있습니다.

* Workfront 통합 경험에서 Adobe 인스턴스를 활성화해야 합니다.

* Workfront 설정 영역에서 통합을 활성화해야 합니다.


## Workfront에서 통합 활성화

1. 왼쪽 상단의 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. 왼쪽 패널에서 **검토 및 승인** > **Adobe GenStudio**&#x200B;을 클릭합니다.
1. **증명 승인 사용**&#x200B;을 사용하도록 설정합니다.
   ![GenStudio 증명 사용](assets/enable-proofing-gs.png)

## Workfront 증명 템플릿을 사용하여 승인 워크플로 정의

조직의 콘텐츠 검토 프로세스가 자주 반복되거나 동일한 사람에 의해 검토되는 경우 증명 템플릿을 사용하여 검토 및 승인 워크플로를 자동화할 수 있습니다.

한 명 또는 두 명의 검토자만을 위한 간단한 단일 단계 템플릿을 만들거나, 여러 단계 및 종속성이 있는 복잡한 검토를 위한 자동화된 다중 단계 템플릿을 만들 수 있습니다.

사용자가 GenStudio에서 검토를 시작할 때 필요한 템플릿을 선택하면 됩니다. 사용자는 언제든지 검토자와 단계를 추가하거나 제거하여 모든 증명 워크플로 템플릿을 쉽게 변경할 수 있습니다.

증명 워크플로 템플릿을 사용하여 다음과 같은 작업을 수행할 수 있습니다.

* 특정 사용자 추가 및 각 사용자에게 지정된 증명 역할 할당
* 기한 설정
* 스테이지가 활성화될 때 선택
* 완료 후 단계 잠금
* 하나의 결정만 필요
* 기본 의사 결정자 지정
* 외

자동화된 워크플로우 및 템플릿에 대한 자세한 내용은

* [자동화된 워크플로우 개요](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [자동화된 워크플로 템플릿 만들기 및 관리](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

## 증명 뷰어에서 GenStudio 초안 콘텐츠 검토 및 승인

증명 뷰어의 GenStudio에서 직접 GenStudio 초안 콘텐츠를 검토하고 승인할 수 있습니다.

증명 뷰어를 사용하여 다음 작업을 수행할 수 있습니다

* 댓글 남기기
* 초안을 마크업하여 변경해야 하는 항목 표시
* 결정

GenStudio의 검토 및 승인에 대한 자세한 내용은 <!--[Workfront Proof integration with GenStudio for Performance Marketing]().-->을(를) 참조하십시오.

## 최종 승인 및 게시를 위한 GenStudio의 검토 결정 보기

자산이 검토 및 승인 프로세스를 거치고 나면 검토 결정을 보고 GenStudio에서 직접 콘텐츠를 게시할 수 있습니다.

자세한 내용은 <!--[link to GS docs]().-->
