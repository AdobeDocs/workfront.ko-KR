---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 연결된 폴더 및 문서 마이그레이션
description: API를 사용하여 연결된 폴더 및 문서를 Adobe Experience Manager Assets으로 마이그레이션할 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# 연결된 폴더 및 문서 마이그레이션

API를 사용하여 연결된 폴더 및 문서를 Adobe Experience Manager Assets으로 마이그레이션할 수 있습니다.

## 프로시저

1. 이전 외부 문서 스토리지 공급자와 연결된 모든 문서 및 폴더를 식별하고 포함된 폴더의 폴더 ID와 Workfront 내부 문서 또는 폴더 식별자를 확인합니다.

   >[!NOTE]
   >
   > 검색된 모든 폴더 또는 문서가 새 공급자에 대한 링크를 아직 만들지 않았는지 확인해야 합니다.

1. 새 저장소에서 경로별로 문서 및 폴더를 찾은 다음 외부 시스템에서 해당 ID를 조회합니다.

1. 내부 Workfront ID와 새 외부 저장소의 ID에 대한 매핑을 만듭니다. 다음 단계에서 새 링크를 만들려면 이 과정이 필요합니다.

1. 새 외부 ID를 통해 새 위치의 리소스를 가리키는 Workfront에서 새 문서 또는 문서 폴더 링크를 만듭니다.

   1. **문서**: 새 외부 문서 공급자를 사용하여 기존 문서의 새 버전을 추가합니다.
   1. **폴더**: 같은 위치에 같은 이름으로 새 폴더를 만듭니다.

>[!CAUTION]
>
>   연결된 기존 폴더는 삭제하지 마십시오. 이로 인해 데이터가 손실될 수 있습니다. Workfront 애플리케이션에서 이전 폴더 링크를 제거하려면 설정 영역에서 사용자 정의 문서 통합을 비활성화하십시오.


## 링크 마이그레이션 예제 프로세스

![간소화된 링크 흐름](assets/links-flow-simplified.png)

## API 정보

이 섹션에서 Workfront API에 대한 자세한 내용은 [개발자 설명서:문서](https://developer.workfront.com/documents.html)를 참조하십시오.

### 모든 문서 찾기

**documentProviderID**&#x200B;을(를) 사용하여 **providerType**&#x200B;의 **문서 공급자**&#x200B;에 연결된 모든 **문서(DOCU)**&#x200B;를 찾으십시오.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API 문서 참조](https://developer.workfront.com/documents.html#get-/docu/search)

### 모든 폴더 찾기

**documentProviderID**&#x200B;을(를) 통해 **providerType**&#x200B;의 문서 공급자에 연결된 모든 **DOCFDR(문서 폴더)**&#x200B;을(를) 찾으십시오.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API 문서: (현재 developer.workfront.com에서 다루지 않는 문서 폴더 엔드포인트)

### 문서 연결

**documentProviderID**&#x200B;을(를) 사용하여 **providerType**&#x200B;의 **외부 문서 공급자**&#x200B;에서 **문서(DOCU)**&#x200B;를 연결합니다.

>[!IMPORTANT]
>
>문서가 일시적으로 저장됩니다. 즉, 문서의 모든 버전에 액세스할 수 있습니다. 링크를 만들 때 기존 문서 ID를 지정할 수 있으므로 해당 문서에 새 버전을 작성하고 새 공급자의 외부에서 데이터를 호스팅합니다. 이 문서 ID는 교체하는 문서 링크에 있는 문서 ID와 동일합니다. 동일한 개념의 문서입니다. 이 새 버전의 바이트가 다른 공급자와 함께 저장되었음을 나타내는 것입니다.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API 문서: (현재 developer.workfront.com에서 다루지 않는 내부 링크 엔드포인트)

### 링크 폴더

**documentProviderID**&#x200B;을(를) 사용하여 **providerType**&#x200B;의 **외부 문서 공급자**&#x200B;에서 **문서 폴더(DOCFDR)**&#x200B;에 연결합니다.

>[!IMPORTANT]
>
>폴더 링크의 경우 문서 링크와 달리 새 링크를 배치할 Workfront의 폴더에 대한 &#39;documentFolderId&#39;가 필요합니다. 이는 복사하는 연결된 폴더와 동일한 상위 폴더입니다.

>[!CAUTION]
>
>폴더는 일시적으로 저장되지 않습니다. 이전 폴더는 삭제하지 마십시오. 설정 영역에서 사용자 정의 문서 통합을 비활성화하여 이전 폴더를 제거합니다.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API 문서: (현재 developer.workfront.com에서 다루지 않는 내부 링크 엔드포인트)

## 중요 용어

* **문서**: Workfront 내의 디지털 에셋

* **문서 폴더**: Workfront 내의 디지털 에셋에 대한 컨테이너입니다.

* **문서 ID**: 디지털 에셋의 Workfront 내부 ID

* **문서 폴더 ID**: 디지털 자산 폴더의 Workfront 내부 ID

* **문서 공급자 ID**: 특정 문서 공급자와 연결된 ID

>[!IMPORTANT]
>
> 주어진 문서 공급자 유형의 경우 고객에게 연결된 인스턴스가 여러 개 있을 수 있습니다. 예를 들어 여러 AEM 저장소가 연결되어 있을 수 있습니다. 또는 여러 Google 드라이브 인스턴스가 연결되어 있습니다. 문서 공급자 ID는 대체하거나 전환할 연결 유형의 특정 인스턴스를 나타냅니다.

* **문서 저장소 공급자 유형(또한 &quot;외부 통합 유형&quot;)**: Workfront에서 지원하는 문서 저장소 공급자 통합 유형입니다. 전용 통합 또는 &quot;사용자 정의 통합&quot;을 통해.

* **현재 문서 저장소 공급자 형식( providerType)**:

  ```
  ATTASK
  BOX
  GOOGLE
  SHAREPOINT
  WEBDAM
  WORKFRONTDAM
  INFERNO
  WIDEN
  DROPBOX
  DROPBOX_BUSINESS
  ONEDRIVE
  QUIP
  WEBHOOKS
  AEM
  MOCK
  ```

* **연결된 문서**: 외부 문서 저장소 공급자에서 호스팅되는 디지털 자산입니다. Workfront에는 자산에 대한 자체 내부 &quot;문서 ID&quot;가 있지만 바이트는 외부에 저장됩니다. 이를 용이하게 하기 위해 Workfront은 &quot;외부 문서 ID&quot;를 저장하여 외부에서 참조한 리소스를 원격 리포지토리 또는 저장소 내에서 찾을 수 있도록 합니다.

* **연결된 문서 폴더**: 외부 문서 저장소 공급자에서 호스팅되는 디지털 에셋의 컨테이너입니다. Workfront에는 자산에 대한 자체 내부 &quot;문서 폴더 ID&quot;가 있지만 바이트는 외부에 저장됩니다. 이를 용이하게 하기 위해 Workfront은 &quot;외부 문서 ID&quot;를 저장하여 외부에서 참조한 리소스를 원격 리포지토리 또는 저장소 내에서 찾을 수 있도록 합니다.

* **외부 문서 ID**: 자산이 Workfront 외부에 저장되어 있을 때 할당된 ID입니다. Workfront은 이 &quot;외부 문서 식별자&quot; 필드를 통해 내부 식별자를 외부 시스템에서 에셋을 찾는 데 사용되는 식별자에 매핑합니다. 따라서 새 외부 저장소에서 문서나 폴더를 연결할 때는 외부 문서 공급자가 새 저장소나 저장소에서 문서를 식별할 수 있는 적절한 형식으로 새 외부 문서 식별자를 작성해야 합니다.

  >[!NOTE]
  >
  > Workfront에는 아직 외부 문서 식별자에 대한 표준이 없습니다. AEM ID에 새 사양이 사용되고 있지만, 다른 ID의 경우 외부 문서 ID는 공급자 유형에 따라 다른 양식을 사용할 수 있습니다.


* **개체 유형**: 이 문서의 목적에 맞는 API 전용 용어입니다. 상호 작용하려는 Workfront 내의 일반 오브젝트 유형입니다. 이 경우 &quot;DOCU&quot; 및 &quot;DOCFDR&quot; 유형이 각각 포함된 문서 및 폴더와 상호 작용하게 됩니다.

* **개체 ID**: 상호 작용하려는 일반 개체의 내부 Workfront 식별자입니다. 문서 및 폴더와 상호 작용하므로 각각 문서 ID 또는 문서 폴더 ID가 됩니다.
