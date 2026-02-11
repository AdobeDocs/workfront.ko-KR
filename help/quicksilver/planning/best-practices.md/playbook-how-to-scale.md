---
title: '플레이북: 첫 번째 승리 후 관리되는 크기 조정'
description: 첫 번째 성공적인 구현 후 Adobe Workfront Planning을 롤아웃하는 방법에 대해 알아봅니다
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 54df36b3-01a3-4fd3-b2d3-64ffb2fe5918
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# 플레이북: 첫 번째 승리 후 관리되는 크기 조정

{{planning-important-intro}}

**버전**: 1.0

**컨텍스트**: &quot;첫 번째 사용 사례를 지정했으며 이제 모든 사용자가 참여하기를 원합니다.&quot;



## &#x200B;1. &quot;성공 트랩&quot;

때로는 WFP 채택의 가장 위험한 단계가 첫 번째 성공적인 사용 사례 또는 POC 직후 인 것처럼 느껴질 수 있습니다. 열의는 높지만, &quot;기술적 부채&quot;와 &quot;행정적 무질서한 팽배&quot;에 대한 두려움은 똑같이 두 가지 피해에 대한 반응을 이끌 수 있다:

1. **Over-Governance**: 새 팀이 스프레드시트로 되돌아갈 수 있도록 시스템을 단단히 잠그십시오.

2. **제로 거버넌스**: 모든 팀이 고유한 필드 및 레코드 형식을 만들 수 있도록 하여 레거시 환경에서 발견되는 분산된 메타데이터를 다시 만듭니다.



## &#x200B;2. 핵심 철학: &quot;조정 엔진&quot;으로서의 WFP

팀이 다른 것이 되지 않도록 하는 대신, WFP를 **이러한 차이점을 표시하여 조정할 수 있도록**&#x200B;한 위치로 지정합니다.



* **채택 속도 관리**: 기존 환경을 &quot;정리&quot;하기 전에 새 도구로 확장하는 것은 신중해야 합니다. **처음 작업을 간소화**&#x200B;하는 것은 매우 효율적인 토대를 제공하지만, 이를 통해 조정할 준비가 된 팀의 가치 실현 시간을 지연시킬 수 있습니다. 이 변경 사항을 진행할 수 있는 가장 효과적인 방법은 **가시성이 1단계**&#x200B;임을 인식하는 것입니다. PPT와 스프레드시트의 무분별한 확산에서 벗어나 전사적 차원의 공유 툴을 구축함으로써 장기적 목표를 달성할 수 있게 되었습니다.



  **권장 사항**: &quot;먼저 정리하기&quot; 권한 대신, 진행 중인 유지 관리에 더 적은 양의 리소스를 할당하고 긴급한 비즈니스 요구 사항을 해결하는 데 더 많은 양의 리소스를 할당하는 것이 좋습니다. 예를 들어, 분류법을 &quot;정리하는&quot; 데에만 1년을 보내는 것은 증분 가치를 거의 산출하지 않습니다. 그러나 **팀 간 가시성**(예: 통합 엔터프라이즈 달력 또는 통합 GTM 로드맵을 통해)을 제공하면 이해 당사자가 필요로 하는 혁신적인 가치를 제공하는 동시에 시간이 지남에 따라 환경을 관리하는 데 필요한 통합 데이터 구조를 제공할 수 있습니다.

* **현실 확인**: 독립 팀은 개별적으로 프로세스를 개발하며, 이 프로세스는 종종 개별적으로 배포된 스프레드시트에 숨겨져 있습니다. WFP로의 전환은 혼란을 야기시키지 않는다. 그것은 이미 존재하는 것에 빛을 비춘다. 이러한 프로세스를 공유 환경에서 볼 수 있도록 함으로써 이러한 프로세스를 최종적으로 해결하고 개선할 수 있는 한 곳에 배치할 수 있습니다.

* **진행 신호**: 팀이 자신의 필드를 요구할 때 &quot;무질서하게&quot; 이동하지 않습니다. **채택**&#x200B;입니다. 이는 그들이 WFP를 그들의 작업 공간으로 본다는 것을 의미한다.

* **부채 관리, 숨기지 않음**: 나중에 분산 분류법을 정리하는 데 필요한 노력에 대해 염려하는 것은 당연합니다. 그러나 엄격한 표준을 너무 일찍 강제하는 대신 각 팀은 프로세스(및 부채)가 숨겨져 있는 스프레드시트로 다시 돌아가게 됩니다. 팀이 현재 분류로 WFP에서 시작할 수 있도록 허용함으로써 해당 부채를 가시적이고 통제된 환경으로 전환하게 됩니다. 따라서 최종 조정은 하나의 압도적인 마이그레이션 프로젝트가 아닌 반복적인 작업이 됩니다.



## &#x200B;3. 도로의 차로 거버넌스 모델

&quot;글로벌 레인&quot;과 &quot;로컬 놀이터&quot;를 정의하여 채무 없이 규모 확장.



### A. 글로벌 레인

* **제어된 개체**: 모든 팀이 엔터프라이즈 보고에 사용해야 하는 개체(예: `Strategic Pillar`, `Region`, `Fiscal Quarter`).

* **관리자**: 중앙 COE/마케팅 운영 관리자

* **규칙**: 이러한 필드는 &quot;공유&quot;되며 필수입니다.



### B. 로컬 플레이그라운드(스포크)

* **실험 개체**: 팀의 전술적 요구 사항에 맞는 필드 또는 레코드 형식(예: 소셜 팀의 `Influencer Handle` 또는 웹 팀의 `URL Slug`).

* **관리자**: 팀장(간단한 지침 포함).

* **규칙**: 팀은 여기서 혁신할 수 있습니다. &quot;로컬&quot; 필드가 >3개 팀에서 채택되면 &quot;글로벌 레인으로 승격&quot;됩니다.



## &#x200B;4. 거버넌스의 역설: 팀 우선, 표준 준수

WFP 확장의 일반적인 문제는 먼저 **기업 거버넌스** 또는 **팀 운영 정렬**&#x200B;을 결정하는 것입니다.



이를 수행하는 가장 효과적인 방법은 엔터프라이즈 가치가 양방향 거리에 구축되어 있음을 인식하는 것입니다.

1. **팀에는 관련성이 필요합니다**: 엔터프라이즈는 해당 팀이 적극적으로 실행할 때만 가치를 실현합니다. 따라서 거버넌스는 알려진 운영 요구 사항을 지원하는 구조를 제공하여 팀을 **지원**&#x200B;해야 합니다.

2. **엔터프라이즈의 가시성이 필요합니다**: 데이터를 집계할 수 있을 만큼 깨끗할 때만 리더가 정보에 입각한 결정을 내릴 수 있습니다. 따라서 팀은 포트폴리오 가시성에 필요한 최소한의 실행 가능한 메타데이터를 제공하여 **엔터프라이즈를 지원**&#x200B;해야 합니다.



&quot;Managed Scaling&quot;의 목표는 이러한 두 가지 요구 사항의 교차를 찾는 것입니다. 이를 통해 가시성을 제공할 수 있을 만큼 표준화하되 팀 실행을 지연시킬 정도는 아닙니다.



### A. 우선 순위 조정: 데이터와 시각화

크기를 조정할 때 &quot;값&quot;의 정의가 성향 간에 다르다는 것을 인지합니다.

* **관리자/제품 소유자**: 값 **통합 분류 및 분류**. 이 솔루션의 목표는 장기적인 확장성을 지원하는 깔끔한 데이터 아키텍처입니다.

* **관련자/리더**: 값 **시각화 및 insight**(예: 전역 일정 또는 Portfolio 타임라인). 그들의 목표는 데이터를 실행 가능하게 만드는 &quot;번개 순간&quot;입니다.



**전략**: 팀이 데이터 표준에 대한 관리자의 요구 사항을 준수하도록 *인센티브*(으)로 이해 당사자의 시각화 필요성을 사용합니다. 리더쉽이 요구하는 &quot;슈퍼 캘린더&quot;를 전달하여 통합 분류법을 얻을 수 있습니다.



### B. &quot;서비스 주도&quot; 관찰 단계

초기 규모 확장 시 관리자의 역할은 팀과 엔터프라이즈 간의 이러한 교환을 용이하게 하는 것입니다.

* **표준화보다 작업 우선 순위 지정**: 팀들이 전역 정의가 없어 중단되는 것보다 개별적으로 배치된 작업 영역에서 적극적으로 계획을 수립하도록 하는 것이 좋습니다. 이 활동은 건강한 실제 표준을 구축하는 데 필요한 &quot;원시 데이터&quot;입니다.

* **&quot;가시성 최소화&quot; 확인**: 리더십을 사용하여 *엔터프라이즈 보고에 대해*&#x200B;이(가) 깔끔해야하는 3~5개 필드(예: `Strategic Alignment`, `Start Date`, `Budget`)를 확인합니다. 여기에만 집행 에너지를 집중하세요.



### B. 소급 조화(Governance as a Service)

팀 간에 &quot;알려진 요구 사항&quot; 패턴이 나타나면 엔터프라이즈는 이러한 패턴을 글로벌 서비스로 통합하기 위해 이동할 수 있습니다.

1. **성공적인 패턴 관찰**: 팀에서 이미 구축하여 채택한 &quot;가장 성과가 좋은&quot; 분류법을 식별합니다.

2. **공동 핸드셰이크**: 팀 챔피언을 모아 로컬 성공을 공유 엔터프라이즈 표준으로 구체화합니다.

3. **서비스로 배포**: &quot;제한&quot;이 아닌 작업을 수행하는 사람들에 대한 보고 및 팀 간 정렬을 간소화하는 방법으로 새 전역 레인을 롤아웃합니다.



**주요 개선 사항**: 거버넌스는 운영 성공에 대한 응답이어야 하며 필수 요구 사항이 아니어야 합니다.



## &#x200B;5. 스케일링 역학: 패턴 기반 성장 모델

이러한 철학을 적용하려면 데이터 구조에 대한 사려깊은 접근이 필요하다. 무질서한 &quot;거버넌스 확산&quot;을 방지하려면 모든 개별 요청에 대해 글로벌 필드를 구축해야 한다는 강박에 저항하십시오. 대신 **필드 성숙도 경로**&#x200B;를 사용하여 실제 사용 시 엔터프라이즈 표준을 안내하도록 하십시오.



1. **수준 1: 로컬 실험**: 팀 A가 작업 영역에 사용자 지정 필드를 만듭니다.

2. **수준 2: 패턴 인식**: 관리자가 B팀과 C팀에서 유사한 필드를 사용하거나 요청하고 있습니다.

3. **수준 3: 엔터프라이즈 표준화**: 관리자가 해당 필드의 표준화된 단일 버전을 **전역 분류법 Workspace**&#x200B;에서 레코드 형식으로 만들어 팀에 배포합니다.



### &quot;부드러운 은퇴&quot;의 역학

WFP에는 현재 필드에 대한 기본 &quot;아카이브&quot; 기능이 없으므로 로컬 필드를 중단하려면 UI를 복잡하게 하지 않고 내역 데이터를 보존하기 위해 의도적인 &quot;소프트 중단&quot; 프로세스가 필요합니다.



1. **데이터 마이그레이션**: 테이블 보기(또는 Fusion)를 사용하여 로컬 &quot;섀도&quot; 필드의 값을 새 전역 레인 필드로 대량 복사합니다. 이 이동 중에 데이터의 유효성을 검사하고 정리해야 합니다.

2. **사용 중지를 위한 이름 바꾸기**: `[DEPRECATED]` 또는 `z_`(예: `z_Language (Old)`)과 같은 접두사를 사용하여 로컬 필드의 이름을 바꿉니다. 이는 필드를 필드 선택기의 맨 아래로 밀고 사용자에게 더 이상 &quot;진실의 Source&quot;가 아니라는 신호를 보냅니다.

3. **양식 제거**: **가장 중요한 단계입니다.** 모든 **레코드 Forms**&#x200B;에서 사용되지 않는 필드를 제거합니다. 이렇게 하면 필요한 경우 기존 테이블 보기 또는 보고서에 이전 데이터가 계속 표시되도록 하면서 새 데이터를 입력할 수 없습니다.

4. **일몰 기간**: 마이그레이션하는 동안 데이터가 누락되지 않도록 사용되지 않는 필드(접두사가 있고 형식이 잘못된 필드)를 30~60일 동안 유지합니다. 이 기간이 지난 후 데이터가 전역 레인에 완전히 조정된 경우 작업 영역에서 로컬 필드를 삭제할 수 있습니다.



## &#x200B;6. &quot;핵심 드리프트&quot;(추상화 규칙) 피하기

Planning이 Core만큼 복잡해지지 않도록 하려면 다음을 수행합니다.

* **추상화 계층**: WFP의 모든 필드는 **전략 질문**&#x200B;에 응답해야 합니다. 필드가 전술적 추적에만 사용되는 경우(예: &quot;이 증명이 승인되었습니까?&quot;) 코어에서 유지합니다.

* **통합 우선**: 팀이 새 메타데이터 필드를 원하는 경우 먼저 전역 분류법을 확인하도록 초대합니다. 이를 위해서는 팀에게 글로벌 분류 작업 영역에 대한 **읽기 전용 액세스 권한**&#x200B;을 부여해야 합니다(섹션 7 참조). 전술적 요구 사항을 기존 전략 필드에 매핑하면 불필요한 중복을 방지하고 보고 무결성을 유지할 수 있습니다.



## &#x200B;7. &quot;읽기 전용 액세스&quot; 가시성 모델

&quot;사일로드&quot; 작품의 소음 없이 &quot;사일로드&quot; 느낌을 해결한다.

* **문제**: 스포크에 있는 팀은 자신의 레코드만 볼 수 있으므로 격리된 느낌이 듭니다.

* **수정 사항**: 공유 레코드 형식에 대해 &#39;기본&#39;으로 지정된 작업 영역에 대한 읽기 전용 액세스 권한을 팀 **부여합니다**.

* **결과**: 사용자는 영감과 맞춤화에 대한 광범위한 엔터프라이즈 컨텍스트를 볼 수 있지만 로컬 작업 영역은 깔끔하고 특정 작업에 집중되어 있습니다.



## &#x200B;8. 워크숍을 통한 성장 관리

WFP를 조정하는 것은 기술적인 문제만큼이나 문화적인 과제입니다. 타깃팅된 워크샵을 사용하여 &quot;거버넌스 격차&quot;를 해소하십시오.



### A. &quot;Necessary Mess&quot; Discovery 워크숍

* **대상**: 지역 마케팅 리드 및 운영 챔피언.

* **목표**: 현재 &quot;고립된 현실&quot;(단편화된 운영 데이터)을 문서화합니다.

* **메시지**: &quot;필드를 삭제하려고 온 것이 아닙니다. 우리는 그들이 어떻게 글로벌 전략과 연계되는지 이해하기 위해 이 자리에 모였습니다.&quot;

* **결과**: 로컬 전술 필드를 전역 전략 차선에 매핑하는 초안



### B. &quot;전략적 가시성&quot; 조정 세션

* **대상**: 높은 수준의 마케팅 이해 당사자(리더십).

* **목표**: &quot;처음 단순화&quot; 불안을 수정했습니다.

* **메시지**: &quot;시작하려면 완벽한 분류법이 필요하지 않습니다. 완벽한 분류법을 *빌드*&#x200B;하기 위한 환경으로 WFP를 사용하고 있습니다.&quot;

* **결과**: Core가 현재 상태에 있는 동안 조정 엔진으로 WFP를 진행할 수 있도록 승인합니다.



### C. &quot;Spoke-to-Global&quot; 쇼케이스

* **대상**: WFP를 탐색하는 새 팀입니다.

* **목표**: &quot;고립된&quot; 느낌을 줄이십시오.

* **메시지**: &quot;팀 A의 로컬 작업이 지정된 기본 Workspace을 자동으로 피드하는 방법을 확인하십시오. 또한 작업에 대해 동일한 가시성을 가질 수 있습니다.&quot;

* **결과**: 로컬 독립성을 잃지 않고 &quot;연결&quot;되는 이점을 얻는 새 부서의 옵트인.



### D. &quot;지속적인 지원&quot; 운영 시간

* **대상**: 모든 WFP 사용자(현재 및 예상 사용자)입니다.

* **목표**: 문제 해결 및 전술적 지침을 위한 낮은 이해도가 반복되는 환경을 제공합니다.

* **메시지**: &quot;잘못된 질문이 없습니다. Dell은 고객의 구체적인 계획 과제를 실시간으로 해결할 수 있도록 도와 드립니다.&quot;

* **결과**: 사용자 신뢰도 향상, 기술 마찰 해결 속도 향상, 글로벌 표준화를 보장할 수 있는 새로운 패턴 식별.



## &#x200B;9. 규모별 인력 배치: 역할 및 책임

관리형 크기 조절 모델은 단순한 도구 구성 이상의 기능을 필요로 합니다. 글로벌 및 Spoke 팀 전체에 명확한 역할 분배가 필요합니다.



### A. 엔터프라이즈 설계자(중앙 COE/마케팅 운영)

* **포커스**: 엔터프라이즈 무결성, 시스템 성능 및 **통합 데이터 분류**.

* **책임**:

   * **전역 분류법 Workspace**&#x200B;을 관리합니다.

   * **필드 완성도 경로**&#x200B;을(를) 용이하게 합니다(전역 표준에 대한 로컬 성공을 촉진함).

   * 경영진 보고를 위해 **기본 Workspace** 보기를 유지 관리합니다.

   * 작업 영역에서 월별 **의미 체계 감사**&#x200B;를 진행합니다.



### B. Spoke 챔피언(팀 프로세스 소유자)

* **포커스**: 팀 관련성 및 채택 속도.

* **책임**:

   * 기능 팀의 단일 연락 창구 역할을 합니다.

   * 로컬 작업 공간 구조 및 사용자 지정 필드 실험을 소유합니다.

   * 팀이 데이터 입력을 위해 **관리되는 게이트웨이**(Forms)를 사용하도록 합니다.

   * 조화 중에 **공동 핸드셰이크**&#x200B;에 참가합니다.



### C. 경영 스폰서(마케팅 리더십)

* **포커스**: 전략적 정렬, OKR 가시성 및 **포트폴리오 시각화(예: 전역 일정)**.

* **책임**:

   * 전역 분류 작업 영역에서 엔터프라이즈 **마케팅 OKR**&#x200B;을(를) 정의합니다.

   * 다른 리더들에게 &quot;Visibility Step 1&quot;의 가치를 부여합니다.

   * 80/20 리소스 할당을 강화합니다(정리 작업 이상의 값).



### D. 지원 리드(변경 관리)

* **포커스**: 문화 이동과 기술 개발.

* **책임**:

   * **근무 시간** 및 **검색 워크숍**&#x200B;을(를) 호스팅합니다.

   * 내부 &quot;Success Story&quot; 쇼케이스를 유지 관리합니다.

   * Enterprise Architect가 해결할 기술 마찰 지점을 식별합니다.



## &#x200B;10. 다음 팀의 확장을 위한 체크리스트

* [ ] **챔피언 식별**: 이 새 팀의 &quot;프로세스 소유자&quot; 또는 &quot;챔피언&quot;은 누구입니까?

* [ ] **로컬 델타 정의**: Global Standard에서 현재 제공하지 않는 2-3 필드는 어떤 것이 필요합니까?

* [ ] **전역 레인에 매핑**: 요구 사항의 80%를 충족할 수 있는 기존 전역 필드는 무엇입니까?

* [ ] **전역 가시성 부여**: 1일에 관련 기본 작업 영역 및 전역 분류 작업 영역에 대한 읽기 전용 액세스 권한을 부여합니다.

* [ ] **전달 설정**: 관련 기본 작업 영역에서 어떻게 &quot;전달&quot;합니까? (예: 글로벌 레코드 유형 또는 특정 조회를 통해).

<!--original content: 

**Version**: 1.0 

**Context**: "We've landed our first use case, and now everyone wants in." 

 

## 1. The "Success Trap" 

Sometimes it can feel like the most dangerous phase of WFP adoption is immediately after the first successful use case or POC. Enthusiasm is high, but the fear of "technical debt" and "administrative sprawl" can lead to two equally damaging responses: 

1.  **Over-Governance**: Locking down the system so tightly that new teams revert to spreadsheets. 

2.  **Zero-Governance**: Letting every team create their own fields and record types, recreating the fragmented metadata sprawl found in legacy environments. 

 

## 2. The Core Philosophy: WFP as the "Reconciliation Engine" 

Instead of trying to stop teams from being different, we position WFP as the place where those differences are **made visible so they can be reconciled**. 

 

*   **Managing Adoption Velocity**: It is natural to feel cautious about expanding into a new tool before "cleaning up" existing environments. While choosing to **Simplify First** provides a highly governed foundation, it can delay time-to-value for teams ready to align. We believe the most effective way to lead through this change is to recognize that **visibility is Step 1**. Momentum toward a shared, enterprise-ready tool (moving away from the sprawl of PPTs and spreadsheets) is what ultimately unblocks long-term goals.  

 

    **Recommendation**: Instead of a "Clean Up First" mandate, we recommend allocating a smaller portion of resources to ongoing maintenance and a significantly larger portion to solving pressing business needs. For example, spending a year solely on "cleaning up" taxonomies yields little incremental value. However, delivering **cross-team visibility** (e.g., through a Unified Enterprise Calendar or a consolidated GTM roadmap) provides the transformative value your stakeholders need, while providing the unified data structure you need to govern the environment over time. 

*   **Acknowledge the Reality**: Independent teams naturally develop their own processes, which often stay hidden in siloed spreadsheets. Transitioning to WFP doesn't create a mess; it shines a light on the one that already exists. By making these processes visible in a shared environment, you put them in the one place where they can finally be addressed and improved. 

*   **The Progress Signal**: When a team asks for their own fields, it's not "sprawl"—it's **Adoption**. It means they see WFP as their workspace. 

*   **Manage Debt, Don't Hide It**: It is natural to be concerned about the effort required to clean up divergent taxonomies later. However, the alternative—forcing strict standards too early—often drives teams back to spreadsheets where their processes (and their debt) remain hidden. By allowing teams to begin in WFP with their current classifications, you are moving that debt into a visible, governed environment. This makes the eventual reconciliation an iterative task rather than a single, overwhelming migration project. 

 

## 3. The "Lanes on a Road" Governance Model 

Scale without debt by defining "Global Lanes" and "Local Playgrounds." 

 

### A. The Global Lanes 

*   **Controlled Objects**: Objects that every team must use for enterprise reporting (e.g., `Strategic Pillar`, `Region`, `Fiscal Quarter`). 

*   **Managed By**: The Central COE/Marketing Ops Admin. 

*   **Rule**: These fields are "Shared" and mandatory. 

 

### B. The Local Playgrounds (Spokes) 

*   **Experimental Objects**: Fields or record types specific to a team's tactical needs (e.g., a Social team's `Influencer Handle` or a Web team's `URL Slug`). 

*   **Managed By**: The Team Lead (with light guidance). 

*   **Rule**: Teams can innovate here. If a "Local" field is adopted by >3 teams, it is "Promoted" to a Global Lane. 

 

## 4. The Governance Paradox: Teams First, Standards Follow 

A common challenge in scaling WFP is deciding which comes first: **Enterprise Governance** or **Team Operational Alignment**.  

 

We believe the most effective way to navigate this is to recognize that enterprise value is built on a two-way street: 

1.  **Teams need relevance**: The enterprise only realizes value when its teams are actively executing. Therefore, governance must **serve the teams** by providing structure that supports their known operational needs. 

2.  **The Enterprise needs visibility**: Leadership can only make informed decisions when data is clean enough to aggregate. Therefore, the teams must **serve the enterprise** by providing the minimum viable metadata required for portfolio visibility. 

 

The goal of "Managed Scaling" is to find the intersection of these two needs—standardizing enough to provide visibility, but not so much that you stall team execution. 

 

### A. Aligning Priorities: Data vs. Visualization 

When scaling, recognize that the definition of "Value" differs between personas: 

*   **The Admin/Product Owner**: Values **unified taxonomies and classifications**. Their goal is a clean data architecture that supports long-term scalability. 

*   **The Stakeholder/Leader**: Values **visualization and insight** (e.g., a Global Calendar or a Portfolio Timeline). Their goal is the "Lightning Moment" that makes the data actionable. 

 

**The Strategy**: Use the stakeholder's need for visualization as the *incentive* for the team's compliance with the admin's need for data standards. You get the unified taxonomy by delivering the "Super Calendar" that leadership demands. 

 

### B. The "Service-Led" Observation Phase 

During early scale-up, the Admin's role is to facilitate this exchange between teams and the enterprise. 

*   **Prioritize Operation over Standardization**: It is better to have teams actively planning in siloed workspaces than to have them stalled by a lack of global definitions. This activity is the "raw data" required to build healthy, real-world standards. 

*   **Identify the "Visibility Minimums"**: Work with leadership to identify the 3-5 fields that *must* be clean for enterprise reporting (e.g., `Strategic Alignment`, `Start Date`, `Budget`). Focus your enforcement energy ONLY here. 

 

### B. Retroactive Harmonization (Governance as a Service) 

Once a pattern of "known needs" emerges across teams, the enterprise can move to consolidate those patterns into a global service. 

1.  **Observe Successful Patterns**: Identify the "winning" taxonomies that teams have already built and adopted. 

2.  **The Collaborative Handshake**: Bring team champions together to refine their local successes into a shared enterprise standard. 

3.  **Deploy as a Service**: Roll out the new global lanes not as a "restriction," but as a way to simplify reporting and cross-team alignment for the people doing the work. 

 

**Key Takeaway**: Governance should be a response to operational success, not a prerequisite for it.  

 

## 5. Scaling Mechanics: The Pattern-Based Growth Model 

Applying this philosophy requires a thoughtful approach to data structure. To avoid "Governance Sprawl," resist the urge to build global fields for every individual request. Instead, use the **Field Maturity Path** to let real-world usage guide your enterprise standards: 

 

1.  **Level 1: Local Experiment**: Team A creates a custom field in their workspace. 

2.  **Level 2: Pattern Recognition**: The Admin notices Teams B and C are using or asking for a similar field. 

3.  **Level 3: Enterprise Standardization**: The Admin creates a single, standardized version of that field as a record type in the **Global Taxonomy Workspace** and syndicates it to teams. 

 

### The Mechanics of "Soft Retirement" 

Because WFP does not currently have a native "Archive" feature for fields, retiring a local field requires a deliberate "Soft Retirement" process to preserve historical data without cluttering the UI: 

 

1.  **Data Migration**: Use a table view (or Fusion) to bulk-copy values from the local "Shadow" field into the new Global Lane field. Ensure the data is validated and cleaned during this move. 

2.  **Rename for Deprecation**: Rename the local field with a prefix like `[DEPRECATED]` or `z_` (e.g., `z_Language (Old)`). This pushes the field to the bottom of field pickers and signals to users that it is no longer the "Source of Truth." 

3.  **Form Removal**: **This is the most critical step.** Remove the deprecated field from all **Record Forms**. This prevents new data from being entered while keeping the old data visible in existing table views or reports if needed. 

4.  **The "Sunset" Period**: Keep the deprecated field (prefixed and off-form) for 30-60 days to ensure no data was missed during migration. After this period, if the data is fully reconciled in the Global Lane, the local field can be deleted from the workspace. 

 

## 6. Avoiding the "Core Drift" (The Abstraction Rule) 

To prevent Planning from becoming as cluttered as Core: 

*   **The Abstraction Layer**: Every field in WFP should answer a **Strategic Question**. If a field is only used for tactical tracking (e.g., "Was this proof approved?"), keep it in Core. 

*   **Consolidation First**: If a team wants a new metadata field, invite them to check the Global Taxonomy first. This requires granting team leads **Read-Only access** to the Global Taxonomy workspace (see Section 7). By mapping their tactical needs to an existing strategic field, you prevent unnecessary duplication and maintain reporting integrity. 

 

## 7. The "Read-Only Access" Visibility Model 

Solve the "Siloed" feeling without the noise of "Siloed" work. 

*   **The Problem**: Teams in spokes feel isolated because they only see their own records. 

*   **The Fix**: Grant teams **Read-Only access to the workspaces designated as 'Primary' for those shared record types**.  

*   **The Result**: They can see the broader enterprise context for inspiration and alignment, but their local workspace remains clean and focused on their specific tasks. 

 

## 8. Managing Growth through Workshops 

Scaling WFP is as much a cultural challenge as a technical one. Use targeted workshops to bridge the "Governance Gap." 

 

### A. The "Necessary Mess" Discovery Workshop 

*   **Audience**: Regional Marketing Leads and Ops Champions. 

*   **Goal**: Document the current "Siloed Reality" (the fragmented operational data). 

*   **The Message**: "We aren't here to delete your fields. We're here to understand how they link to the global strategy." 

*   **Outcome**: A draft mapping of local tactical fields to global strategic lanes. 

 

### B. The "Strategic Visibility" Alignment Session 

*   **Audience**: High-level Marketing Stakeholders (leadership). 

*   **Goal**: Reframe the "Simplify First" anxiety. 

*   **The Message**: "We don't need a perfect taxonomy to start. We are using WFP as the environment to *build* the perfect taxonomy." 

*   **Outcome**: Approval to move forward with WFP as the reconciliation engine while Core remains in its current state. 

 

### C. The "Spoke-to-Global" Showcase 

*   **Audience**: New teams exploring WFP. 

*   **Goal**: Reduce the "siloed" feeling. 

*   **The Message**: "See how Team A's local work automatically feeds the designated Primary Workspace? You can have that same visibility for your work too." 

*   **Outcome**: Opt-in from new departments who see the benefit of being "connected" without losing their local independence. 

 

### D. The "Ongoing Support" Office Hours 

*   **Audience**: All WFP users (current and prospective). 

*   **Goal**: Provide a recurring, low-stakes environment for troubleshooting and tactical guidance. 

*   **The Message**: "There are no wrong questions. We are here to help you solve your specific planning challenges in real-time." 

*   **Outcome**: Increased user confidence, faster resolution of technical friction, and the identification of new patterns that might warrant global standardization. 

 

## 9. Staffing for Scale: Roles and Responsibilities 

Success in a managed scaling model requires more than just tool configuration; it requires a clear distribution of roles across the Global and Spoke teams. 

 

### A. The Enterprise Architect (Central COE/Marketing Ops) 

*   **Focus**: Enterprise integrity, system performance, and **unified data taxonomy**. 

*   **Responsibilities**: 

    *   Manages the **Global Taxonomy Workspace**. 

    *   Facilitates the **Field Maturity Path** (promoting local successes to global standards). 

    *   Maintains the **Primary Workspace** views for executive reporting. 

    *   Leads the monthly **Semantic Audit** across workspaces. 

 

### B. The Spoke Champion (Team Process Owner) 

*   **Focus**: Team relevance and adoption velocity. 

*   **Responsibilities**: 

    *   Acts as the single point of contact for the functional team. 

    *   Owns the local workspace structure and custom field experiments. 

    *   Ensures the team uses the **Governed Gateway** (Forms) for data entry. 

    *   Participates in the **Collaborative Handshake** during harmonization. 

 

### C. The Executive Sponsor (Marketing Leadership) 

*   **Focus**: Strategic alignment, OKR visibility, and **portfolio visualization (e.g., Global Calendaring)**. 

*   **Responsibilities**: 

    *   Defines the enterprise **Marketing OKRs** in the Global Taxonomy workspace. 

    *   Champions the value of "Visibility Step 1" to other leaders. 

    *   Reinforces the 80/20 resource allocation (Value over Cleanup). 

 

### D. The Enablement Lead (Change Management) 

*   **Focus**: Cultural shift and skill development. 

*   **Responsibilities**: 

    *   Hosts recurring **Office Hours** and **Discovery Workshops**. 

    *   Maintains the internal "Success Story" showcase. 

    *   Identifies technical friction points for the Enterprise Architect to resolve. 

 

## 10. Checklist for Scaling the Next Team 

* [ ] **Identify the Champion**: Who is the "Process Owner" or "Champion" of this new team? 

* [ ] **Define the "Local Delta"**: What 2-3 fields does this team need that the Global standard doesn't currently provide? 

* [ ] **Map to Global Lanes**: Which existing Global fields can satisfy 80% of their needs? 

* [ ] **Grant Global Visibility**: Give them Read-Only access to the relevant Primary Workspaces and the Global Taxonomy workspace on Day 1. 

* [ ] **Establish the Handoff**: How does their work "feed" the relevant Primary Workspaces? (e.g., via a Global Record Type or a specific lookup).

-->