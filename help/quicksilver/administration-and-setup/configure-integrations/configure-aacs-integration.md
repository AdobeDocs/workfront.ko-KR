---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: '[!UICONTROL Experience Manager Assets as a Cloud Service] 통합 구성'
description: ' [!DNL Experience Manager Assets]에서 작업을 콘텐츠와 연결할 수 있습니다.'
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1708'
ht-degree: 0%

---

# [!UICONTROL Experience Manager Assets as a Cloud Service] 통합 구성

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>이 기능은 [!DNL Adobe Admin Console]에 온보딩된 조직에서만 사용할 수 있습니다.

[!DNL Experience Manager Assets]의 콘텐츠와 작업을 연결할 수 있습니다&#x200B;.

* 자산 및 메타데이터를 [!DNL Adobe Workfront]에서 [!DNL Experience Manager Assets]&#x200B;(으)로 &#x200B; 푸시
* [!DNL Experience Manager Assets]의 자산을 [!DNL Workfront&#x200B;]의 프로젝트 및 작업에 연결
* 버전 관리 사용 사례 촉진
* [!DNL Experience Manager Assets]에 연결된 폴더 만들기
* 에셋 및 폴더에 대한 메타데이터 추적
* [!DNL Workfront]과(와) [!DNL Experience Manager Assets] 간 프로젝트 메타데이터 동기화

>[!NOTE]
>
>조직 ID를 통해 여러 [!DNL Experience Manager Assets] 저장소를 하나의 [!UICONTROL Workfront] 환경에 연결하거나 여러 [!DNL Workfront] 환경을 하나의 [!DNL Experience Manager Assets] 저장소에 연결할 수도 있습니다. 설정하려는 각 통합에 대해 이 문서의 구성 지침을 따르십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table>
  <tr>
   <td>[!DNL Adobe Workfront] 플랜
   </td>
   <td>임의
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] 라이센스
   </td>
   <td><p>현재: [!UICONTROL Plan]</p>
   <p>새로운 기능: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] 라이센스
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>제품
   </td>
   <td>[!DNL Experience Manager Assets as a Cloud Service]이(가) 있어야 하며 제품에 사용자로 추가되어야 합니다.
   </td>
  </tr>
  <tr>
   <td>액세스 수준 구성
   </td>
   <td>[!DNL Workfront] 관리자여야 합니다.
   </td>
  </tr>
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에,

* [!DNL Workfront]에서 조직 ID와 연결된 [!DNL Adobe Experience Manager Assets] 및 [!DNL Adobe Admin Console]이(가) 있어야 합니다. 자세한 내용은 [플랫폼 기반 관리 차이점([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하세요.


## 통합 정보 설정

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 문서]**&#x200B;를 선택한 다음 **[!UICONTROL [!DNL Experience Manager]통합]**&#x200B;을 선택합니다.

   >[!NOTE]
   >
   >이 구성 영역은 [!DNL Workfront] 환경이 [!DNL Adobe Admin Console] 아래에 포함된 경우에만 나타납니다.

1. **[!UICONTROL [!DNL Experience Manager] 통합 추가]**&#x200B;를 선택합니다.
1. Workfront 및 Experience Manager Assets에서 이 통합과 상호 작용할 때 사용자가 볼 이름을 **[!UICONTROL 이름]** 필드에 입력하십시오.
1. **[!UICONTROL 탐색 URL]** 필드에서 탐색 URL이 자동으로 채워집니다. 이 읽기 전용 URL은 빠른 액세스를 위해 [!DNL Experience Manager]기본 메뉴[!UICONTROL 에서 조직의 &#x200B;] 인스턴스에 연결하는 데 사용됩니다.
1. **[!UICONTROL [!DNL Experience Manager]Assets 저장소]** 드롭다운 메뉴에서 저장소를 선택합니다. 사용자 프로필이 할당된 조직 ID와 연결된 [!DNL Experience Manager] 저장소가 자동으로 채워집니다.
   ![experience manager 저장소 선택](assets/setup-information.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭하거나 이 문서의 [메타데이터 설정(선택 사항)](#set-up-metadata-optional) 섹션으로 이동하십시오.

   >[!NOTE]
   >
   >통합의 복잡성으로 인해 초기 구성을 저장한 후에는 저장소를 변경할 수 없습니다.

## 메타데이터 설정(선택 사항)

[!DNL Workfront] 개체 데이터를 [!DNL Experience Manager] Assets의 에셋 미디어 필드에 매핑할 수 있습니다.

>[!IMPORTANT]
>
>메타데이터는 [!DNL Workfront]에서 [!DNL Experience Manager] 방향으로만 매핑할 수 있습니다. [!DNL Workfront]에서 [!DNL Experience Manager]에 연결된 문서의 메타데이터를 [!DNL Workfront]&#x200B;(으)로 전송할 수 없습니다.

### 메타데이터 필드 구성

메타데이터 필드 매핑을 시작하기 전에 Workfront 및 Experience Manager Assets 모두에서 메타데이터 필드를 구성해야 합니다.

메타데이터 필드를 구성하려면:

1. [!DNL Experience Manager Assets]Adobe과(와) [ [!DNL Workfront]  간의 에셋 메타데이터 매핑 구성 [!DNL Experience Manager Assets]에 설명된 대로 ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping)에서 메타데이터 스키마를 구성합니다.


1. Workfront에서 사용자 정의 양식 필드를 구성합니다. [!DNL Workfront]에 사용할 수 있는 기본 제공 사용자 지정 필드가 많습니다. 그러나 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)에 설명된 대로 사용자 정의 필드를 만들 수도 있습니다.

+++ **지원되는 Workfront 및 Experience Manager Assets 필드에 대한 자세한 내용을 보려면 확장** 

**Experience Manager Assets 태그**

Workfront 지원 필드를 Experience Manager Assets의 태그에 매핑할 수 있습니다. 이렇게 하려면 Experience Manager Assets의 태그 값이 Workfront과 일치하는지 확인해야 합니다.

* 태그와 Workfront 필드 값은 맞춤법 및 형식에서 정확히 일치해야 합니다.
* experience Manager assets 태그에 매핑된 Workfront 필드 값은 Experience Manager Assets의 태그가 대문자로 표시되더라도 모두 소문자여야 합니다.
* Workfront 필드 값에는 공백이 없어야 합니다.
* Workfront의 필드 값에는 Experience Manager Assets 태그의 폴더 구조도 포함되어야 합니다.
* 여러 한 줄 텍스트 필드를 태그에 매핑하려면 메타데이터 매핑의 Workfront 쪽에 쉼표로 구분된 태그 값 목록을 입력하고 Experience Manager Assets 쪽에 `xcm:keywords`을(를) 입력하십시오. 각 필드 값은 별도의 태그에 매핑됩니다. 계산된 필드를 사용하여 여러 Workfront 필드를 쉼표로 구분된 단일 텍스트 필드로 결합할 수 있습니다.
* 해당 필드에 사용 가능한 값의 쉼표로 구분된 목록을 입력하여 드롭다운, 라디오 버튼 또는 확인란 필드의 값을 매핑할 수 있습니다.


>[!INFO]
>
>**예**: 여기에서 폴더 구조에 표시된 태그를 일치시키려면 Workfront의 필드 값은 `landscapes:trees/spruce`이(가) 됩니다. Workfront 필드 값에서 소문자를 확인합니다.
>
>태그 트리에서 태그가 맨 왼쪽 항목이 되도록 하려면 뒤에 콜론이 와야 합니다. 이 예제에서 landscape 태그에 매핑하려면 Workfront의 필드 값은 `landscapes:`입니다.
>
>![AEM의 폴더 구조](assets/aem-folder-structure-with-red-boxes.png)


Experience Manager Assets에서 태그를 만들면 메타데이터 섹션의 태그 드롭다운 아래에 태그가 표시됩니다. 필드를 태그에 연결하려면 메타데이터 매핑 영역의 Experience Manager Assets 필드 드롭다운에서 `xcm:keywords`을(를) 선택합니다.

태그를 만들고 관리하는 방법을 포함하여 Experience Manager Assets의 태그에 대한 자세한 내용은 [태그 관리](https://experienceleague.adobe.com/en/docs/experience-manager-64/administering/contentmanagement/tags)를 참조하십시오.

**Experience Manager Assets 사용자 지정 메타데이터 스키마 필드**

기본 제공 및 사용자 지정 Workfront 필드를 모두 Experience Manager Assets의 사용자 지정 메타데이터 스키마 필드에 매핑할 수 있습니다.

Experience Manager Assets에서 만든 사용자 지정 메타데이터 필드는 메타데이터 설정 영역의 자체 섹션에 구성됩니다.

![사용자 지정 메타데이터 섹션](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront 필드**

기본 제공 필드와 사용자 지정 Workfront 필드를 모두 Experience Manager Assets에 매핑할 수 있습니다. 다음 필드 값은 Workfront과 Experience Manager Assets 간에 대소문자와 맞춤법 모두에서 일치해야 합니다.

* 드롭다운 필드
* 다중 선택 필드

>[!TIP]
>
> 필드 값이 정확히 일치하는지 확인하려면
>
> * 설정 > Workfront의 사용자 지정 Forms 또는 오브젝트의 필드
> * Assets > Experience Manager Assets의 메타데이터 스키마

+++

### 에셋의 메타데이터 매핑

에셋이 [!DNL Workfront]에서 처음으로 전달될 때 메타데이터가 매핑됩니다. 기본 제공 필드 또는 사용자 지정 필드가 있는 문서는 에셋을 [!DNL Experience Manager Assets]&#x200B;(으)로 처음 보낼 때 지정된 필드에 자동으로 매핑됩니다.

에셋의 메타데이터를 매핑하려면 다음을 수행합니다.

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. **[!UICONTROL [!DNL Workfront]필드]** 열에서 기본 제공 또는 사용자 지정 Workfront 필드를 선택합니다.

   >[!NOTE]
   >
   >단일 [!DNL Workfront] 필드를 여러 [!UICONTROL Experience Manager Assets] 필드에 매핑할 수 있습니다. 여러 [!DNL Workfront] 필드를 하나의 [!DNL Experience Manager Assets] 필드에 매핑할 수 없습니다.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. [!DNL Experience Manager Assets] 필드에서 미리 채워진 범주를 검색하거나 검색 필드에 두 개 이상의 문자를 입력하여 추가 범주에 액세스합니다.
1. 필요에 따라 2단계와 3단계를 반복합니다.
   ![메타데이터 필드](assets/metadata-no-asset-toggle.png)
1. 이 문서의 [!UICONTROL 저장]을 클릭하거나 [워크플로 설정](#set-up-workflows-optional) 섹션으로 이동하십시오.

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## 워크플로우 설정(선택 사항)

워크플로는 Workfront을 Adobe Experience Manager as a Cloud Service에 연결하는 작업 세트입니다. Workfront 관리자는 Workfront에서 워크플로우를 구성한 다음 프로젝트 템플릿에 할당할 수 있습니다.

워크플로가 할당된 프로젝트 템플릿을 사용하여 프로젝트를 만들면 워크플로에 정의된 작업이 트리거됩니다.

Adobe Experience Manager 전체에 대해 워크플로우가 활성화되고 구성됩니다. 그런 다음 이러한 워크플로를 프로젝트 템플릿에 적용할 수 있습니다. 템플릿 수준 또는 해당 템플릿에서 프로젝트를 만들 때 프로젝트 수준에서 조정하거나 사용자 지정할 수 있습니다.

Adobe Experience Manager 통합에서 사용할 수 있는 워크플로는 다음과 같습니다.

* [Adobe Experience Manager 연결 폴더 만들기](#create-adobe-experience-manager-linked-folders)
* [Adobe Experience Manager Assets으로 전송된 자산 게시](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Adobe Experience Manager 연결 폴더 만들기

폴더 트리당 최대 100개의 연결된 폴더를 만들 수 있습니다.

1. **[!UICONTROL 연결된 폴더 만들기]**&#x200B;를 전환합니다.
1. 생성 중인 연결된 폴더의 이름을 입력합니다.
1. (조건부) 이 연결된 폴더가 이 통합을 사용하는 템플릿으로 만든 프로젝트의 기본 폴더가 되게 하려면 **기본 폴더 트리** 옵션을 활성화합니다. 하나 이상의 기본 폴더를 선택할 수 있습니다.
1. 폴더 경로를 선택하여 이 통합과 연결된 모든 폴더를 연결할 위치를 지정합니다.
1. (조건부) 이 통합에 폴더 트리(중첩된 폴더)를 추가하려면 다음을 수행합니다.

   1. **폴더 추가** 아이콘 ![폴더 추가](assets/add-folder-aem.png)를 클릭합니다.
   1. **이름 형식** 필드에서 폴더 이름을 지정할 방법을 선택합니다.

      * **이름**: 폴더 이름을 입력하십시오.
      * **개체 데이터**: 폴더 이름에 대한 원본(예: 프로젝트 이름)을 선택하십시오.

      >[!NOTE]
      >
      >* 폴더 이름은 100자 미만이어야 합니다.
      >* 폴더 이름에서 다음 문자가 제거됩니다.
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. 폴더 트리에 중첩된 폴더를 추가하려면 중첩된 폴더를 만들 폴더 옆에 있는 세 점 메뉴를 클릭하고 **폴더 추가**&#x200B;를 선택합니다. 이전 단계 의 설명에 따라 필드를 채웁니다.
   1. 폴더를 Workfront에 연결하려면 폴더를 선택하고 **연결된 폴더 만들기**&#x200B;를 클릭하십시오.   아이콘 ![폴더 연결](assets/link-folder.png).
   1. (선택 사항) 폴더를 편집하려면 폴더를 선택하고 **폴더 편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
   1. (선택 사항) 폴더를 삭제하려면 폴더를 선택하고 **폴더 삭제** 아이콘 ![폴더 삭제](assets/delete-folder.png)를 클릭합니다.
1. (조건부) 다른 폴더 트리를 추가하려면 **+ 폴더 트리 추가**&#x200B;를 클릭하고 5단계의 단계를 따릅니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭하거나 이 문서의 [Adobe Experience Manager Assets으로 보낸 에셋 게시](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) 섹션으로 이동하십시오.

>[!NOTE]
>
>* 이 통합은 생성된 폴더 트리의 수에 관계없이 100개 이하의 폴더를 만듭니다. 예를 들어 4개의 폴더 트리로 통합하면 400개의 폴더가 아니라 최대 100개의 폴더를 만들 수 있습니다.
>* 폴더 트리의 첫 번째 폴더는 자동으로 Workfront에 연결된 것으로 표시됩니다. 이 폴더에 연결하지 않으려면 연결을 해제할 수 있습니다.
>* 제공된 폴더 트리가 없으면 루트 폴더가 연결된 폴더가 됩니다.


### Adobe Experience Manager Assets으로 전송된 자산 게시

1. **[!UICONTROL 자산을 자동으로 게시]**&#x200B;합니다.
1. Adobe Experience Manager Assets로 전송된 자산을 게시할 위치 옆에 있는 상자를 선택합니다. 두 옵션 중 하나 또는 모두를 활성화할 수 있습니다.
1. (조건부) Brand Portal 옵션을 활성화한 경우 에셋을 게시할 Brand Portal을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭하거나 이 문서의 [연결된 폴더 설정(선택 사항)](#set-up-linked-folders-optional) 섹션으로 이동하십시오.

## 연결된 폴더 설정(선택 사항)

사용자가 [!DNL Experience Manager] 프로젝트에 있는 동안 [!DNL Workfront]에 연결된 폴더를 만들도록 허용할 수 있습니다. 폴더가 연결되면 폴더에 추가된 모든 자산이 [!DNL Workfront]과(와) [!DNL Experience Manager] 모두에 자동으로 표시됩니다. [!DNL Workfront]의 연결된 폴더에 에셋을 처음 추가하면 에셋의 메타데이터가 [!DNL Experience Manager Assets]&#x200B;(으)로 푸시됩니다.

아래 단계에서는 연결된 폴더를 만들 위치를 지정합니다. 각 통합에는 연결된 모든 폴더에 대해 하나의 위치만 있을 수 있습니다.

연결된 폴더를 설정하려면 다음을 수행하십시오.

1. **[!UICONTROL 연결된 폴더 사용]** 설정을 전환합니다.
1. 폴더 경로를 선택하여 이 통합과 연결된 모든 폴더를 연결할 위치를 지정합니다.

   >[!NOTE]
   >
   >연결된 폴더를 만들려면 [!DNL Adobe Experience Manager Assets]에서 지정한 폴더에 쓰기 액세스 권한이 필요합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
