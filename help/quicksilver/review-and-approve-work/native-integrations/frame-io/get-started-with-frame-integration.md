---
product-area: documents
navigation-topic: approvals
title: Frame.io 통합 시작
description: Frame.io 통합을 시작합니다.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b9a83bc2-4dd8-4c77-a2e7-385baa809b3b
source-git-commit: a3edfadc447a763c638cc926b386272890697f81
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# Frame.io 통합 시작

Workfront과 Frame.io 통합을 통해 크리에이티브, 마케터 및 이해 당사자를 원활한 워크플로우로 연결할 수 있습니다. 시작 전에 실시간 업데이트에 액세스하고, 중복 작업을 방지하고, 자산이 승인되도록 합니다.

Frame.io에 대한 자세한 내용은 [Frame.io 시작하기](https://support.frame.io/en/collections/49298-getting-started)를 참조하십시오.

Workfront 인스턴스에 Workfront 및 Frame.io 통합이 설정되어 있어야 합니다. 자세한 내용은 [Frame.io 통합 개요](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md#integration-requirements)를 참조하십시오.

<!--## Integration requirements

* Workfront and Frame.io must be deployed to the same Identity Management system (IMS) organization.

* Users can belong to only one Workfront instance within the IMS organization.

* The Workfront instance must be enabled on the Adobe Unified Experience.

* The integration is configured by Adobe Professional Services. -->

## Workfront의 작업 시작 및 계획

프로젝트 코디네이터는 Workfront에서 프로젝트를 만들고 작업을 계획할 수 있습니다. Frame.io 통합이 활성화된 인스턴스에서 만든 프로젝트는 Adobe 에코시스템 내에서 에셋을 저장하고 관리할 수 있는 Adobe Enterprise Storage를 사용합니다.

조직에 Frame.io Enterprise 라이센스가 있는 경우 Workfront에서 만든 프로젝트도 Frame.io에 표시되므로 사용자가 두 제품 중 하나에서 자산을 상호 작용하고 업로드할 수 있습니다.

Adobe Enterprise Storage 또는 Frame.io의 프로젝트에 대한 자세한 내용은

* [Workspace 개요: 프로젝트](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Adobe 엔터프라이즈 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)

## 에셋 검토 및 승인

에셋이 완료되면 프로젝트 코디네이터는 Workfront에서 공식 검토 및 승인 프로세스를 시작할 수 있습니다.

승인 워크플로가 만들어지면 검토자와 승인자는 Frame.io 뷰어를 사용하여 주석을 추가하고 에셋을 표시할 수 있습니다. Frame.io 뷰어에서 승인 결정을 내릴 수도 있습니다.

프로젝트 설정에 대한 자세한 내용은

* [프로젝트 만들기](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
* [Frame.io 통합 개요](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)

### Workfront에서 공식 검토 및 승인 시작

프로젝트 코디네이터는 일회성 검토 및 승인 또는 재생성 가능한 승인 템플릿을 생성할 수 있습니다. 검토자, 승인자 또는 두 가지 모두를 혼합하여 할당할 수 있습니다.

* **검토자**&#x200B;이(가) 댓글을 추가하고 자산을 표시할 수 있습니다. 완료되면 검토를 완료된 것으로 표시할 수 있습니다. 에셋이 승인 프로세스에서 앞으로 이동하기 위해서는 검토를 완료로 표시할 필요가 없습니다.
* **승인자**&#x200B;는 댓글을 추가하고 자산을 표시할 수 있습니다. 그들은 승인 절차를 진행하기 위해 결정을 내려야 한다.

#### 검토 및 승인 워크플로우 만들기

검토자와 승인자를 일회용 승인 워크플로 또는 재사용 가능한 승인 템플릿에 추가할 수 있습니다.

* **단일 사용 승인**: 에셋이 있는 프로젝트 또는 작업에서 프로젝트 코디네이터는 검토자와 승인자를 할당하고 완료 기한을 설정할 수 있습니다. 검토자와 승인자는 기한 72시간 전, 기한 24시간 전, 그리고 기한 자체에 이메일로 알림을 받습니다.

  자세한 내용은 [문서 검토 또는 승인 요청 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

* **승인 템플릿**: Workfront 설정 영역에서 프로젝트 코디네이터가 다시 사용할 수 있는 승인 템플릿을 만들 수 있습니다. 템플릿 내에서 검토자와 승인자를 추가하고 완료 기간을 지정할 수 있습니다. 승인 템플릿이 에셋에 적용되면 기한은 지정된 시간대에서 계산됩니다.

  템플릿이 생성되면 자산에 적용하여 Workfront에서 공식 검토 및 승인 프로세스를 시작할 수 있습니다.

  자세한 내용은 [승인 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)를 참조하세요.


  ![템플릿 할당](assets/assign-template.png)

### Frame.io 뷰어에서 자산 검토 및 승인

Workfront에서 검토 및 승인 워크플로가 시작되면 검토자와 승인자는 Frame.io 뷰어에 액세스하여 주석을 추가하고 에셋을 표시한 다음 결정을 내릴 수 있습니다.

자세한 내용은 [Frame.io 뷰어로 검토 및 승인](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)을 참조하세요.

#### Frame.io 뷰어 액세스

사용자는 다음과 같은 방법으로 Frame.io 뷰어에 액세스할 수 있습니다.

* Workfront 이메일 알림
* Workfront 홈 영역의 내 승인 위젯

>[!NOTE]
>
>외부 Workfront 사용자는 이메일을 통해 알림을 받으며 에셋을 검토하고 승인하기 위해 Frame.io 로그인을 만들라는 요청을 받게 됩니다.

![홈에서 프레임 뷰어를 엽니다](assets/open-fio-viewwer.png)

#### 댓글 추가 및 자산 표시

주석 및 에셋 마크업이 Frame.io 뷰어에 표시됩니다. Frame.io 뷰어 사용에 대한 자세한 내용은 [미디어에 주석 달기](https://help.frame.io/en/articles/9105251-commenting-on-your-media)를 참조하십시오.

#### 결정

모든 검토 활동이 완료되면 승인자는 다음 결정 중 하나를 내려야 합니다.

* **승인**: 자산은 변경할 필요가 없으며 사용할 준비가 되었습니다.
* **작업 필요**: 자산을 변경해야 하며 사용할 준비가 되지 않았습니다. 지정된 변경 사항이 적용되면 에셋을 새 버전으로 업로드하고 다른 승인을 거쳐야 합니다. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

검토자는 Workfront 내에서 검토 완료를 표시할 수 있지만 승인 프로세스에서 에셋이 앞으로 진행되는 데에는 필요하지 않습니다.

Workfront의 의사 결정에 대한 자세한 내용은 [문서 의사 결정 상태 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)를 참조하십시오.

![프레임 뷰어 및 결정](assets/decision-fio.png)


### 검토 및 승인 지표 추적

프로젝트 코디네이터는 Workfront 홈 영역에서 모든 진행 중인 승인의 진행 상황을 모니터링하거나 캔버스 대시보드의 사용자 정의된 보고서를 모니터링할 수 있습니다.

* **사용자 지정 대시보드**: [캔버스 대시보드] 영역에 보고서 대시보드를 만들어 통합 승인 기능을 사용한 검토 및 승인에 대한 고급 정보와 자세한 정보를 모두 표시합니다. 시작하는 방법에 대한 자세한 내용은 [검토 및 승인을 위한 보고서 대시보드 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)를 참조하세요.
* **문서 승인 지표 홈 위젯**: 평균 승인 시간 및 결정과 보류 중인 승인 및 기한이 지난 승인의 목록 보기에 대한 정보가 포함된 2개의 차트를 표시합니다.
  ![모든 승인](assets/all-approvals.png)