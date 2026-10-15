---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: 레거시 개체를 Adobe 클라우드 스토리지로 변환
description: 기존 Workfront 스토리지 개체를 Adobe 클라우드 스토리지로 변환할 수 있는 세 가지 경우를 알아보고 각 변환 동안 이동되는 내용과 유지되는 내용을 이해합니다.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---
# 레거시 개체를 Adobe 클라우드 스토리지로 변환

대부분의 시나리오에서는 와 같은 스토리지 모델 사이에서만 Workfront 개체를 이동, 복사 및 변환할 수 있습니다. 예를 들어 작업을 한 Adobe 클라우드 스토리지 프로젝트에서 다른 Adobe 클라우드 스토리지 프로젝트로 이동할 수 있습니다. 다음과 같은 세 가지 특정 경우에 기존 Workfront 스토리지 개체를 Adobe 클라우드 스토리지로 변환할 수 있습니다.

* 레거시 Workfront 스토리지 작업을 Adobe 클라우드 스토리지 프로젝트로 전환
* 기존 Workfront 스토리지 포트폴리오를 Adobe 클라우드 스토리지 포트폴리오로 변환
* 기존 Workfront 스토리지 템플릿에서 Adobe 클라우드 스토리지 프로젝트 만들기

이동 방향과 Adobe 클라우드 스토리지의 차이점에 대해서는 [Adobe 클라우드 스토리지로 Workfront 이동](/help/quicksilver/review-and-approve-work/workfront-storage.md)을 참조하십시오.

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## 레거시 작업을 Adobe 클라우드 스토리지 프로젝트로 전환

기존 Workfront 스토리지 작업을 Adobe 클라우드 스토리지 프로젝트로 변환하려면 작업에 대한 기존 프로젝트 간 변환 흐름을 사용하십시오. 전환 중:

* 하위 작업 및 문제가 새 프로젝트로 이동합니다.
* 작업 및 해당 승인 워크플로에 첨부된 문서는 원래 프로젝트에 유지됩니다.
* 작업 승인 및 해결 중 오브젝트 링크가 제거됩니다.
* 원래 작업이 삭제됩니다.

## 레거시 포트폴리오를 Adobe 클라우드 스토리지 포트폴리오로 변환

Workfront 관리자는 설정 영역에서 기존 Workfront 스토리지 포트폴리오를 Adobe 클라우드 스토리지 포트폴리오로 변환할 수 있습니다. 전환 후:

* 더 이상 레거시 Workfront 스토리지 프로젝트를 포트폴리오로 이동할 수 없습니다.
* 포트폴리오에서 생성된 모든 새 프로젝트는 Adobe 클라우드 스토리지를 사용합니다.
* Frame.io는 포트폴리오의 Adobe 클라우드 스토리지 프로젝트에 있는 문서의 뷰어입니다.
* 기존 Workfront 스토리지를 사용하는 하위 프로젝트는 기존 스토리지에 유지됩니다.
* 하위 프로그램은 기존 스토리지에 유지됩니다.

>[!NOTE]
>
>하위 레거시 프로그램은 Adobe 클라우드 스토리지 프로젝트를 수동으로 추가하는 경우에만 Adobe 클라우드 스토리지로 자동으로 변환됩니다.

자세한 내용은 [레거시 포트폴리오를 Adobe 클라우드 스토리지로 변환](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md)을 참조하십시오.

## 레거시 템플릿에서 Adobe 클라우드 스토리지 프로젝트 만들기

기존 Workfront 저장소 템플릿에서 프로젝트를 만들 때 프로젝트 만들기 대화 상자의 **Adobe 클라우드 저장소에서 이 프로젝트 만들기** 확인란이 새 프로젝트의 저장소 유형을 결정합니다. 확인란 동작은 프로젝트를 만드는 위치에 따라 다릅니다.

* **포트폴리오 외부**: 기본적으로 확인란을 사용할 수 있고 선택을 취소할 수 있습니다. Adobe 클라우드 스토리지에서 새 프로젝트를 만들려면 선택하십시오.
* **Adobe 클라우드 저장소 포트폴리오 내부**: 확인란이 선택되어 있고 잠겨 있습니다. 새 프로젝트는 포트폴리오의 스토리지 유형과 일치해야 합니다.
* **기존 Workfront 저장소 포트폴리오 내**: 확인란을 사용할 수 없습니다. 새 프로젝트는 기존 Workfront 스토리지를 사용합니다.

자세한 내용은 [프로젝트 만들기](/help/quicksilver/manage-work/projects/create-projects/create-project.md)를 참조하십시오.
