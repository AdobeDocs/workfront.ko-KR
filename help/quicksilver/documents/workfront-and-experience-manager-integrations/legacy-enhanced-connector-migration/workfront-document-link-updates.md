---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 연결된 폴더 및 문서 마이그레이션
description: API를 사용하여 연결된 폴더 및 문서를 Adobe Experience Manager Assets에 마이그레이션할 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 연결된 폴더 및 문서 마이그레이션

API를 사용하여 연결된 폴더 및 문서를 Adobe Experience Manager Assets에 마이그레이션할 수 있습니다.

## 프로시저

1. 이전 외부 문서 저장소 공급자와 연결된 모든 문서 및 폴더를 식별하고 Workfront 내부 문서 또는 폴더 식별자와 포함된 폴더의 폴더 ID를 확인합니다.

   >[!NOTE]
   >
   > 검색된 모든 폴더 또는 문서를 확인하여 새 공급자와 해당 폴더에 대한 링크를 아직 만들지 않았는지 확인해야 합니다.

1. 새 저장소에서 문서와 폴더를 경로별로 찾은 다음 외부 시스템에서 해당 ID를 찾습니다.

1. 새 외부 저장소의 ID에 내부 Workfront ID를 매핑하는 작업을 만듭니다. 다음 단계에서 새 링크를 만들려면 이 방법이 필요합니다.

1. Workfront에서 새 외부 ID를 통해 새 위치의 리소스를 가리키는 새 문서 또는 문서 폴더 링크를 만듭니다.

   1. **문서**: 새 외부 문서 공급자를 사용하여 기존 문서의 새 버전을 추가합니다.
   1. **폴더**: 같은 위치에 같은 이름으로 새 필터를 만듭니다.

>[!CAUTION]
>
>   기존 연결된 폴더는 삭제하지 마십시오. 이로 인해 데이터 손실이 발생할 수 있습니다. Workfront 애플리케이션에서 이전 폴더 링크를 제거하려면 설정 영역에서 사용자 지정 문서 통합을 비활성화합니다.


## 링크 마이그레이션을 위한 예제 프로세스

![간소화된 링크 흐름](assets/links-flow-simplified.png)

## API 정보

이 섹션의 Workfront API에 대한 자세한 내용은 [개발자 설명서: 문서](https://developer.workfront.com/documents.html).

### 모든 문서 찾기

모두 찾기 **문서(DOCU)** 에 연결됨 **문서 공급자** 의 **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API 문서 참조](https://developer.workfront.com/documents.html#get-/docu/search)

### 모든 폴더 찾기

모두 찾기 **문서 폴더(DOCFDR)** 문서 공급자 연결 **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API 문서: (문서 폴더 엔드포인트는 현재 developer.workfront.com에서 다루지 않음)

### 문서 연결

링크 **문서(DOCU)** 변환 전: **외부 문서 공급자** 의 **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>문서가 일시적으로 저장됩니다. 즉, 문서의 모든 버전에 액세스할 수 있습니다. 링크를 만들 때 기존 문서 ID를 지정할 수 있으므로 데이터를 새 공급자에서 외부에서 호스팅하면서 해당 문서에 새 버전을 작성하는 것입니다. 이 문서 ID는 바꾸려는 문서 링크에 있는 문서 ID와 동일합니다. 그것은 같은 개념적 문서입니다. 이 새 버전의 바이트가 다른 공급자와 함께 저장된다는 의미일 뿐입니다.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API 문서: (현재 developer.workfront.com에서 다루지 않은 내부 링크 엔드포인트)

### 폴더 연결

링크 **문서 폴더(DOCFDR)** 변환 전: **외부 문서 공급자** 의 **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>폴더 링크 의 경우, 문서 링크와 달리 새 링크를 삽입할 Workfront 폴더의 &#39;documentFolderId&#39;가 필요합니다. 이는 복사 중인 연결된 폴더와 동일한 상위 폴더일 수 있습니다.

>[!CAUTION]
>
>폴더는 일시적으로 저장되지 않습니다. 이전 폴더를 삭제하지 마십시오. 설정 영역에서 사용자 지정 문서 통합을 비활성화하여 이전 폴더를 제거합니다.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API 문서: (현재 developer.workfront.com에서 다루지 않은 내부 링크 엔드포인트)

## 중요한 용어

* **문서**: Workfront 내의 디지털 자산

* **문서 폴더**: Workfront 내의 디지털 자산에 대한 컨테이너입니다

* **문서 ID**: 디지털 자산에 대한 Workfront 내부 ID

* **문서 폴더 ID**: 디지털 자산 폴더에 대한 Workfront 내부 ID

* **문서 공급자 ID**: 특정 문서 공급자와 연결된 ID

>[!IMPORTANT]
>
> 지정된 문서 공급자 유형에 대해 고객은 여러 개의 연결된 인스턴스를 가질 수 있습니다. 여기에는 여러 AEM 리포지토리가 연결되어 있을 수 있습니다. 또는 여러 Google 드라이브 인스턴스가 연결되어 있습니다. 문서 공급자 ID는 바꾸거나 전환할 연결 유형의 특정 인스턴스를 나타냅니다.

* **문서 저장소 공급자 유형(&quot;외부 통합 유형&quot;)**: Workfront에서 지원하는 문서 저장소 공급자 통합 유형입니다. 전용 통합 또는 &quot;사용자 지정 통합&quot;을 통해 사용할 수 있습니다.

* **현재 문서 저장소 공급자 유형( providerType)**:

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

* **링크된 문서**: 외부 문서 저장소 공급자에서 호스팅되는 디지털 자산입니다. Workfront에는 자산에 대한 자체 내부 &quot;문서 ID&quot;가 있지만, 바이트는 외부에서 저장됩니다. 이를 위해 Workfront에서는 &quot;외부 문서 ID&quot;도 저장하여 원격 저장소 또는 저장소 내에서 외부에서 참조되는 리소스를 찾는 데 도움이 됩니다.

* **링크된 문서 폴더**: 외부 문서 저장소 공급자에서 호스팅되는 디지털 자산에 대한 컨테이너입니다. Workfront에는 자산에 대한 자체 내부 &quot;문서 폴더 ID&quot;가 있지만 바이트는 외부에 저장됩니다. 이를 위해 Workfront에서는 &quot;외부 문서 ID&quot;도 저장하여 원격 저장소 또는 저장소 내에서 외부에서 참조되는 리소스를 찾는 데 도움이 됩니다.

* **외부 문서 ID**: 자산이 workfront 외부에 저장될 때 지정된 ID입니다. Workfront은 이 &quot;외부 문서 식별자&quot; 필드를 통해 내부 식별자를 외부 시스템에서 자산을 찾는 데 사용되는 식별자에 매핑합니다. 따라서 새 외부 저장소에서 문서나 폴더를 연결할 때 새 외부 문서 식별자를 외부 문서 공급자가 새 리포지토리 또는 저장소에서 문서를 식별하도록 적절한 형식으로 작성해야 합니다.

   >[!NOTE]
   >
   > Workfront에는 아직 외부 문서 식별자에 대한 표준이 없습니다. AEM ID에 새 사양을 사용하고 있지만 다른 ID의 경우 외부 문서 ID는 공급자 유형에 따라 다른 양식을 사용할 수 있습니다.


* **개체 유형**: 이 문서의 목적에 대한 API 전용 용어입니다. Workfront에서 사용할 수 있는 일반적인 객체 유형입니다. 이 경우 각각 &quot;DOCU&quot; 및 &quot;DOCFDR&quot; 유형을 갖는 문서 및 폴더와 상호 작용합니다.

* **개체 ID**: 상호 작용할 일반 개체의 내부 Workfront 식별자입니다. 문서 및 폴더와 상호 작용하므로 문서 ID 또는 문서 폴더 ID가 됩니다.
