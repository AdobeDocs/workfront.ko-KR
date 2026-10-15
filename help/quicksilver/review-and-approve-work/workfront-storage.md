---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Adobe 클라우드 스토리지의 Workfront으로 이동
description: Adobe 클라우드 스토리지에서 Workfront으로의 이동을 계획합니다. 조직이 활성화될 때 발생하는 일, Adobe 클라우드 스토리지 개체의 차이점 및 고유한 타이밍에 롤아웃하는 방법을 이해합니다.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---
# Adobe 클라우드 스토리지의 Workfront으로 이동

Adobe 클라우드 스토리지의 Workfront은 Frame.io 뷰어의 검토, 강력한 승인 워크플로, 자산에 대한 제품 간 가시성 등과 같은 전체 통합 검토 및 승인 경험을 제공합니다.

이 문서는 Adobe 클라우드 스토리지로 이동하는 Workfront 관리자의 시작점입니다. Adobe 클라우드 스토리지를 활성화하면 어떤 일이 발생하는지 설명하고, 차이점에 대한 세부 정보를 안내하며, 변경을 계획하고 실행하는 데 도움이 되는 문서에 대한 링크를 제공합니다.

## Adobe 클라우드 스토리지가 켜지는 시기를 결정합니다.

Workfront 관리자가 **설정** > **시스템** > **환경 설정**&#x200B;에서 Adobe 클라우드 저장소를 기본 저장소 옵션으로 사용하도록 설정할 때까지 Workfront 환경이 변경되지 않습니다. 그때까지 기존 프로젝트 및 새로 만드는 모든 프로젝트는 레거시 Workfront 스토리지에 유지되며 현재 사용하는 승인 서비스를 유지합니다.

관리자가 Adobe 클라우드 스토리지를 기본 스토리지 옵션으로 활성화하는 경우:

* 새 프로젝트에서 Adobe 클라우드 스토리지 사용
* Frame.io가 기본 뷰어입니다.
* 통합 승인이 기본 승인 서비스입니다.

기존 프로젝트는 변경되지 않습니다.

타이밍을 제어하므로 누구나 작업을 하기 전에 경험을 테스트하고, Workfront Fusion 시나리오를 업데이트하고, 변경 사항 보고를 위한 계획을 세울 수 있습니다. 단계별 지침은 [조직에 Adobe 클라우드 저장소 사용](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)을 참조하십시오.

## Adobe 클라우드 스토리지에서 승인이 작동하는 방식

Adobe 클라우드 스토리지 프로젝트는 기본적으로 Frame.io 뷰어에서 검토 및 승인과 함께 통합 승인을 사용합니다. 기존 Workfront 스토리지에 있는 오브젝트는 기존 문서 승인 또는 통합 승인과 같이 이미 사용하는 모든 승인 서비스를 유지합니다.

>[!NOTE]
>
>Adobe 클라우드 스토리지를 기본값으로 설정해도 기존 Workfront 스토리지 개체에서 이미 사용 중인 승인 서비스는 변경되지 않습니다. 통합 승인은 Adobe 클라우드 스토리지에서 생성된 새 오브젝트에 대한 기본값입니다.

Adobe 클라우드 스토리지를 롤아웃하기 전에 승인을 관리하는 사용자에게 예상 내용을 알려야 합니다. 자세한 내용은 [기존 문서 승인에서 통합 승인으로 이동](/help/quicksilver/review-and-approve-work/move-to-unified-approvals.md)을 참조하십시오.

## 이동 계획

다음 문서를 준비하면서 순서대로 진행합니다.

* [Adobe 클라우드 스토리지의 차이점](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md): 새 문서 영역과 Frame.io 뷰어에서 이름 지정 규칙, 저장소 할당량 및 Fusion에 이르기까지 Adobe 클라우드 스토리지 개체의 주요 차이점.
* [Adobe 클라우드 저장소 롤아웃을 계획합니다](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md): 롤아웃 구성을 선택하고 단일 그룹으로 테스트하며 사용자를 위해 예기치 않은 작업이 없도록 작업 순서를 지정하는 방법.
* [조직에 Adobe 클라우드 저장소를 사용하도록 설정](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md): 전체 조직 또는 특정 그룹에 대한 기본 저장소 옵션을 설정하는 단계입니다.
* [기존 개체를 Adobe 클라우드 저장소로 변환](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md): 기존 개체를 Adobe 클라우드 저장소로 변환할 수 있는 세 가지 경우와 각 변환 중 이동되는 사항.


## 관련 문서

* [Adobe 클라우드 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [통합 검토 및 승인 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [문서 영역](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Adobe 클라우드 스토리지 모델에 대한 개체 권한 및 액세스 수준 개요](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)
