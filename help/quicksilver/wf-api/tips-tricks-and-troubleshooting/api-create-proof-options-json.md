---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API를 사용하여 고급 언어 교정 옵션 추가
description: Adobe Workfront API를 사용하여 고급 언어 교정 옵션 추가
author: Becky
feature: Workfront API, Workfront Proof
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# Adobe Workfront API를 통해 증명을 만들 때 고급 교정 옵션을 추가합니다

Workfront API에서 증명을 만들 때 고급 교정 옵션을 추가할 수 있습니다.

다음 워크플로우 중 하나를 사용하여 API를 사용하여 증명 옵션을 추가할 수 있습니다.

* (권장) Workfront API를 사용하여 간단한 증명을 만든 다음 ProofHQ API를 사용하여 증명에 고급 교정 옵션을 추가합니다

* Workfront API에서 JSON을 사용하여 고급 교정 옵션이 있는 증명 만들기

## Workfront 및 ProofHQ API를 사용하여 증명 만들기(권장) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

이 섹션에서는 Workfront 및 ProofHQ API의 조합을 사용하여 Workfront API를 통해 고급 교정 옵션이 있는 증명을 만드는 방법을 설명합니다.

ProofHQ API에는 Workfront API에서 증명을 사용할 수 없는 다양한 작업이 포함되어 있습니다. 이러한 작업을 사용하면 Workfront API에서 사용할 수 있는 것보다 더 정밀하게 증명을 수정하거나 구성할 수 있습니다.

ProofHQ API에 대한 개요는 다음을 참조하십시오. [PofHQ 개요](../../proofhq-api/general/overview.md). 또한 [증명 HQ 설명서](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* Workfront API는 REST-ful API입니다. ProofHQ API는 SOAP API입니다.
>* ProofHQ API에서 만든 증명이 Workfront에 자동으로 연결되어 있지 않습니다. 따라서 ProofHQ API로 업데이트하기 전에 Workfront API에서 증명을 만드는 것이 좋습니다.
>


### 고급 교정 옵션을 사용하여 증명 만들기

1. 를 사용하여 증명 만들기 `Document createProof` 작업 을 참조하십시오.

   >[!NOTE]
   증명을 만들 때는 advancedProofingOptions 매개 변수에 값을 포함하지 마십시오.

1. 증명을 만든 후 ProofHQ API를 사용하여 고급 옵션을 추가합니다.

### 예

이 섹션에서는 ProofHQ API로 만들 수 있는 몇 가지 샘플 업데이트를 보여줍니다.

**예:**

* [증명을 다운로드하여 메시지를 관리하고 공개적으로 공유할 수 있습니다](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [비공개 단계가 아니며, 필수가 아니며, 하나의 승인만 필요하도록 스테이지를 업데이트합니다](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [기본 의사 결정자가 없는 증표에 두 명의 수신자를 추가합니다](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**증명을 다운로드하여 메시지를 관리하고 공개적으로 공유할 수 있습니다**

이 종단점에 대한 설명서는 [증명HQ API 업데이트 증명](https://api.proofhq.com/home/proofs/updateproof.html) 페이지.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**비공개 단계가 아니며, 필수가 아니며, 하나의 승인만 필요하도록 스테이지를 업데이트합니다**

이 종단점에 대한 설명서는 [증명HQ API 업데이트WorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) 페이지.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**기본 의사 결정자가 없는 증표에 두 명의 수신자를 추가합니다**

이 종단점에 대한 설명서는 [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) 페이지.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Workfront API에서 JSON을 사용하여 증명 만들기

이 섹션에서는 Workfront API에서 매개 변수 값으로 JSON을 사용하여 Workfront API를 통해 고급 교정 옵션이 있는 증명을 만드는 방법을 설명합니다

### 고급 교정 옵션을 사용하여 증명 만들기

Workfront API를 사용하여 증명을 만들 수 있습니다 `Document createProof` 작업. 이 작업은 `advancedProofingOptions` 매개 변수 - 값 유형이 `string`. 고급 교정 옵션을 `createProof` 작업을 수행하려면 `advancedProofingOptions` 매개 변수에 채울 수 있습니다.

>[!NOTE]
advancedProofingOptions JSON에 포함할 필드를 예측하기가 어려울 수 있습니다. Workfront에서 고급 언어 처리를 사용하는 동안 조직의 네트워크 데이터를 검사하고, JSON을 조직에서 일반적으로 사용하는 필드 및 값에 기반을 둘 수 있습니다.
이러한 필드를 예측하기 어려울 수 있으므로 Workfront API를 사용하여 증명을 만든 다음 ProofHQ API를 사용하여 업데이트하는 것이 좋습니다. 자세한 내용은 [Workfront 및 ProofHQ API를 사용하여 증명 만들기(권장)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) 이 문서

### 예

이 예는 용 JSON을 만들 때 사용할 수 있는 필드와 형식을 보여줍니다. `advancedProofingOptions` 매개 변수. 사용자 `advancedProofingOptions` JSON 파일에는 여기에 표시된 것보다 더 많거나 적은 필드가 있을 수 있습니다.

**예:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
