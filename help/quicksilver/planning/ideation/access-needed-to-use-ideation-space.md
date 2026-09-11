---
title: 관념화 공간을 사용하는 데 필요한 액세스
description: 이제 Adobe Workfront Planning에서는 캠페인을 시작하기 전에 식별할 수 있는 추가 기능을 제공합니다. AI의 기능을 활용하여 데이터와 직접 입력을 가시적인 계획으로 전환하고 Adobe Ideation 공간의 빈 페이지가 아닌 정보에 입각한 시작점을 팀에 제공합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---


# 관념화 공간을 사용하는 데 필요한 액세스 권한

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. **관념화 공간 Beta** 프로그램의 일부로서만 사용할 수 있습니다. </span>

<span class="preview">자세한 내용은 [Adobe Workfront Planning의 Ideation 공간 시작](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)을 참조하십시오.</span>


{{planning-important-intro}}

이제 Adobe Workfront Planning에서는 캠페인을 시작하기 전에 식별할 수 있는 추가 기능을 제공합니다. AI의 기능을 활용하여 데이터와 직접 입력을 가시적인 계획으로 전환하고 Adobe Ideation 공간의 빈 페이지가 아닌 정보에 입각한 시작점을 팀에 제공합니다.

이 문서에서는 Workfront Planning에서 Ideation 공간에 액세스하는 데 필요한 액세스 및 권한에 대해 설명합니다.

관념화 공간에 대한 일반적인 정보는 [Adobe Workfront Planning의 관념화 공간 시작](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)을 참조하십시오.

## 제품 요구 사항

관념화 공간은 독립 실행형 제품이 아닙니다. Workfront Planning 패키지가 필요하며 Workfront Planning에서만 액세스할 수 있습니다. 추가 제품도 필요합니다.

Ideation 공간에 액세스하려면 조직에서 다음 제품에 대한 패키지를 구매해야 합니다.

* Planning 패키지 외에 Adobe Workfront Workflow 패키지

  또는

  독립 실행형 제품으로 구입한 Adobe Workfront Planning.
* Adobe GenStudio for Performance Marketing 라이선스

  >[!TIP]
  >
  >GenStudio for Performance Marketing은 올바른 글꼴 권한에 액세스할 수 있어야 합니다.


<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Workfront Planning 액세스 수준 요구 사항

관념화 공간 액세스가 Workfront에서 구성되었습니다.

Ideation 공간에 액세스하려면 Workfront 액세스 수준에 다음 항목이 포함되어야 합니다.

* 표준 워크플로 라이선스(회사에서 Planning 패키지 외에 워크플로 패키지를 구입한 경우).
* 표준 계획 라이선스(회사가 워크플로우 및 계획 패키지 또는 Workfront Planning을 독립형 제품으로 구입한 경우)
* 액세스 수준의 추가 제한 설정 섹션에서 관념화 공간 사용 안 함 설정을 선택 취소해야 합니다. <!--***********check the UI for this***********-->

## Workfront Planning 권한 요구 사항

각 Planning 레코드는 Ideation Space에서 하나의 간결에 연결됩니다.

관념화 공간 개요 권한은 Workfront Planning 레코드 권한에서 상속됩니다. <!--not sure if this is right, because now you can share the ideation with others??-->

Planning에서 레코드 유형에 대한 관리 권한이 있어야 Ideation Space에서 레코드를 만들거나 편집할 수 있습니다.

레코드에 대한 보기 권한이 있는 Planning 사용자는 레코드의 아이디어 공간을 볼 수 있습니다.

다음 표는 Workfront Planning 레코드 권한과 Ideation Space Brief 권한 간의 연결을 보여 줍니다.

| 레코드 수준 권한 계획 | 관념화 공간 개요 수준 권한 |
|---|---|
| 레코드에 대한 권한 관리 | 레코드의 관념화 공간에 간단한 설명을 만들 수 있습니다. |
| 레코드에 대한 권한 보기 | 관념화 공간에서 해당 레코드의 개요를 읽을 수 있지만 수정할 수는 없습니다 |

## 관념화 공간 권한

<!--this is also duplicated in the intro of the Share an ideation space article-->

계획 권한은 레코드의 관념화 공간으로 전송됩니다.

또한 다른 사용자에게 아이디어 공간을 사용하고 아이디어를 추가할 수 있는 권한을 부여할 수 있습니다.

다음 사항을 고려하십시오.

* 아이디어 생성자는 항상 자신의 아이디어에 대한 편집기 권한을 가집니다.

* 브리프를 만들고 다른 응용 프로그램으로 내보내려면 아이디어 공간에 대한 편집기 권한이 있어야 합니다.

다음은 관념화 공간 권한 및 이들이 제공하는 기능입니다.

| 관념화 공간 권한 | 기능 |
|---|---|
| 편집자 | 관념화 공간을 편집, 다운로드 및 공유할 수 있음 |
| Comenter | 관념화 공간을 보고 코멘트할 수 있음 |
| 뷰어 | 관념화 공간을 볼 수 있음 |

관념화 공간 공유에 대한 자세한 내용은 [관념화 공간 공유](/help/quicksilver/planning/ideation/share-the-ideation-space.md)를 참조하십시오.

<!--there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
