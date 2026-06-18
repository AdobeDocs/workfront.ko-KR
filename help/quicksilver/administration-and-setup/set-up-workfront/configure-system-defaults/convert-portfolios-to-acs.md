---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 레거시 포트폴리오를 Adobe 클라우드 스토리지로 변환
description: 시스템 환경 설정의 스토리지 환경 설정 영역에서 기존 레거시 Workfront 스토리지 포트폴리오를 Adobe 클라우드 스토리지로 변환합니다.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 5%

---

# 레거시 포트폴리오를 Adobe 클라우드 스토리지로 변환

Workfront 관리자는 시스템 환경 설정의 스토리지 환경 설정 영역에서 기존 기존 Workfront 스토리지 포트폴리오를 Adobe 클라우드 스토리지로 변환할 수 있습니다. 포트폴리오가 전환되면 다른 Adobe 클라우드 스토리지 포트폴리오와 동일하게 작동합니다.

변환된 포트폴리오의 동작 방식과 자식 개체가 영향을 받는 방법에 대한 자세한 내용은 [Adobe 클라우드 저장소의 Workfront으로 이동](/help/quicksilver/review-and-approve-work/workfront-storage.md)에서 [개체 이동성](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability)을(를) 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>모든 워크플로우 패키지</p></td> 
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

## 포트폴리오를 변환하기 전에

기존 Workfront 스토리지 포트폴리오를 변환하기 전에 다음 사항을 고려하십시오.

* 전환은 포트폴리오 자체에만 영향을 줍니다. 기존 Workfront 스토리지를 사용하는 하위 프로젝트 및 프로그램은 기존 스토리지에 유지됩니다.

  >[!NOTE]
  >
  >하위 레거시 프로그램은 Adobe 클라우드 스토리지 프로젝트를 수동으로 추가하는 경우에만 Adobe 클라우드 스토리지로 자동으로 변환됩니다.
* 포트폴리오의 문서 및 문서 폴더는 변환 후 레거시 Workfront 스토리지에 남아 있습니다.
* 변환 후에는 레거시 Workfront 스토리지 프로젝트를 포트폴리오에 추가할 수 없습니다.

## 레거시 포트폴리오를 Adobe 클라우드 스토리지로 변환

하나 이상의 기존 Workfront 스토리지 포트폴리오를 Adobe 클라우드 스토리지로 변환하려면 다음을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **시스템**&#x200B;을 선택한 다음 **기본 설정**&#x200B;을 선택하십시오.

1. **저장소 환경 설정** 섹션까지 아래로 스크롤합니다.

1. **Adobe 클라우드 저장소로 변환할 포트폴리오 선택** 필드에서 하나 이상의 레거시 Workfront 저장소 포트폴리오를 선택합니다.

1. **저장**&#x200B;을 클릭합니다.

   포트폴리오를 변환할 때 발생하는 작업을 설명하는 확인 메시지가 나타납니다.

   * 더 이상 레거시 Workfront 스토리지 프로젝트를 포트폴리오로 이동할 수 없습니다.
   * 포트폴리오에서 생성된 모든 새 프로젝트는 Adobe 클라우드 스토리지를 사용합니다.
   * Frame.io는 포트폴리오의 Adobe 클라우드 스토리지 프로젝트에 있는 문서의 뷰어입니다.
   * 기존 Workfront 스토리지를 사용하는 하위 프로젝트는 기존 스토리지에 유지됩니다.
   * 하위 프로그램은 기존 스토리지에 유지됩니다.

1. 확인하려면 **변환**&#x200B;을 클릭하세요.

   선택한 포트폴리오는 Adobe 클라우드 스토리지로 변환됩니다.
