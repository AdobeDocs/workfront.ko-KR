---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 현재 사용 가능한 Adobe Workfront Fusion 템플릿
description: 현재 Adobe Workfront Fusion에서 사용할 수 있는 공용 템플릿은 다음과 같습니다.
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: 2211431b4c4e3d751519fe8441cfa578e713ac77
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# 현재 사용 가능한 Adobe Workfront Fusion 템플릿

현재 Adobe Workfront Fusion에서 사용할 수 있는 공용 템플릿은 다음과 같습니다.

팀이나 조직에 다른 팀에서 만든 템플릿을 사용할 수 있습니다.

사용 가능한 템플릿을 보려면 **템플릿** 아이콘 ![](assets/fusion-template-icon.png) Fusion의 측면 탐색 메뉴에서 을 클릭합니다.

## Workfront 템플릿

이러한 템플릿은 Workfront 프로세스 및 워크플로를 자동화합니다.

### [!BADGE 신규!]{type=Informative}

이 자동화는 사용자 정의 양식이 있는 프로그램의 새 프로젝트를 감시합니다. 그런 다음 해당 프로그램 사용자 정의 양식 및 필드를 새 프로젝트에 추가합니다.

### [!BADGE 신규!]{type=Informative}

이 자동화는 사용자 정의 양식으로 포트폴리오의 새 프로젝트를 감시합니다. 그런 다음 해당 포트폴리오 사용자 정의 양식 및 필드를 새 프로젝트에 추가합니다.

### Workfront - 승인된 문제를 프로젝트로 전환

이 템플릿은 문제를 프로젝트로 변환합니다. 조직의 표준에 맞게 수정할 수 있습니다.

### 필드 변경에 따른 맞춤 알림

이 템플릿은 필드 값 변경과 같은 일부 고유 이벤트를 기반으로 Workfront 프로젝트에서 작업하는 개인에게 맞춤 업데이트(및 관련 알림)를 만듭니다. 시나리오는 작업 또는 문제에서 지정된 필드가 변경될 때 Workfront을 감시합니다. 이 경우 시나리오에서는 관련 프로젝트의 정보를 평가하고 프로젝트의 특정 역할에 할당된 사용자에 대한 맞춤 업데이트를 만듭니다.

### Workfront - 규칙을 사용하여 프로젝트 이름에 일괄 추가

이 벌크 업데이트 템플릿은 검색 기준을 충족하는 모든 프로젝트(포트폴리오 내에 포함)의 이름을 바꾸고 표준 형식으로 변경합니다.

### Workfront - 규칙을 사용하여 프로젝트 이름 변경

이 템플릿은 필터(포트폴리오 내에 있음)의 기준을 충족하는 모든 프로젝트를 찾은 다음 표준 형식으로 이름을 바꿉니다.

### Workfront - 상태 변경 시 기준선 만들기

이 템플릿은 &quot;스위치&quot; 모듈에 기록된 프로젝트 상태 변경 시 프로젝트 베이스라인을 캡처하고 로깅을 위해 업데이트 스트림에 업데이트를 만듭니다.

### Workfront - 주별 기준선 만들기

이 템플릿은 포트폴리오로 필터링된 프로젝트에 대해 매주 월요일 오전 6시(ET 기준)에 프로젝트 기준선을 캡처하고 로깅을 위해 업데이트 스트림에 업데이트를 만듭니다.

### [!BADGE 신규!]{type=Informative}

한 달에 한 번, 자체 정책을 사용하여 프로젝트 템플릿을 검토하십시오. 이를 통해 손쉽게 관리할 수 있습니다. 템플릿을 사용하면 정책을 위반하는 템플릿에 대해 적절한 사용자에게 알릴 수 있습니다.

## Workfront - Workfront 증명 템플릿

이러한 템플릿은 Workfront과 Workfront Proof를 결합하는 워크플로를 자동화합니다.

### Workfront 증명 > Workfront - 증명 결정에 대한 프로젝트 업데이트

프로젝트에 직접 추가된 Proof에 대한 결정이 내려지면 이 자동화는 결정 주체 등 Proof 결정에 대한 정보를 수집한 다음 해당 Workfront 프로젝트에 이 진행 상황을 업데이트로 반영합니다.

### Workfront 증명 > Workfront - 증명 결정에 대한 작업 업데이트 및 완료(승인된 경우)

개별 증명이 개별 작업에 연결된 경우 이 시나리오는 증명에 대한 승인 결정이 내려지면 관련 작업을 닫습니다. 승인되면 작업이 완료되고 프로젝트가 업데이트됩니다.

## HTTP - Workfront 템플릿

이러한 템플릿은 웹 서비스에서 정보를 검색하고 해당 정보를 Workfront으로 가져옵니다.

>[!NOTE]
>
> 이 섹션의 템플릿을 사용하려면 작업 자동화 및 통합용 Workfront Fusion 라이선스가 있어야 합니다.

### APILayer > Workfront - 일일 환율 업데이트 (EUR)

이 템플릿은 설정된 시점의 환율 업데이트를 자동화하는 시나리오를 만듭니다. 이 시나리오는 APIlayers.com API에서 유로(EUR) ~ 미국 달러(USD) 요금을 가져오고 Workfront에서 요금을 업데이트합니다.

## Workfront-Marketo 틀

이러한 템플릿은 Workfront-Marketo 통합을 지원합니다.

>[!NOTE]
>
> 이 섹션의 템플릿을 사용하려면 작업 자동화 및 통합용 Workfront Fusion 라이선스가 있어야 합니다.

### Workfront 승인 워크플로우로 Marketo Engage 이메일 초안 승인

이는 Workfront과 Marketo Engage 간의 검토 및 승인 통합의 일부입니다. 이 템플릿은 Workfront의 이메일 증명이 승인되었는지 감지한 다음, Marketo Engage에서 해당 이메일을 승인됨으로 업데이트합니다.

### Workfront에서 마케팅 캠페인 요청 접수 및 Marketo Engage에서 캠페인 생성 자동화

이 시나리오는 Workfront에서 만든 요청으로 Marketo Engage에서 이메일 및 웨비나 캠페인을 만드는 프로그래밍 방식을 제공합니다. 자동화를 사용하여 캠페인을 만들고, 구성하고, 구성함으로써 팀은 효율성을 향상시킬 수 있습니다.

### Workfront에서 Marketo Engage 이메일 초안의 이메일 증명 검토

이 템플릿은 Workfront 작업이 검토 준비됨 상태로 설정되어 있는지 감지한 다음, Marketo Engage에서 이메일 초안을 내보내어 Workfront의 증명으로 저장합니다.

## Workfront-아나플란 틀

이러한 템플릿은 Workfront-Anaplan 통합을 지원하며 Workfront의 두 Anaplan 모두에서 특정 구성을 예상합니다. 이러한 템플릿 및 필수 구성에 대한 자세한 내용은 개별 템플릿 문서를 참조하십시오.

Workfront-Anaplan 통합에 대한 자세한 내용은 [Adobe Workfront과 Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> 이 섹션의 템플릿을 사용하려면 작업 자동화 및 통합용 Workfront Fusion 라이선스가 있어야 합니다.

### 지출 최적화 워크플로우

* [보내기 [!DNL Adobe Workfront] 프로젝트 업데이트: [!DNL Anaplan] 목록 항목](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [보내기 [!DNL Adobe Workfront] 에 대한 경비 [!DNL Anaplan] 목록 항목](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [보내기 [!DNL Adobe Workfront] 에 대한 실제 시간 업데이트 [!DNL Anaplan] 목록 항목](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### 예산 요청 연결을 위한 워크플로

* [만들기 [!DNL Anaplan] 의 목록 항목 [!DNL Adobe Workfront] 예산 요청](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [적용 [!DNL Anaplan] 에 대한 예산 할당 [!DNL Adobe Workfront] 프로젝트](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### 캠페인 요청 연결을 위한 워크플로우

* [만들기 [!DNL Anaplan] 의 목록 항목 [!DNL Adobe Workfront] 캠페인 요청](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [적용 [!DNL Anaplan] 에 대한 예산 할당 [!DNL Adobe Workfront] 캠페인 요청 또는 캠페인 프로젝트](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
