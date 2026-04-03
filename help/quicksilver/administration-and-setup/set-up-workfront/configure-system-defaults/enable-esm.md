---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 귀사를 위한 Adobe 엔터프라이즈 스토리지 활성화
description: 조직에서 모든 Adobe 제품에 통합 스토리지 솔루션을 사용하도록 Adobe 엔터프라이즈 스토리지를 설정할 수 있습니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 5%

---

# 조직을 위한 Adobe 엔터프라이즈 스토리지 활성화

Adobe 엔터프라이즈 스토리지는 모든 Adobe 제품을 위한 통합 스토리지 솔루션입니다. Adobe 엔터프라이즈 제품 전반에 걸쳐 에셋의 중앙 저장소 역할을 하는 클라우드 기반 스토리지 솔루션입니다.

Adobe 엔터프라이즈 스토리지는 신규 고객에 대해 기본적으로 활성화되고 계약 갱신 시 기존 고객에 대해 활성화될 수 있습니다.

Adobe 엔터프라이즈 스토리지에 대한 자세한 내용은 [Adobe 엔터프라이즈 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p> <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>Workfront 관리자여야 합니다. </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 조직을 위한 Adobe 엔터프라이즈 스토리지 활성화

조직에 Adobe 엔터프라이즈 스토리지를 활성화하려면 다음을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **시스템**&#x200B;을 선택한 다음 **기본 설정**&#x200B;을 선택하십시오.
1. **저장소 환경 설정** 섹션까지 아래로 스크롤합니다.
1. 기본 드롭다운 메뉴에서 **Adobe 엔터프라이즈 스토리지**&#x200B;를 선택합니다.
1. (선택 사항) Adobe 엔터프라이즈 스토리지와 레거시 Workfront 스토리지를 함께 사용하려면 **사용자가 스토리지 공급자를 선택할 수 있도록 허용** 확인란을 선택하십시오.

   >[!NOTE]
   >
   >이 옵션을 활성화하면 사용자가 새 프로젝트를 만들 때 스토리지 공급자를 선택할 수 있습니다. 엔터프라이즈 스토리지는 기본 스토리지 제공업체이므로 &quot;새 프로젝트&quot;로 레이블이 지정됩니다. 레거시 Workfront 스토리지는 &quot;레거시 프로젝트&quot;로 레이블이 지정됩니다.
   >
   >![새 프로젝트 및 레거시 프로젝트 옵션](assets/new-esm-project.png)

1. 적용 대상 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.

   - **전체 조직**: 이 옵션은 기본 저장소 공급자를 전체 Workfront 환경에 적용합니다. 사용자가 새 프로젝트를 만들 때마다 기본 저장소 공급자가 사용됩니다.
   - **특정 그룹**: 이 옵션은 조직 내의 특정 그룹에만 기본 저장소 공급자를 적용합니다. 지정된 그룹의 사용자가 새 프로젝트를 만들 때마다 기본 저장소 공급자가 사용됩니다.

1. **저장**&#x200B;을 클릭합니다.
