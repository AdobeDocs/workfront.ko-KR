---
title: Adobe Workfront 계획 모범 사례
description: 마케팅 운영 리더로서 Adobe Workfront Planning을 사용하여 모든 팀의 마케팅 라이프사이클 전반에서 작업을 구성할 수 있습니다. 다음은 Workfront Planning을 시작할 때 권장하는 몇 가지 모범 사례입니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: 1926500c76e4f9cfdac829f8d9f0cdfa6231e31d
workflow-type: tm+mt
source-wordcount: '3304'
ht-degree: 0%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Adobe Workfront 계획 모범 사례

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

마케팅 운영 리더로서 Adobe Workfront Planning을 사용하여 모든 팀의 마케팅 라이프사이클 전반에서 작업을 구성할 수 있습니다.

이 문서에서는 Workfront Planning을 시작할 때 권장하는 몇 가지 FAQ 및 모범 사례를 문서화합니다.

## 구성 모범 사례

### 작업 영역

작업 공간은 팀이 작업을 계획하는 중앙 집중식 위치입니다. 작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다.

다음은 Workfront Planning 구성에 대한 몇 가지 FAQ입니다.

#### 어떻게 시작해야 합니까?

* ✅ Planning에 처음 로그인할 때 Planning의 가치를 명확하게 전달하고 제품을 효과적으로 탐색하고 활용하는 방법을 안내하는 인앱 온보딩 프로세스를 따르십시오. 이렇게 하면 기능의 정의와 작업을 쉽게 시작하는 방법을 이해할 수 있습니다.
* ✅ 먼저 기존의 유사한 사용 사례에 대한 아이디어를 미리 정의한 작업 영역 템플릿을 살펴봅니다. 템플릿에 있는 미리 정의된 레코드 종류 및 필드를 사용하거나 사용자 고유의 레코드 종류를 추가할 수 있습니다.
* ✅ Workfront Planning에서 해결할 주요 사용 사례를 식별합니다. 예를 들어 대부분의 조직은 전략 활동에 대한 가시성을 향상시키고자 하며, 여기에는 더 나은 &quot;캠페인 달력&quot; 구축이 포함될 수 있습니다. 따라서 이 사용 사례의 경우 몇 가지 질문에 답변하는 것으로 시작하고자 합니다.

   * 누가 그걸 요구합니까?
   * 달력에 넣고 싶은 것을 뭐라고 부릅니까?
캠페인? 전술이요? 이니셔티브? 활동? 이벤트?
   * 이 달력으로 어떤 종류의 질문에 답하고 싶습니까?
   * 동일한 대상에 대해 중복 캠페인이 있습니까?
   * 그 캠페인, 전술, 활동 또는 이벤트에 대한 우리의 예산은 무엇입니까?

  이러한 질문에 대한 답변은 Workfront Planning 내부에 빌드하는 데 필요한 사항을 지시합니다.

  또한 현재 Workfront 사용자가 아닌 다른 플래너가 있을 수 있습니다. 이러한 플래너는 Excel 스프레드시트, Word 문서, PowerPoint 등으로 작동할 수 있습니다. 방문자가 Workfront Planning에서 정보에 액세스하는 방법을 고려합니다.

* ✅ Workfront Planning을 최대한 활용하려면 Workfront Workflow의 포트폴리오 및 프로그램 사용을 Workfront Planning의 다른 상위 계층 구조로 바꾸는 것이 좋습니다.

  현재 Workfront 고객은 포트폴리오와 프로그램을 통해, 경우에 따라 다른 유형의 프로젝트로 자신의 전략 작업을 나타냅니다. Planning의 도입으로 이러한 모든 전략적 작업은 Workfront Planning에서 사용자 정의 레코드 유형을 통해 처리해야 하는 반면 Workfront은 프로젝트 및 작업으로 표현되는 작업 실행 단계를 중심으로 이루어집니다.


#### 기존 작업 영역을 수정하는 것과 비교하여 새 작업 영역을 언제 만들어야 합니까?

* ✅ 조직 수준 작업 영역의 가장 낮은 볼륨에 대한 디자인입니다. 각 장치의 고유한 작동 방식에 맞게 특정 운영 조직 단위에 대한 작업 공간을 만들 수 있습니다.

  단일 Workspace에 정보를 배치하여 모든 데이터 간의 관계를 쉽게 관리할 수 있습니다.

  예를 들어 모든 마케팅에 대해 단일 작업 영역을 생성해 보십시오.

  완전히 다른 운영 구조를 가진 팀을 위해 새 작업 영역을 생성해도 됩니다.

  예를 들어 **제품 개발** 작업 영역은 **마케팅** 작업 영역과 구별되어야 합니다.

* ⛔ 조직 내의 각 팀 또는 프로세스에 대해 고유한 작업 영역을 만들지 마십시오.

  마케팅 조직은 가시성을 유지하고 글로벌 계획 수준에서 데이터를 롤업할 수 있도록 한 개의 작업 영역만 유지 관리하도록 노력해야 합니다.

  유사한 프로세스를 따르는 팀(예: EMEA 마케팅 대 APAC 마케팅)에 대해 유사 또는 중복 작업 영역을 만들지 마십시오. 특히 이러한 팀이 공통 전략 캠페인에 맞춰 작업을 수행할 수 있는 경우에는 더욱 그렇습니다.

#### Workspace 섹션을 어떻게 사용해야 합니까?

* ✅ 사용자가 작업 주기를 구성하는 방법을 이해하는 데 도움이 되는 섹션을 만들고 레이블을 지정합니다.

  예를 들어, 캠페인, 전술 및 결과물을 작업 공간에 배치하는 **핵심 레코드**&#x200B;라는 섹션을 만들 수 있습니다.
* ✅ 그룹 &quot;좋아요&quot; 레코드 유형을 함께 묶습니다.

  예를들어 지역, 국가, 도시 등의 레코드 종류를 포함하는 **지역** 섹션을 만들 수 있습니다.

### 레코드 유형

레코드 유형은 Workfront Planning Workspace의 기본 구성단위입니다. 레코드 유형이 상호 연결되는 방법을 정의할 수 있습니다.


#### 작업 영역에서 레코드 유형을 정의하려면 어떻게 해야 합니까?

* ✅ 추적해야 하는 정보(필요한 레코드 종류)와 이 정보를 연결하는 방법을 확인하는 데 시간이 걸립니다. 작업 영역을 사용하여 모든 요구 사항을 고려할 이해 당사자와 대화합니다. 다양한 레코드 유형으로 사용자 정의 섹션을 만들어 정보를 매우 쉽게 사용할 수 있도록 제공할 수도 있습니다.


* ⛔ 다른 기간의 레코드 형식을 복제하지 마십시오(예: **Campaigns 2024** 및 **Campaigns 2025**&#x200B;에 대해 별도의 레코드 형식을 만들지 마십시오).

  다양한 레코드 유형을 만들면 여러 해에 걸친 데이터를 비교하려는 때마다 데이터 흐름이 끊어집니다. 오늘 보기는 레코드 유형별로 다르므로 연도가 종료되는 즉시 해당 레코드 유형의 보기에는 향후 항목이 더 이상 표시되지 않습니다. 가장 좋은 방법은 작업 유형에 대해 하나의 레코드 유형을 갖고 필요한 경우 필터를 사용하거나 보관을 사용하여 데이터를 세그먼트화하는 것입니다.

#### 단일 또는 다중 선택 필드와 연결된 레코드 유형은 언제 사용해야 합니까?

* ✅ 개체를 다른 여러 레코드 형식과 연결하여 사용할 경우 새 레코드 형식을 추가합니다.

  예를 들어, 캠페인은 여러 Target 대상에 연결되고, 전술은 단일 Target 대상에 연결될 수 있습니다. 따라서 캠페인, 전술 및 대상자는 다중 선택 필드가 아닌 레코드 유형이어야 합니다.

* ✅ 개체에서 조회에 유용할 수 있는 추가 메타데이터 값을 저장해야 하는 경우 새 레코드 형식을 추가합니다.

  예를 들어, **Email**&#x200B;과 같은 채널 레코드 유형에는 기본 메타데이터나 독립 실행형 **Deliverables** 레코드 유형에 대한 연결로서 지원 게재 항목 목록을 저장할 수 있습니다.
* ⛔ 저장하는 데이터가 단일 레코드 형식에 대해서만 적절한 경우 새 레코드 형식을 추가하지 마십시오.

  예를 들어 **Campaign** 레코드 유형에는 특정 캠페인과 직접 연결된 경우에만 관련이 있는 **캠페인 크기**&#x200B;라는 단일 선택 필드가 있을 수 있습니다.

#### 레코드 유형에 레이블을 지정하려면 어떻게 해야 합니까?

* ✅ **캠페인**&#x200B;과 같이 단일 구문 또는 명사를 나타내는 레코드 형식을 만들고 레이블을 지정합니다.
* ⛔ 보기로 더 잘 표현되는 레코드 형식을 만들지 않습니다.

  예를들어 **Calendar**&#x200B;은(는) 레코드 형식 자체가 아니라 레코드 보기이므로 레코드 형식에 적합하지 않은 선택입니다.

### 필드 관리

필드는 레코드 유형의 속성이며 테이블 보기에서 열로 표시됩니다. 레코드 유형에 대한 사용자 정의 필드를 만든 다음 필드를 Workfront Planning 레코드와 연결하여 레코드 정보를 개선할 수 있습니다.


#### 기본 필드로 정의하려면 어떤 필드를 권장합니다.


* ✅ 연결할 때 해당 레코드를 더 쉽게 찾고 &quot;선택&quot;할 수 있도록 고유한 기본 필드 값을 사용하지 마십시오. 

  연결할 때 사용자는 기본 필드의 값을 검색하고 값이 고유하지 않으면 사용자는 선택할 값을 알 수 없습니다. 
* ⛔ 연결 선택 메뉴를 사용할 때 기본 필드를 검색해야 하는 사용자에게 혼동을 줄 수 있으므로 고유하지 않은 값을 기본 필드로 사용하지 마십시오. 

#### 수식을 사용하려면 어떻게 해야 합니까?

* ✅ 수식 필드 형식을 사용하여 수동 입력을 줄이십시오. 테이블 보기에 이미 있는 데이터를 기반으로 정보를 입력할 때 공식을 사용하여 해당 정보를 자동으로 계산하면 시간을 절약할 수 있습니다.

#### 내 작업 영역에서 데이터 연결을 시작하려면 어떻게 해야 합니까?

* ✅ 연결 만들기는 Workfront Planning의 가장 강력한 기능 중 하나입니다. 기록 유형을 서로 연결하거나 Adobe Workfront(프로젝트, 포트폴리오, 프로그램, 회사 및 그룹에 연결)와 Adobe Experience Manager Assets(자산 및 폴더에 연결)와 같은 다른 애플리케이션의 객체 유형이 있는 기록 유형을 연결할 수 있습니다.

  개체 및 레코드 유형을 연결하면 회사의 모든 것이 어떻게 연결되는지에 대한 전체 개요가 제공됩니다.

  예를 들어, **Campaign** 레코드 형식과 **Tactics** 레코드 형식이 있고, 이 두 레코드 형식을 연결하여 특정 **Campaign**&#x200B;에 연결된 **Tactics**&#x200B;을(를) 확인할 수 있습니다.

  연결을 정의한 후 작업 영역의 모든 사용자가 연결 필드를 두 번 클릭하여 **캠페인**&#x200B;에 대한 값을 추가하기 시작할 수 있습니다. 이 필드에서는 사용 가능한 모든 **전술**&#x200B;의 목록을 볼 수 있습니다. 이를 통해 캠페인과 연결해야 하는 전술을 빠르게 찾을 수 있습니다.

#### 조회 필드는 어떻게 사용해야 합니까?

* ✅ 레코드나 개체 형식 간에 연결을 설정한 후 개별 레코드를 서로 연결하고 연결된 레코드나 개체 형식의 필드를 Workfront Planning 레코드에 표시할 수 있습니다. 동일한 정보를 업데이트해야 하는 위치의 수를 줄이고 완벽한 일치성을 보장합니다.

  예를 들어, **Campaign** 레코드 형식과 **Tactics** 레코드 형식 간에 연결이 있으면 기본 필드 정보가 표시되지만 조회 필드를 추가할 때 해당 **Tactical**&#x200B;에 대한 **시작 날짜**&#x200B;와 같은 해당 레코드 형식에서 추가 정보를 가져올 수 있습니다. 이러한 조회 필드의 데이터는 레코드가 추가되면 자동으로 채워집니다.

#### URL에는 어떤 필드 유형이 권장됩니까? 

* ✅ 한 줄 텍스트 필드를 사용하여 URL 데이터를 레코드에 추가합니다.

### 보기

#### 보기와 레코드 유형이 어떻게 되어야 하는지 어떻게 결정합니까?

* ✅단일 구문 또는 명사를 나타내는 항목(예: **Campaigns**)에 대해 레코드 형식을 만드십시오. 

* ⛔ 보기로 더 잘 표현되는 레코드 형식을 만들지 않습니다.

  예를들어 **Calendar**&#x200B;은(는) 레코드 형식 자체가 아니라 레코드 보기이므로 레코드 형식에 적합하지 않은 선택입니다. 

#### 나와 관련이 없는 필드를 숨기거나 삭제해야 합니까?

* ✅ 이 정보가 같은 레코드 종류를 사용하는 다른 사용자와 관련이 있는 경우 열을 삭제하지 않고 숨깁니다. 특정 테이블 보기에서 필드를 삭제하면 이 필드는 이 레코드의 나머지 보기뿐만 아니라 이 레코드 종류가 연결되는 모든 곳에서도 삭제됩니다.

#### 테이블 및 타임라인 보기에서 필터 및 그룹화를 사용하는 방법은 무엇입니까?

* ✅ 필터 및 그룹화가 있는 보기를 사용하여 보아야 할 항목의 스냅숏을 표시합니다. 데이터를 필터링하고 그룹화하여 계획된 항목을 보다 쉽게 이해할 수 있습니다. 메타데이터 필드별로 레코드를 그룹화할 수 있습니다.

  예를 들어, **Target 대상**&#x200B;별로 그룹화하고 **날짜**&#x200B;별로 필터링하여 현재 연도만 표시할 수 있는 **Campaign** 레코드 종류에 대한 타임라인 보기가 있을 수 있습니다.

#### 내 타임라인 보기의 모든 레코드가 표시되지 않는 이유는 무엇입니까?

* ✅ 레코드에 대해 2개의 날짜 필드를 정의해야 합니다. 레코드 종류와 관련된 날짜 필드가 두 개 이상 있는 경우에만 타임라인 보기를 만들 수 있습니다. 시작 또는 종료 날짜 중 하나 또는 둘 다에 값이 없고 시작 날짜가 종료 날짜 이후인 경우 일부 레코드가 타임라인 보기에 표시되지 않을 수 있습니다.

#### 타임라인 보기 설정 사용 방법

* ✅ 보다 시각적으로 풍부한 보기를 만들려면 **막대 스타일** 및 **색상**&#x200B;과 같은 타임라인 보기의 설정을 정의합니다. 의미 있는 이미지가 있는 썸네일을 표시할지 여부를 정의하고 표시줄에 표시할 더 많은 필드(예: **소유자** 또는 **상태**)를 추가하여 **표시줄 스타일**&#x200B;을(를) 사용자 지정할 수 있습니다.

  기본적으로 기본 필드만 표시됩니다. 또한 필드 값(예: 상태 필드와 일치시켜 막대 색상을 사용자 정의)이나 적용한 그룹별로 막대 색상을 정의할 수 있습니다. 기본적으로 색상은 레코드 유형의 색상과 일치합니다.

  레코드 유형 색상이나 색상과 관련된 옵션이 있는 필드만 타임라인에 있는 레코드 막대의 색상에 영향을 줄 수 있습니다.

### 권한 및 공유

공유 기능을 사용하여 직원에게 보기 및 작업 영역에 대한 적절한 권한을 부여합니다.

#### 작업 공간에 대한 권한을 관리하려면 어떻게 해야 합니까?

* ✅ **작업 영역**&#x200B;을(를) 만드는 경우 사용자만 사용할 수 있습니다. 시스템 관리자를 제외한 다른 사용자는 찾을 수 없습니다. 작업 영역이 정의되었으며 팀을 가져와 공동 작업을 시작할 준비가 되면 작업 영역을 작업 영역과 공유하고 해당 권한 수준을 정의해야 합니다.

  다음 권한 수준 중에서 선택할 수 있습니다.

   * **관리**: 사용자가 작업 영역을 편집, 삭제 및 공유할 수 있습니다.
   * **참여**: 사용자는 레코드를 만들고 편집하고 삭제할 수 있습니다.
   * **보기**: 사람들이 레코드를 볼 수 있습니다.

* ✅ 많은 고객이 대부분의 사용자에게 작업 영역에 대한 **관리** 권한을 부여할 것으로 생각하지만, 실수로 레코드 형식을 삭제하거나 불필요한 레코드 형식 및 필드를 만들지 않는 신뢰할 수 있는 사용자 선택 그룹에 대한 **관리** 권한을 제한하지 마십시오. 작업 영역을 편집, 공유 및 삭제할 수도 있습니다. 이 수준의 권한은 사용자에게 Workspace에 대한 전체 관리 액세스 권한을 부여합니다.

  작업 공간에 대한 관리 권한을 가지려면 Standard 사용자 라이선스가 필요합니다.

* ✅ 레코드를 만들고, 편집하고, 삭제할 수 있도록 하되 작업 영역의 구조와 스키마를 변경하지 않도록 하려면 **Contribute** 사용자에게 권한을 부여합니다. **Contribute** 사용 권한이 있으면 레코드 형식을 만들거나 기존 레코드 형식의 필드를 변경할 수 없습니다.

  작업 영역에 대한 **Contribute** 권한을 가지려면 Standard 사용자 라이선스가 필요합니다.

* ✅ 레코드를 보려면 사용자에게 **보기** 권한을 부여합니다.

  >[!NOTE]
  >
  >현재 레코드 종류 또는 레코드에 대한 특정 권한이 없으므로 작업 영역에 대한 **보기** 액세스 권한을 다른 사용자에게 부여하면 모든 레코드 종류의 모든 레코드가 표시됩니다.


#### 레코드 유형에 대한 권한을 관리하려면 어떻게 해야 합니까?

* ✅ 작업 영역에 대한 관리 권한이 있는 사용자는 레코드 형식에 대해 사용 권한을 낮출 수 없습니다. 레코드 유형에 대한 관리 권한도 상속합니다. 사용자에게 작업 영역에 대한 관리 권한을 부여할 수 없지만, 기록 유형에 대해서는 기여 또는 보기 권한을 부여할 수 있습니다.
* ✅ 사용자가 작업 영역에 비해 레코드 유형에 대한 권한 수준(예: 보기 권한)이 낮도록 하려면 작업 영역에 Contribute 권한을 부여하는 것이 좋습니다. 그런 다음 레코드 유형에 대한 보기 권한을 부여할 수 있습니다.
* 레코드 유형의 권한에서 사용자를 제거하면 여전히 작업 영역에 대해 최소 보기 권한이 제공됩니다.

#### 보기에 대한 권한을 관리하려면 어떻게 해야 합니까?

* ✅ 보기를 편집, 삭제 및 공유할 수 있도록 **관리** 권한을 제한합니다. 즉, 필터, 그룹화 필드 또는 보기의 일부 구성을 변경할 수 있습니다. 이러한 변경 사항은 보기를 사용하는 모든 사용자의 기본 보기 구성에 영향을 줍니다.

  보기에 대한 관리 권한이 있는 사용자에게 표준 사용자 라이선스가 필요합니다.

* ✅ 사용자에게 **보기** 액세스 권한을 부여하여 보기를 적용할 수 있도록 합니다. 일부 필터 또는 그룹화와 정렬을 변경할 수 있지만 이러한 변경 사항은 일시적일 뿐 뷰에 액세스하는 다른 모든 사용자에 대해서는 변경 사항이 저장되지 않습니다. 이러한 변경 사항은 보기를 사용하는 다른 모든 사용자의 기본 구성에 영향을 주지 않습니다.  해당 변경 사항은 수정된 설정을 적용하는 사용자만 볼 수 있습니다. 화면을 새로 고치면 변경 사항이 기본값으로 재설정됩니다.

* ✅ 작업 영역을 볼 수 있는 모든 사람이 해당 특정 보기의 레코드와 해당 필드를 볼 수 있도록 하려면 **작업 영역의 모든 사람에게** 사용 권한을 부여합니다. 이렇게 하면 보기에 대한 공유 권한 상자에 수동으로 다른 사용자를 추가할 필요가 없습니다.

  >[!NOTE]
  >
  >보기가 공유되지 않았으며 이 보기에 대한 링크를 다른 사용자와 공유하는 경우 **기본 표 보기**&#x200B;에서 레코드를 볼 수 있습니다. 표준 Workfront 라이선스가 있는 경우 자체 보기를 빌드할 수 있습니다.


#### **Workspace 공유**&#x200B;와(과) **공유 보기**&#x200B;의 차이점은 무엇입니까?

* **Workspace 공유**&#x200B;는 작업 영역, 해당 레코드 종류, 레코드 및 필드에 대한 사용자의 액세스 권한을 정의합니다.

* **보기 공유**&#x200B;는 사용자가 만든 보기를 볼 수 있는지 여부와 필터, 그룹화 필드 또는 보기의 다른 구성을 변경할 수 있는지 여부를 정의합니다. 보기 내에 표시되는 레코드의 가시성은 보기 공유가 아니라 Workspace 공유에 의해 제어됩니다.

#### Workfront 라이선스 유형이 Workfront Planning 권한에 어떤 영향을 줍니까?

* **Workspace 공유**&#x200B;의 경우: Light 및 Contribute 라이선스 사용자는 작업 영역에 대한 보기 액세스만 얻을 수 있습니다. 다른 사용자에게 작업 영역에 대한 기여 또는 관리 권한을 부여하려면 Standard 라이센스가 있어야 합니다.

* **보기 공유**: 작업 영역에 대한 관리 권한이 있는 표준 라이선스 사용자가 보기를 만들 수 있습니다. Light 및 Contribute 라이선스 사용자는 Standard 사용자가 만들고 공유한 보기만 사용할 수 있습니다. 그렇지 않으면 사용자가 **기본 테이블 보기**&#x200B;를 볼 수 있습니다.


#### Workspace 소유자가 변경되면 어떻게 해야 합니까?

* Workfront은 작업 영역 작성자를 소유자로 설정하지만, 기능상 소유자는 관리 권한이 있는 사용자와 동일한 권한을 갖습니다.
* 소유자가 비활성화되면 다른 구성원은 중단 없이 작업 영역에서 작업을 계속할 수 있습니다.
* 시스템 관리자는 모든 작업 영역에 액세스할 수 있으므로 소유자가 관리 권한을 가진 유일한 사람이었던 경우 관리자는 다른 사람을 추가하고 관리자에게 작업 영역 관리를 처리할 관리 권한을 부여할 수 있습니다.

### Workfront Planning에서 요청 제출

사용자가 레코드 유형의 페이지 외부에 레코드를 추가하도록 하려면 각 레코드 유형에 대한 요청 양식을 만들 수 있습니다. 양식을 제출하면 레코드 유형에 새 레코드가 추가됩니다.

#### 레코드 유형에 대한 요청 양식을 언제부터 만들어야 합니까?

* ✅ 테이블에 필요한 필드를 추가하여 레코드 형식 구조를 먼저 설정해야 합니다. 이러한 필드는 레코드에 대해 설명하며 양식 빌더에서 액세스할 수 있습니다.

  레코드 유형 구조가 완료된 후 요청 또는 접수 양식을 작성하여 키 필드가 누락되지 않도록 하는 것이 좋습니다.

#### 누가 요청 양식을 만들 수 있습니까?

* ✅ 작업 영역에 대한 관리 액세스 권한이 있는 모든 사용자는 요청 양식을 만들거나 편집할 수 있습니다. 이 기능을 허용하도록 사용자의 권한이 제대로 할당되었는지 확인하십시오.

#### 레코드 유형에 대한 요청 양식을 만들거나 편집하려면 어떻게 해야 합니까?

* ✅ 작업 영역에 대한 관리 액세스 권한이 있는 모든 사용자는 문서 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)에 설명된 단계를 따를 수 있습니다.


#### 누가 요청서를 사용하여 새로운 기록을 제출할 수 있습니까?

* ✅ 제출 권한은 각 양식에 대해 구성하는 설정에 따라 다릅니다.

  양식 빌더에서 양식을 게시한 후 요청을 제출할 수 있는 사용자를 제어하는 권한을 관리할 수 있습니다.

  다음 세 가지 공유 옵션 중에서 선택할 수 있습니다.

   * **작업 영역에 대한 보기 이상의 액세스 권한이 있는 모든 사용자:** 작업 영역에 대한 보기 이상의 권한이 있는 모든 사용자는 레코드를 만드는 요청을 제출할 수 있습니다.
   * **작업 영역에 대한 기여자 이상의 액세스 권한이 있는 사용자**: 작업 영역에 대한 기여자 이상의 사용 권한이 있는 사용자에 대한 제출을 제한합니다.
   * **다음 링크를 가진 모든 사용자:** 양식 링크를 가진 모든 사용자가 요청을 제출할 수 있습니다.
   * **만료 날짜:** 보안을 강화하려면 공개 링크의 만료 날짜를 설정해야 합니다.

### 요청 양식 관리에 대한 우수 사례

다음은 요청 양식 관리를 위한 권장 사항입니다.

* 미리 계획하기: 나중에 과도한 수정을 방지하기 위해 양식을 만들기 전에 요청자에게 필요하거나 필요한 정보를 명확히 정의합니다.
* 일반 레이블 사용: 필드 레이블과 설명이 모든 사용자에게 명확하고 이해 가능한지 확인하십시오.
* 테스트 양식: 새 양식을 더 많은 대상자에게 롤아웃하기 전에 양식 링크 및 양식 미리 보기 옵션을 사용하여 테스트하여 모든 필드 및 논리가 예상대로 작동하는지 확인하십시오.
* 양식 업데이트 유지: 정기적으로 양식을 검토하고 레코드 유형 구조 또는 운영 프로세스의 변경 사항에 맞게 업데이트하십시오.

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/ko/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/ko/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/ko/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->
