---
product-area: documents
navigation-topic: approvals
title: Adobe 클라우드 스토리지의 차이점
description: 새 문서 영역, Frame.io 뷰어, 문서 권한, 개체 이름 지정 규칙, 저장소 할당량 및 Workfront Fusion을 포함하여 Adobe 클라우드 저장소 개체에 대한 주요 차이점을 이해합니다.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 120abd12533cfed2e5c7f8c2f849d34a26054dbb
workflow-type: tm+mt
source-wordcount: '1714'
ht-degree: 0%
---
# Adobe 클라우드 스토리지의 차이점

Adobe 클라우드 스토리지를 사용하면 기존 Workfront 스토리지에 있는 오브젝트(현재 보유 중인 오브젝트)와 Adobe 클라우드 스토리지를 사용하여 생성된 오브젝트의 두 가지 유형의 오브젝트를 환경에 포함할 수 있습니다. 새 문서 영역, Frame.io 뷰어 및 여기에 설명된 기타 동작은 Adobe 클라우드 스토리지를 사용하는 객체에만 적용됩니다.

이동 방향은 [Adobe 클라우드 저장소에서 Workfront으로 이동](/help/quicksilver/review-and-approve-work/workfront-storage.md)을 참조하십시오.

## 기존 Workfront 스토리지 및 Adobe 클라우드 스토리지 이해

상위 수준에서 두 스토리지 모델은 데이터가 어디에 있는지, 어떤 Adobe 제품이 볼 수 있는지, 어떤 기능을 사용할 수 있는지 다릅니다.

|  | 기존 Workfront 스토리지의 오브젝트 | Adobe 클라우드 스토리지의 오브젝트 |
|---|---|---|
| 스토리지 백엔드 | Workfront 전용 | Adobe 클라우드 스토리지 |
| 제품 간 가시성 | Workfront 전용 | Workfront, Frame.io 및 Creative Cloud |
| 기능 | 레거시 기능 | 새로운 기능 |

Adobe 클라우드 스토리지 이전에 생성된 객체는 기본적으로 기존 Workfront 스토리지에 남아 있습니다. 이 문서에 설명된 동작은 Adobe 클라우드 스토리지가 기본값이면 사용자와 사용자가 만드는 Adobe 클라우드 스토리지 개체에만 적용됩니다.

## 차이점 요약

Adobe 클라우드 스토리지의 가장 큰 일상적인 변경 사항은 새로운 문서 영역과 그 내에서 검토 및 승인을 지원하는 Frame.io 뷰어입니다. 객체, 문서 및 검토를 관리하는 방식에 영향을 주는 다른 차이점도 있습니다. 다음 표의 각 영역은 아래의 세부 섹션으로 연결됩니다.

| 영역 | 차이점 | 알아 두어야 할 사항 |
|---|---|---|
| [새 문서 영역](#the-new-documents-area) | 다시 디자인된 통합 문서 영역이 기존 문서 영역을 대체합니다. | 글로벌 문서 영역이 없습니다. 프로그램, 포트폴리오, 프로젝트, 작업 또는 문제의 문서에 액세스합니다. |
| [문서 권한](#document-permissions) | 문서는 연결된 프로젝트, 작업 또는 문제에서 권한을 상속합니다. | 개별 문서에 대한 권한을 공유하거나 설정할 수 없습니다. 시스템 생성 문서 폴더에 캐스케이드되는 Workfront의 공유 모달을 통해 모든 액세스를 관리합니다. |
| [개체 권한 매핑](#object-permissions-mapping) | 관리 및 기여 권한은 모두 Frame.io의 편집 및 공유에 매핑됩니다. 맵을 주석으로만 봅니다. | Workfront에서 권한을 관리합니다. Manage 및 Contribute 사용자는 모두 Frame.io에서 외부 공유 기능을 사용할 수 있습니다. |
| [검토 및 승인 뷰어](#review-and-approval-viewer) | Frame.io 뷰어는 Workfront Proofing 뷰어를 대체합니다. | 검토 또는 승인에 할당된 외부 사용자를 포함하여 모든 Workfront 사용자에 대해 포함됩니다. 마크업, 타임스탬프가 지정된 주석, 버전 기록, 모바일, 40개 이상의 형식 및 최대 500GB의 파일을 지원합니다. |
| [개체 명명 규칙](#object-naming-rules) | 엄격한 이름 지정 규칙이 적용됩니다. 포트폴리오 또는 프로젝트 내의 고유한 이름, 특수 문자 없음, 후행 기간 또는 공백 없음, 255자 제한 등이 있습니다. | Workfront은 충돌이 발생하면 오브젝트의 이름을 자동으로 바꿉니다. 새 프로젝트 이름 및 구조를 생성하는 템플릿을 감사합니다. |
| [개체 이동성](#object-portability) | 대부분의 시나리오에서는 같은 저장 장치 모델 사이에서만 개체를 이동, 복사 및 변환할 수 있습니다. | 세 가지 특정 경우에 레거시 개체를 Adobe 클라우드 스토리지로 변환할 수 있습니다. 문서 및 문서 폴더는 변환 중에 기존 스토리지에서 이동하지 않습니다. |
| [기능을 사용할 수 없음](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, Workfront 문서 뷰어, 즐겨 찾는 문서 및 요청 문서는 경험의 일부가 아닙니다. | 기존 객체에는 이러한 기능이 유지됩니다. Workfront Proof은 새로운 투자를 받지 않으며 향후 릴리스에서 중단될 예정입니다. |
| [저장소 할당량](#storage-quota) | 스토리지는 하드 캡 없이 라이선스가 부여된 사용자당 60GB로 레거시 Workfront 프로젝트 및 Adobe 클라우드 스토리지 프로젝트용으로 풀링됩니다. | 시스템 관리자는 설정 의 고객 정보 페이지에서 스토리지 사용량을 볼 수 있습니다. |
| [연간 비디오 리뷰 상한](#annual-video-review-cap) | 유료 Workfront 사용자 라이선스(표준 및 라이트)의 10%에 비디오 증명 요청에 대한 조직 수준의 상한이 있습니다. | 상한선에 도달하면 다음 연간 기간까지 새 비디오 리뷰를 만들 수 없습니다. 80% 및 100%의 인앱 알림을 받습니다. Frame.io Enterprise 고객에게는 캡이 적용되지 않습니다. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | 기존 증명 기반 Fusion 시나리오는 Adobe 클라우드 스토리지 프로젝트에 대해 자동으로 작동하지 않습니다. | 레거시 프로젝트에 범위가 지정된 시나리오가 계속 작동합니다. 영향을 받는 각 시나리오는 편집, 다시 빌드 또는 사용 중지의 세 가지 경로 중 하나를 사용합니다. |

## 새 문서 영역

새 문서 영역은 Adobe 클라우드 스토리지용으로 설계된 통합 문서 환경입니다. 탐색을 단순화하고 검토 및 승인 활동을 통합하며 Frame.io 뷰어의 진입점입니다.

글로벌 문서 영역은 새 경험의 일부가 아닙니다. Adobe 클라우드 스토리지 프로젝트에서는 프로그램, 포트폴리오, 프로젝트, 작업 또는 문제의 문서에 액세스합니다.

자세한 내용은 [문서 영역](/help/quicksilver/documents/managing-documents/documents-area.md)을 참조하세요.

## 문서 권한

문서 권한은 Adobe 클라우드 스토리지 프로젝트에서 기본적으로 다릅니다.

* 개별 문서에 대한 권한을 공유하거나 설정할 수 없습니다. 대신 문서가 포함된 시스템 생성 문서 폴더에 권한이 적용됩니다.
* 시스템 생성 문서 폴더는 상위 프로젝트, 작업 또는 문제에서 권한을 상속합니다.
* 하위 폴더는 상위 시스템에서 생성한 문서 폴더에서 권한을 상속합니다.
* 하위 작업은 상위 작업에서 권한을 상속하지 않습니다. 시스템에서 생성한 문서 폴더에 액세스하려면 하위 작업에 직접 추가해야 합니다.

문서 권한이 작동하는 방식에 대한 자세한 내용은 [Adobe 클라우드 저장소 모델에 대한 개체 권한 및 액세스 수준 개요](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)를 참조하십시오.

## 개체 권한 매핑

권한은 Workfront에서 설정되고 Frame.io를 통해 한 방향으로 흐릅니다. Frame.io에서 Adobe 클라우드 스토리지 프로젝트에 사용자를 초대하거나 Frame.io에서 사용자 권한을 수정할 수 없습니다.

>[!TIP]
>
>프로젝트 코디네이터에게 Frame.io 액세스가 Workfront 권한의 다운스트림 반영임을 교육합니다. 관련자가 Adobe 클라우드 스토리지 프로젝트에 대한 검토에 액세스할 수 없다고 보고하면 수정 사항은 Frame.io가 아니라 Workfront에 있습니다.

다음 표에서는 Workfront 개체 권한을 Frame.io 권한에 매핑합니다.

| Workfront 권한 | Frame.io 권한 |
|---|---|
| 관리 | 편집 및 공유 |
| 참여 | 편집 및 공유 |
| 보기 | 주석만 |

관리 및 기여 모두 Frame.io에서 편집 및 공유에 매핑됩니다. Adobe 클라우드 스토리지 프로젝트에 대한 공유 패턴을 검토할 때 기여자가 외부 공유를 포함하여 관리자와 동일한 검토 측 기능을 갖도록 하는 것이 귀사의 거버넌스 모델에 적합한지 여부를 고려하십시오.

자세한 내용은 [Adobe 클라우드 저장소 모델에 대한 개체 권한 및 액세스 수준 개요](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio)를 참조하십시오.

## 검토 및 승인 뷰어

Adobe 클라우드 스토리지 개체에서 Frame.io 뷰어는 Workfront Proof 대신 검토 및 승인 화면입니다. Frame.io 뷰어는 검토 또는 승인에 할당된 외부 사용자를 포함하여 추가 비용 없이 모든 Workfront 사용자에 대해 포함됩니다.

Frame.io 뷰어는 다음을 제공합니다.

* 원, 화살표, 사각형과 같은 표준 모양과 자유 형식 드로잉을 포함한 마크업 및 주석 도구
* 비디오 검토를 위해 프레임 수준의 정확한 정밀도로 타임스탬프가 지정된 주석
* 버전 기록 및 버전 비교
* [Frame.io iOS 앱](https://help.frame.io/en/collections/9679120-ios-app)을 통해 이동 중 검토 및 승인을 위한 모바일 액세스
* ProRes, H.265, DNxHD와 같은 전문 비디오 형식에 대한 기본 재생과 함께 모든 일반 비디오, 이미지, 오디오, PDF, Microsoft Office 유형을 포함한 40개 이상의 파일 형식 지원 및 최대 500GB의 파일 지원

## 객체 이름 지정 규칙

Adobe 클라우드 스토리지는 엄격한 이름 지정 및 구조 규칙을 적용하여 Adobe 제품 전반에서 스토리지 레이어를 일관되게 유지합니다. 이러한 규칙은 Adobe 클라우드 스토리지 프로젝트에서 만드는 개체에 적용됩니다. 기존 레거시 프로젝트는 현재 이름을 유지합니다.

Adobe 클라우드 스토리지 프로젝트에는 다음 규칙이 적용됩니다.

| 규칙 | 세부 사항 |
|---|---|
| 고유 프로그램 및 프로젝트 이름 | 프로그램 및 프로젝트가 동일한 포트폴리오에 속하는 경우 동일한 이름을 가질 수 없습니다. |
| 고유 문서 이름 | 문서가 동일한 프로젝트에 속하는 경우 문서의 이름이 같을 수 없습니다. 문서 이름은 폴더 계층의 동일한 상위 항목에서 고유해야 합니다. |
| 금지된 문자 | 프로그램, 포트폴리오, 프로젝트, 템플릿, 작업, 문제, 문서 폴더 및 문서에는 다음 특수 문자를 사용할 수 없습니다. `\ / : * ? " \| < >` |
| 후행 문자 | 프로그램, 포트폴리오, 프로젝트, 템플릿, 작업, 문제 및 문서 폴더에는 마침표나 공백으로 끝나는 이름을 사용할 수 없습니다. |
| 이름 길이 제한 | 개체 이름은 255자로 제한됩니다. |

이름이 이러한 규칙과 충돌하는 경우 Workfront은 충돌을 해결하기 위해 자동으로 오브젝트의 이름을 바꿉니다.

>[!TIP]
>
>템플릿에서 Adobe 클라우드 스토리지 프로젝트를 만드는 경우 기존 템플릿을 검토하여 위에서 규정한 규칙에 맞게 프로젝트 이름과 구조를 생성하십시오.

## 객체 이동성

대부분의 시나리오에서는 와 같은 스토리지 모델 사이에서만 Workfront 개체를 이동, 복사 및 변환할 수 있습니다. 예를 들어 작업을 한 Adobe 클라우드 스토리지 프로젝트에서 다른 Adobe 클라우드 스토리지 프로젝트로 이동할 수 있습니다. 세 가지 특정 경우에 기존 Workfront 스토리지 개체를 Adobe 클라우드 스토리지로 변환할 수 있습니다.

<!--
During a group-scoped rollout, only members of the group that has Adobe cloud storage can convert an Adobe cloud storage object, such as a request, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."

For more information, see [Plan your Adobe cloud storage rollout](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md).
-->

자세한 내용은 [레거시 개체를 Adobe 클라우드 저장소로 변환](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md)을 참조하십시오.

## Adobe 클라우드 스토리지 개체에서 사용할 수 없는 기능

다음 기능은 Adobe 클라우드 스토리지 개체의 일부가 아닙니다.

* Workfront Proof
* Workfront 문서 뷰어
* 즐겨 찾는 문서
* 요청 문서

레거시 프로젝트는 위에 나열된 Workfront Proof 및 레거시 문서 기능에 대한 액세스 권한을 유지합니다. Workfront Proof은 향후 새로운 투자를 받지 않으며 향후 릴리스에서 중단될 예정입니다.

## 저장소 할당량

스토리지는 기존 Workfront 개체 및 Adobe 클라우드 스토리지 개체에 대해 풀링됩니다. 각 라이센스 사용자는 60GB의 스토리지를 받습니다. 스토리지 사용량에 대한 하드 캡은 없지만 할당량의 75%, 90%, 100%에 도달하면 Workfront 관리자가 이메일 알림을 받습니다.

현재 저장소 사용량 및 할당량을 보려면 **설정** > **시스템** > **고객 정보**(으)로 이동하세요.

자세한 내용은 [문서 저장소 제한 확인](/help/quicksilver/documents/managing-documents/check-document-storage.md)을 참조하세요.

## 연간 비디오 리뷰 상한

조직의 총 유료 Workfront 사용자 라이선스(표준 및 라이트)의 10%로 설정된 비디오 증명 요청에 대한 연간 상한이 있습니다. 이 상한은 조직 수준에서 적용됩니다.

* Workfront 관리자는 사용량이 상한의 80% 및 100%에 도달하면 인앱 알림을 받습니다.
* 상한에 도달하면 다음 연간 기간까지 새 비디오 검토 요청을 만들 수 없습니다.
* 이 제한은 Frame.io Enterprise 고객에게는 적용되지 않습니다. 조직에서 대량의 비디오 콘텐츠를 정기적으로 검토하는 경우 Adobe 계정 담당자에게 문의하여 Frame.io Enterprise 라이선싱에 대해 알아보십시오.

자세한 내용은 [통합 검토 및 승인 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)에서 에셋 및 비디오 검토 및 승인 FAQ를 참조하십시오.

## Adobe 클라우드 스토리지 프로젝트의 Workfront Fusion

레거시 증명을 기반으로 구축된 기존 Workfront Fusion 시나리오는 Adobe 클라우드 스토리지 프로젝트에 대해 자동으로 작동하지 않습니다. 증명별 모듈, 웹후크 및 API 엔드포인트는 경우에 따라 직접적인 등가물을 가지며 다른 경우에는 상당한 변경을 가집니다. 레거시 프로젝트에 범위가 지정된 시나리오는 오늘날과 같이 계속 작동합니다.

일반적인 시나리오 유형에 미치는 영향 및 각 시나리오를 해당 기능을 기반으로 편집, 다시 빌드 또는 사용 중지로 분류하는 방법에 대한 자세한 내용은 [통합 검토 및 승인을 위해 Workfront Fusion 시나리오 업데이트](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)를 참조하십시오.
