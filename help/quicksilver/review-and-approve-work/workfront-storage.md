---
product-area: documents
navigation-topic: approvals
title: Adobe 클라우드 스토리지의 Workfront으로 이동
description: Adobe 클라우드 스토리지에서 Workfront 롤아웃을 계획합니다. 새 문서 영역 및 Frame.io 검토 환경을 포함하여 Adobe 클라우드 스토리지 개체에 대한 차이점을 알아보고 Adobe 클라우드 스토리지가 환경에서 롤아웃되는 방법을 결정합니다.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 12242501adb13cd349a2282996c7186e90d6c94d
workflow-type: tm+mt
source-wordcount: '2375'
ht-degree: 0%

---

# Adobe 클라우드 스토리지의 Workfront으로 이동

Adobe 클라우드 스토리지의 Workfront을 사용하면 Frame.io 뷰어의 검토, 강력한 승인 워크플로, 자산에 대한 제품 간 가시성 등과 같은 전체 통합 검토 및 승인 경험을 사용할 수 있습니다.

기존 오브젝트는 오늘날과 같은 방식으로 계속 작동합니다. 새 문서 영역, Frame.io 뷰어 및 기타 Adobe 클라우드 스토리지 동작은 Adobe 클라우드 스토리지를 사용하는 객체에만 적용됩니다.

이 문서는 Adobe 클라우드 스토리지에서 Workfront을 롤아웃하려는 Workfront 관리자를 위한 것입니다. 이 섹션에서는 사용자를 위해 Adobe 클라우드 스토리지를 활성화하기 전에 Adobe 클라우드 스토리지 개체에 대한 주요 차이점, 롤아웃 유형을 선택하는 방법 및 고려해야 할 사항에 대해 다룹니다.

>[!IMPORTANT]
>
>Adobe 클라우드 스토리지를 지원하는 Workfront 버전을 사용해야 합니다. 조직이 이미 지원되는 버전을 사용하고 있지 않은 경우 Adobe 계정 담당자에게 문의하십시오.



## 기존 Workfront 스토리지 및 Adobe 클라우드 스토리지 이해

새로운 통합 검토 및 승인 환경을 포함하도록 계약이 업데이트되면 환경에는 기존 Workfront 스토리지에 있는 개체(현재 보유하고 있는 개체)와 Adobe 클라우드 스토리지를 사용하여 생성된 개체, 이렇게 두 가지 유형의 개체가 포함될 수 있습니다. 상위 수준에서 두 스토리지 모델은 데이터가 어디에 있는지, 어떤 Adobe 제품이 볼 수 있는지, 어떤 기능을 사용할 수 있는지 다릅니다.

|  | 기존 Workfront 스토리지의 오브젝트 | Adobe 클라우드 스토리지의 오브젝트 |
|---|---|---|
| 스토리지 백엔드 | Workfront 전용 | Adobe 클라우드 스토리지 |
| 제품 간 가시성 | Workfront 전용 | Workfront, Frame.io 및 Creative Cloud |
| 기능 | 레거시 기능 | 새로운 기능 |

설정 영역에서 Adobe 클라우드 스토리지가 활성화되기 전에 생성된 오브젝트는 기존 Workfront 스토리지에 유지됩니다. 이 문서에 설명된 새로운 동작은 Adobe 클라우드 스토리지가 활성화되면 사용자와 사용자가 만드는 Adobe 클라우드 스토리지 개체에만 적용됩니다.

## Adobe 클라우드 스토리지의 차이점

Adobe 클라우드 스토리지의 가장 큰 일상적인 변경 사항은 새로운 문서 영역과 그 내에서 검토 및 승인을 지원하는 Frame.io 뷰어입니다. 객체, 문서 및 검토를 관리하는 방식에 영향을 주는 다른 차이점도 있습니다.

다음 표에는 Adobe 클라우드 스토리지로 전환할 때의 주요 차이점이 요약되어 있습니다. 표의 각 영역은 아래의 세부 섹션으로 연결됩니다.

| 영역 | 차이점 | 알아 두어야 할 사항 |
|---|---|---|
| [새 문서 영역](#the-new-documents-area) | 다시 디자인된 통합 문서 영역이 기존 문서 영역을 대체합니다. | 글로벌 문서 영역이 없습니다. 프로그램, 포트폴리오, 프로젝트, 작업 또는 문제의 문서에 액세스합니다. |
| [문서 권한](#document-permissions) | 문서는 연결된 프로젝트, 작업 또는 문제에서 권한을 상속합니다. | 개별 문서에 대한 권한을 공유하거나 설정할 수 없습니다. 시스템 생성 문서 폴더에 캐스케이드되는 Workfront의 공유 모달을 통해 모든 액세스를 관리합니다. |
| [개체 권한 매핑](#object-permissions-mapping) | Workfront의 관리 및 기여 권한은 모두 Frame.io의 편집 및 공유에 매핑됩니다. 맵을 주석으로만 봅니다. | 권한은 Workfront에서 관리됩니다. Manage 및 Contribute 사용자는 모두 Frame.io에서 외부 공유 기능을 사용할 수 있습니다. |
| [검토 및 승인 뷰어](#review-and-approval-viewer) | Frame.io 뷰어는 Workfront Proofing 뷰어를 대체합니다. | 검토 또는 승인에 할당된 외부 사용자를 포함하여 모든 Workfront 사용자에 대해 포함됩니다. 마크업, 타임스탬프가 지정된 주석, 버전 기록, 모바일, 40개 이상의 형식, 최대 500GB의 파일을 지원합니다. |
| [개체 명명 규칙](#object-naming-rules) | 엄격한 이름 지정 규칙이 적용됩니다. 포트폴리오 또는 프로젝트 내의 고유한 이름, 특수 문자 없음, 후행 기간 또는 공백 없음, 255자 제한. | Workfront은 충돌이 발생할 때 오브젝트의 이름을 자동으로 바꿉니다. 새 프로젝트 이름 및 구조를 생성하는 감사 템플릿. |
| [개체 이동성](#object-portability) | 저장 모델과 같은 개체 사이에서만 개체를 이동, 복사 및 변환할 수 있습니다. | Adobe 클라우드 스토리지 개체는 이전 프로젝트로 이동하거나 그 반대로 이동할 수 없습니다. Adobe 클라우드 스토리지 프로젝트를 레거시 포트폴리오 또는 프로그램으로 이동하면 상위 클라우드 스토리지가 Adobe 클라우드 스토리지로 변환됩니다. |
| [기능을 사용할 수 없음](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, Workfront 문서 뷰어, 즐겨 찾는 문서 및 요청 문서는 경험의 일부가 아닙니다. | 기존 객체에는 이러한 기능이 유지됩니다. Workfront Proof은 새로운 투자를 받지 않으며 향후 릴리스에서 중단될 예정입니다. |
| [저장소 할당량](#storage-quota) | 스토리지는 기존 Workfront 프로젝트 및 Adobe 클라우드 스토리지 프로젝트용으로 풀링됩니다. 라이센스 사용자당 60GB입니다. 하드 캡은 없습니다. | 시스템 관리자는 설정의 고객 정보 페이지에서 저장소 사용량을 볼 수 있습니다. |
| [연간 비디오 리뷰 상한](#annual-video-review-cap) | 유료 Workfront 사용자 라이선스의 10%에서 비디오 증명 요청에 대한 조직 수준의 상한(표준 및 라이트). | 이 기간이 만료되면 다음 연간 기간까지 새로운 비디오 리뷰를 제공하지 않습니다. 80% 및 100%의 인앱 알림. Frame.io Enterprise 고객에게는 적용되지 않습니다. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | 기존 증명 기반 Fusion 시나리오는 Adobe 클라우드 스토리지 프로젝트에 대해 자동으로 작동하지 않습니다. | 레거시 프로젝트에 범위가 지정된 시나리오가 계속 작동합니다. 영향을 받는 각 시나리오는 편집, 다시 빌드 또는 사용 중지의 세 가지 경로 중 하나를 가져옵니다. 새로운 커넥터는 2026년 3분기로 예상됩니다. |

### 새 문서 영역

새 문서 영역은 Adobe 클라우드 스토리지용으로 설계된 통합 문서 환경입니다. 탐색을 단순화하고 검토 및 승인 활동을 통합하며 Frame.io 뷰어의 진입점입니다.

글로벌 문서 영역은 새 경험의 일부가 아닙니다. Adobe 클라우드 스토리지 프로젝트에서는 프로그램, 포트폴리오, 프로젝트, 작업 또는 문제의 문서에 액세스합니다.

자세한 내용은 [문서 영역](/help/quicksilver/documents/managing-documents/documents-area.md)을 참조하세요.

### 문서 권한

문서 권한은 Adobe 클라우드 스토리지 프로젝트에서 기본적으로 다릅니다.

* 개별 문서에 대한 권한을 공유하거나 설정할 수 없습니다. 대신 문서가 포함된 시스템 생성 문서 폴더에 권한이 적용됩니다.
* 시스템 생성 문서 폴더는 상위 프로젝트, 작업 또는 문제에서 권한을 상속합니다.
* 하위 폴더는 상위 시스템에서 생성한 문서 폴더에서 권한을 상속합니다.
* 하위 작업은 상위 작업에서 권한을 상속하지 않습니다. 시스템에서 생성한 문서 폴더에 액세스하려면 하위 작업에 직접 추가해야 합니다.


문서 권한이 작동하는 방식에 대한 자세한 내용은 [Adobe 클라우드 저장소 모델에 대한 개체 권한 및 액세스 수준 개요](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)를 참조하십시오.


### 개체 권한 매핑

권한은 Workfront에서 설정되고 Frame.io를 통해 한 방향으로 흐릅니다. Frame.io에서 Adobe 클라우드 스토리지 프로젝트에 사용자를 초대하거나 Frame.io에서 사용자 권한을 수정할 수 없습니다.

>[!TIP]
>
>프로젝트 코디네이터에게 Frame.io 액세스가 Workfront 권한의 다운스트림 반영임을 교육합니다. 관련자가 Adobe 클라우드 스토리지 프로젝트에 대한 검토에 액세스할 수 없다고 보고하면 수정 사항은 Frame.io가 아닌 Workfront에 있습니다.

다음 표에서는 Workfront 개체 권한을 Frame.io 권한에 매핑합니다.

| Workfront 권한 | Frame.io 권한 |
|---|---|
| 관리 | 편집 및 공유 |
| 참여 | 편집 및 공유 |
| 보기 | 주석만 |

Manage와 Contribute는 모두 Frame.io의 **Edit &amp; Share**&#x200B;에 매핑됩니다. Adobe 클라우드 스토리지 프로젝트에 대한 공유 패턴을 검토할 때 기여자가 외부 공유를 포함하여 관리자와 동일한 검토 측 기능을 갖도록 하는 것이 귀사의 거버넌스 모델에 적합한지 여부를 고려하십시오.

자세한 내용은 [Adobe 클라우드 저장소 모델에 대한 개체 권한 및 액세스 수준 개요](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio)를 참조하십시오.


### 검토 및 승인 뷰어

Adobe 클라우드 스토리지 개체에서 Frame.io 뷰어는 Workfront Proof 대신 검토 및 승인 화면입니다. Frame.io 뷰어는 검토 또는 승인에 할당된 외부 사용자를 포함하여 추가 비용 없이 모든 Workfront 사용자에 대해 포함됩니다.

Frame.io 뷰어는 다음을 제공합니다.

* 원, 화살표, 사각형과 같은 표준 모양과 자유 형식 드로잉을 포함한 마크업 및 주석 도구
* 비디오 검토를 위해 프레임 수준의 정확한 정밀도로 타임스탬프가 지정된 주석
* 버전 기록 및 버전 비교
* 이동 중 검토 및 승인을 위한 모바일 액세스
* ProRes, H.265, DNxHD와 같은 전문 비디오 형식에 대한 기본 재생과 함께 모든 일반 비디오, 이미지, 오디오, PDF, Microsoft Office 유형을 포함한 40개 이상의 파일 형식 지원 및 최대 500GB의 파일 지원


### 객체 이름 지정 규칙

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


### 객체 이동성

저장 모델과 같은 간에 Workfront 개체를 이동, 복사 및 변환할 수 있습니다. 예를 들어 작업을 한 Adobe 클라우드 스토리지 프로젝트에서 다른 Adobe 클라우드 스토리지 프로젝트로 이동할 수 있습니다. Adobe 클라우드 스토리지 프로젝트의 작업 또는 문제를 이전 프로젝트로 이동하거나 복사할 수 없으며 그 반대의 경우도 마찬가지입니다.

현재 Adobe 클라우드 스토리지 프로젝트를 생성하거나 이전 포트폴리오 또는 프로그램으로 이동하면 포트폴리오 또는 프로그램이 자동으로 Adobe 클라우드 스토리지 개체로 변환됩니다. 향후 릴리스를 통해 시스템 관리자는 어떤 객체가 자동으로 변환되는지 보다 세밀하게 제어할 수 있습니다.

### Adobe 클라우드 스토리지 개체에서 사용할 수 없는 기능

다음 기능은 Adobe 클라우드 스토리지 개체의 일부가 아닙니다.

* Workfront Proof
* Workfront 문서 뷰어
* 즐겨 찾는 문서
* 요청 문서

레거시 프로젝트는 위에 나열된 Workfront Proof 및 레거시 문서 기능에 대한 액세스 권한을 유지합니다. Workfront Proof은 향후 새로운 투자를 받지 않으며 향후 릴리스에서 중단될 예정입니다.

### 저장소 할당량

스토리지는 기존 Workfront 개체 및 Adobe 클라우드 스토리지 개체에 대해 풀링됩니다. 각 라이센스 사용자는 60GB의 스토리지를 받습니다. 스토리지 사용량에 대한 하드 캡은 없지만 할당량의 75%, 90%, 100%에 도달하면 Workfront 관리자가 이메일 알림을 받습니다.

시스템 관리자는 **설정** > **시스템** > **고객 정보**(으)로 이동하여 현재 저장소 사용량 및 할당량을 볼 수 있습니다.

자세한 내용은 [문서 저장소 제한 확인](/help/quicksilver/documents/managing-documents/check-document-storage.md)을 참조하세요.


### 연간 비디오 리뷰 상한

조직의 총 유료 Workfront 사용자 라이선스(표준 및 라이트)의 10%로 설정된 비디오 증명 요청에 대한 연간 상한이 있습니다. 이 상한은 조직 수준에서 적용됩니다.

* Workfront 관리자는 사용량이 상한의 80% 및 100%에 도달하면 인앱 알림을 받습니다.
* 상한에 도달하면 다음 연간 기간까지 새 비디오 검토 요청을 만들 수 없습니다.
* 이 제한은 Frame.io Enterprise 고객에게는 적용되지 않습니다. 조직에서 대량의 비디오 콘텐츠를 정기적으로 검토하는 경우 Adobe 계정 담당자에게 문의하여 Frame.io Enterprise 라이선싱에 대해 알아보십시오.

자세한 내용은 [통합 검토 및 승인 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)에서 에셋 및 비디오 검토 및 승인 FAQ를 참조하십시오.

### Adobe 클라우드 스토리지 프로젝트의 Workfront Fusion

레거시 증명을 기반으로 구축된 기존 Workfront Fusion 시나리오는 Adobe 클라우드 스토리지 프로젝트에 대해 자동으로 작동하지 않습니다. 증명별 모듈, 웹후크 및 API 엔드포인트는 경우에 따라 직접적인 등가물을 가지며 다른 경우에는 상당한 변경을 가집니다. 레거시 프로젝트에 범위가 지정된 시나리오는 오늘날과 같이 계속 작동합니다.

통합 검토 및 승인을 위한 기본 지원이 포함된 Fusion 커넥터는 2026년 3분기에 사용할 수 있습니다.

일반적인 시나리오 유형에 미치는 영향 및 각 시나리오를 해당 기능을 기반으로 편집, 다시 빌드 또는 사용 중지로 분류하는 방법에 대한 자세한 내용은 [통합 검토 및 승인을 위해 Workfront Fusion 시나리오 업데이트](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)를 참조하십시오.


## Adobe 클라우드 스토리지 롤아웃 방법 선택

Adobe 클라우드 스토리지가 사용자에게 표시되는 방식을 결정합니다. 두 가지 구성이 있으며, 둘 중 하나는 전체 조직 또는 특정 Workfront 그룹에 적용할 수 있습니다.

단계별 지침은 [조직에 Adobe 클라우드 저장소 사용](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)을 참조하십시오.

* **Adobe 클라우드 저장소만**: 새 프로젝트는 기본적으로 Adobe 클라우드 저장소를 사용합니다. 사용자가 레거시 프로젝트를 만들 수 없습니다.
* **Adobe 클라우드 저장소 및 레거시 Workfront 저장소**: 사용자가 프로젝트를 만들 때 Adobe 클라우드 저장소(&quot;새 프로젝트&quot;로 표시)와 레거시 Workfront 저장소(&quot;레거시 저장소&quot;로 표시) 중에서 선택합니다.

  ![프로젝트 형식 선택](assets/choose-project-type.png)



>[!TIP]
>
>먼저 Adobe 클라우드 스토리지를 더 작은 팀 앞에 배치하려면 단일 Workfront 그룹에 구성 중 하나를 적용하십시오. 이렇게 하면 더 광범위하게 롤아웃하기 전에 타깃팅된 파일럿을 실행할 수 있습니다. 제어된 게재 간격에 대한 그룹 수준 롤아웃으로 시작한 다음 파일럿 그룹이 경험의 유효성을 검사하면 전체 조직으로 확장하는 것이 좋습니다.

기존 객체는 생성된 스토리지 모델을 유지합니다. 기본 저장소 기본 설정을 변경해도 기존 개체는 변경되지 않습니다.

## 롤아웃 계획

모든 Workfront 환경은 다릅니다. 사용자를 위해 Adobe 클라우드 스토리지를 활성화하기 전에 조직의 성공적인 롤아웃을 계획하는 데 약간의 시간을 투자하십시오. 아래의 제안은 체크리스트가 아니라, 자신의 플랜에 대한 시작점이다.

**1. 파일럿 그룹을 선택하십시오.** 그룹 범위 롤아웃을 사용하면 Adobe 클라우드 스토리지를 더 작은 팀 앞에 먼저 배치하고 피드백을 수집한 다음 더 넓은 롤아웃 전에 조정할 수 있습니다. 초기에 알고 싶은 문제를 표시할 수 있을 만큼 작업 패턴이 대표적인 그룹을 선택하십시오.

**2. 최종 사용자에게 변경 내용을 전달합니다.** 검토자, 승인자 및 프로젝트 소유자에게 표시되는 가장 큰 변경 사항은 Adobe 클라우드 스토리지 프로젝트에 대한 검토 및 승인을 지원하는 새 문서 영역 및 Frame.io 뷰어입니다. 사용자가 첫 번째 Adobe 클라우드 스토리지 프로젝트를 접했을 때 예상되는 결과를 알 수 있도록 이러한 사항을 도입하는 방법을 계획합니다. [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) 문서는 최종 사용자 대면 자료에 유용한 시작점입니다.

**3. Workfront Fusion 커넥터 가용성에 대해 계획합니다.** 통합 검토 및 승인을 위한 기본 지원이 포함된 Fusion 커넥터는 2026년 3분기에 사용할 수 있습니다. 기존 증명 기반 Fusion 시나리오는 레거시 프로젝트에서 계속 작동합니다. 이러한 시나리오에 의존하는 팀을 Adobe 클라우드 스토리지 파일럿으로 가져오기 전에 새 커넥터를 기다리거나 현재 API에 대해 다시 빌드하거나 이러한 시나리오를 기본 통합 검토 및 승인 기능으로 대체할지 여부를 결정하십시오.

일반적인 시나리오 유형에 미치는 영향 및 각 시나리오를 해당 기능을 기반으로 편집, 다시 빌드 또는 사용 중지로 분류하는 방법에 대한 자세한 내용은 [통합 검토 및 승인을 위해 Workfront Fusion 시나리오 업데이트](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)를 참조하십시오.


## 관련 문서

* [Adobe 클라우드 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [조직에 Adobe 클라우드 스토리지 활성화](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [통합 검토 및 승인 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [문서 영역](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Adobe 클라우드 스토리지 모델에 대한 개체 권한 및 액세스 수준 개요](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)

