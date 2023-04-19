---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager 자산 통합
description: 다음 Adobe Experience Manager Assets 통합으로 작업을 연결할 수 있습니다.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: b874cb1a99840db11d6d55c86b7f779aa3e6ef35
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---

# 구성 [!UICONTROL Experience Manager Assets as a Cloud Service] 통합

에서 작업을 콘텐츠와 연결할 수 있습니다. [!DNL Experience Manager Assets]&#x200B;:

* 에서 자산 및 메타데이터 푸시 [!DNL Adobe Workfront] to [!DNL Experience Manager Assets]&#x200B;
* 다음에서 자산 연결 [!DNL Experience Manager Assets] 의 프로젝트 및 작업에 [!DNL Workfront&#x200B;]
* 버전 관리 사용 사례 용이성
* 에 연결된 폴더 만들기 [!DNL Experience Manager Assets]
* 자산 및 폴더에 대한 메타데이터 추적
* 프로젝트 메타데이터 간 동기화 [!DNL Workfront] 및 [!DNL Experience Manager Assets]

여러 Experience Manager Assets 저장소를 하나의 Workfront 환경에 연결하거나 여러 Workfront 환경을 조직 ID에서 하나의 Experience Manager Assets 저장소에 연결할 수도 있습니다. 설정할 각 통합에 대해 이 문서의 구성 지침을 따르십시오.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 플랜*</strong>
   </td>
   <td>모든
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 라이센스*</strong>
   </td>
   <td>[!UICONTROL 계획]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] 라이선스</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>제품</strong>
   </td>
   <td>다음을 수행해야 합니다. [!DNL Experience Manager Assets as a Cloud Service], 및에 사용자로 제품에 추가해야 합니다.
   </td>
  </tr>
  <tr>
   <td>액세스 수준 구성*
   </td>
   <td>넌 [!DNL Workfront] 관리자 에 대한 자세한 정보 [!DNL Workfront] 관리자 <strong>사용자에게 전체 관리자 액세스 권한 부여</strong>.
   </td>
  </tr>
</table>


*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.


## 전제 조건

시작하기 전에

* 다음을 수행해야 합니다. [!DNL Workfront] 및 [!DNL Adobe Experience Manager Assets] 을 조직 ID와 연결된 경우 [!DNL Adobe Admin Consol]e. 자세한 내용은 다음을 참조하십시오. [플랫폼 기반의 관리 차이점 ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## 통합 정보 설정

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** Adobe Workfront의 오른쪽 위 모서리에 있는 아이콘을 클릭한 다음 **[!UICONTROL 설정]** .
1. 선택 **[!UICONTROL 문서]** 왼쪽 패널에서 를 선택하고 **[!UICONTROL [!DNL Experience Manager]통합]**.
   >[!NOTE]
   >
   >이 구성 영역은 [!DNL Workfront] 환경은 [!DNL Adobe Admin Console].

1. 선택 **[!UICONTROL 추가 [!DNL Experience Manager] 통합]**.
1. 에서 **[!UICONTROL 이름]** 필드에서 Workfront 및 Experience Manager Assets에서 이 통합과 상호 작용할 때 사용자가 볼 이름을 입력합니다.
1. 에서 **[!UICONTROL 탐색 URL]** 필드를 입력하면 시스템이 자동으로 탐색 URL을 채웁니다. 이 읽기 전용 URL은 조직의 [!DNL Experience Manager] 인스턴스 [!UICONTROL 기본 메뉴] 을 참조하십시오.
1. 저장소에서 저장소 선택 **[!UICONTROL [!DNL Experience Manager]자산 저장소]** 드롭다운 메뉴 시스템이 자동으로 모든 항목을 채웁니다 [!DNL Experience Manager] 사용자 프로필이 할당된 조직 ID와 연결된 저장소입니다.
   ![experience manager 저장소 선택](assets/setup-information.png)

1. 클릭 **[!UICONTROL 저장]** 또는 다음 위치로 이동 [메타데이터 설정(선택 사항)](#set-up-metadata-optional) 섹션에 자세히 설명되어 있습니다.

   >[!NOTE]
   >
   >통합의 복잡성으로 인해 초기 구성을 저장한 후에는 리포지토리를 변경할 수 없습니다.

## 메타데이터 설정(선택 사항)

매핑할 수 있습니다 [!DNL Workfront] 의 자산 미디어 필드에 대한 개체 데이터 [!DNL Experience Manager] 자산.

>[!IMPORTANT]
>
>메타데이터는 한 방향으로만 매핑할 수 있습니다. 변환 전: [!DNL Workfront] to [!DNL Experience Manager]. 에 연결된 문서의 메타데이터 [!DNL Workfront] 변환 전: [!DNL Experience Manager] 로 전송할 수 없음 [!DNL Workfront].



### 메타데이터 필드 구성

1. 에서 메타데이터 스키마 구성 [!DNL Experience Manager Assets] 에 설명된 대로 [Adobe 간 자산 메타데이터 매핑 구성 [!DNL Workfront] 및 [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
1. Workfront에서 사용자 지정 양식 필드를 구성합니다. [!DNL Workfront] 에는 사용할 수 있는 기본 제공 사용자 지정 필드가 많이 있습니다. 그러나 다음에 설명된 대로 사용자 지정 필드를 직접 만들 수도 있습니다. [사용자 지정 양식 만들기 또는 편집](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### 자산

자산이 푸시될 때 메타데이터가 매핑됩니다 [!DNL Workfront] 처음으로 기본 제공 또는 사용자 지정 필드가 있는 문서는 자산을 처음 보낼 때 지정된 필드에 자동으로 매핑됩니다 [!DNL Experience Manager Assets].

>[!NOTE]
>
>이 통합은 의 사용자 지정 메타데이터를 지원하지 않습니다. [!DNL Adobe Experience Manager].

자산에 대한 메타데이터를 매핑하려면,

1. 선택 **[!UICONTROL 자산]** 메타데이터 테이블 위에 있습니다.
1. 에서 **[!UICONTROL [!DNL Workfront]필드]** 열에서 내장 또는 사용자 지정 Workfront 필드를 선택합니다.

   >[!NOTE]
   >
   >단일 [!DNL Workfront] 여러 필드 [!UICONTROL Experience Manager Assets] 필드. 여러 개를 매핑할 수 없습니다 [!DNL Workfront] 필드를 단일 [!DNL Experience Manager Assets] 필드.

1. 에서 [!DNL Experience Manager Assets] 필드, 미리 채워진 카테고리를 검색하거나 검색 필드에 적어도 두 문자를 입력하여 추가 카테고리에 액세스합니다.
1. 필요에 따라 2단계와 3단계를 반복합니다.
   ![메타데이터 필드](assets/asset-metadata.png)
1. 클릭 [!UICONTROL 저장] 또는 다음 위치로 이동 [폴더](#folders) 섹션에 자세히 설명되어 있습니다.

### 폴더

사용자가 프로젝트에 연결된 폴더를 만들면 연결된 프로젝트, 포트폴리오 및 프로그램 데이터가 의 폴더 메타데이터 필드에 매핑됩니다 [!DNL Experience Manager Assets].

>[!NOTE]
>
>이 통합은 의 사용자 지정 메타데이터를 지원하지 않습니다. [!DNL Adobe Experience Manager].

폴더에 대한 메타데이터를 매핑하려면 다음을 수행합니다.

1. 선택 **[!UICONTROL 폴더]** 메타데이터 테이블 위에 있습니다.
1. 에서 **[!UICONTROL [!DNL Workfront]필드]** 열에서 내장 또는 사용자 지정 Workfront 필드를 선택합니다.

   >[!NOTE]
   >
   >단일 Workfront 필드를 여러 Experience Manager Assets 필드에 매핑할 수 있습니다. 여러 개를 매핑할 수 없습니다 [!DNL Workfront] 필드를 단일 [!DNL Experience Manager Assets] 필드.

1. 에서 **[!DNL Experience Manager Assets]** 필드, 미리 채워진 카테고리를 검색하거나 검색 필드에 적어도 두 문자를 입력하여 추가 카테고리에 액세스합니다.
1. 필요에 따라 2단계와 3단계를 반복합니다.
   ![폴더 메타데이터](assets/folder-metadata.png)
1. 클릭 **[!UICONTROL 저장]** 또는 다음 위치로 이동 [프로젝트 메타데이터 동기화](#project-metadata-sync) 섹션에 자세히 설명되어 있습니다.


### 개체 메타데이터 동기화

An [!DNL Experience Manager] 매핑된 필드 [!DNL Workfront] 포트폴리오, 프로그램, 프로젝트, 작업, 문제 및 문서 필드는 [!DNL Workfront].

>[!IMPORTANT]
>
>사용자는에 쓰기 액세스 권한이 있어야 합니다. [!DNL Experience Manager] 업데이트될 때 메타데이터를 동기화하기 위해 객체에 있는 자산의 경우.

1. 를 활성화합니다 **[!UICONTROL 개체 메타데이터 동기화]** 필드.
1. 저장 을 클릭하거나 [연결된 폴더 설정(선택 사항)](#set-up-linked-folders-optional) 섹션에 자세히 설명되어 있습니다.

## 연결된 폴더 설정(선택 사항)

사용자가 연결된 폴더를 만들 수 있도록 허용할 수 있습니다 [!DNL Experience Manager] 잠시 [!DNL Workfront] 프로젝트. 폴더가 연결되면 폴더에 추가된 모든 자산이 자동으로 두 폴더에 표시됩니다 [!DNL Workfront] 및 [!DNL Experience Manager]. 자산이 의 연결된 폴더에 추가되는 경우 [!DNL Workfront] 처음으로 자산의 메타데이터가 [!DNL Experience Manager Assets].

아래 단계에서는 연결된 폴더를 만들 위치를 나타냅니다. 각 통합에는 연결된 모든 폴더에 대해 하나의 위치만 있을 수 있습니다.

연결된 폴더를 설정하려면 다음을 수행하십시오.

1. 전환 **[!UICONTROL 연결된 폴더 활성화]** 설정
1. 이 통합과 관련된 모든 연결된 폴더를 표시할 폴더 경로를 선택합니다.

   >[!NOTE]
   >
   >사용자는 쓰기 액세스 권한이 필요합니다. [!DNL Adobe Experience Manager Assets] 연결된 폴더를 만들기 위해 지정된 폴더로 이동합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
