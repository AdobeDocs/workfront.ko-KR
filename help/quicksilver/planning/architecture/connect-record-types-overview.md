---
title: 레코드 유형 연결 개요
description: 개별 레코드 종류가 서로 관련되는 방식을 나타내는 방법은 해당 레코드 종류를 연결하는 것입니다. 또한 Adobe Workfront Planning 레코드 유형을 다른 애플리케이션의 객체 유형과 연결하여 사용자 경험을 향상시키고 한 애플리케이션에서 집중할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# 레코드 유형 연결 개요

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

개별 레코드 유형을 연결하여 서로 관련되거나 다른 응용 프로그램의 오브젝트와 관련됨을 나타낼 수 있습니다.

이 문서에서는 레코드 형식이 연결되는 방법에 대한 개요를 살펴보고 레코드와 개체 형식 간에 설정할 수 있는 연결 형식을 설명합니다.

레코드 종류를 연결하는 방법에 대한 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

## 레코드 유형 연결에 대한 고려 사항

* Adobe Workfront Planning에서 다음 엔티티를 연결할 수 있습니다.

   * 두 가지 레코드 유형

     레코드 유형은 동일한 작업 영역에 속해야 합니다.
   * 다른 응용 프로그램의 레코드 형식과 개체 형식입니다.

* 다음 응용 프로그램에서 Workfront Planning 레코드 유형과 다음 객체 유형을 연결할 수 있습니다.

   * Adobe Workfront:

      * 프로젝트
      * 포트폴리오
      * 프로그램
      * 회사
      * 그룹

   * Adobe Experience Manager Assets:

      * 이미지
      * 폴더

     >[!IMPORTANT]
     >
     >Adobe Experience Manager Assets 라이선스가 있어야 하며 Workfront Planning 레코드를 Adobe Experience Manager Assets에 연결하려면 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.
     >
     >Adobe Admin Console 온보딩에 대한 질문이 있는 경우 [통합 경험 Adobe FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md)를 참조하십시오.

* 레코드 유형에 대한 개별 레코드를 만든 후 연결된 레코드 유형 필드에서 연결하는 레코드를 선택할 수 있습니다. 자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

* 레코드 유형을 다른 레코드 유형이나 다른 응용 프로그램의 개체 유형과 연결한 후에는 다음과 같은 시나리오가 있습니다.

   * **두 레코드 형식을 연결할 때**: 연결 중인 레코드 형식에 연결된 레코드 필드가 만들어집니다. 연결하는 레코드 종류에 유사한 연결된 레코드 필드가 만들어집니다.

     예를 들어 &quot;Campaign&quot; 레코드 유형을 &quot;Product&quot; 레코드 유형과 연결하는 경우 이름을 &quot;Linked Product&quot;로 지정한 연결된 레코드 필드가 캠페인 레코드 유형에 만들어집니다. 제품 레코드 유형에 자동으로 &quot;캠페인&quot;이라는 연결된 레코드 유형이 만들어집니다.

   * **다른 응용 프로그램의 개체 형식과 레코드 형식을 연결하는 경우**:

      * 연결하는 레코드 종류에 연결된 레코드 필드가 만들어집니다. 연결된 레코드 필드는 다른 응용 프로그램의 개체 유형에 자동으로 만들어지지 않습니다.

      * Workfront 오브젝트에서 Planning 레코드 필드에 액세스할 수 없습니다.
      * Workfront 관리자가 Workfront과 Adobe Experience Manager Assets 간의 통합을 통해 메타데이터 매핑을 구성할 때 Experience Manager 에셋에서 계획 레코드 필드에 액세스할 수 있습니다. 자세한 내용은 [Adobe Workfront과 Experience Manager Assets 간의 에셋 메타데이터 매핑 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)을 참조하십시오.

   * **연결된 레코드 또는 개체에서 연결된(또는 조회) 필드를 추가할 때**: 연결 중인 레코드의 정보가 있는 연결된(또는 조회 필드)가 연결 중인 레코드에 표시됩니다.

     다른 레코드 유형이나 다른 응용 프로그램 객체의 필드를 Workfront Planning 레코드 유형에 연결할 수 있습니다.

     연결된 필드는 읽기 전용이며 레코드나 개체를 연결할 때 연결된 레코드나 개체의 정보를 자동으로 표시합니다.

     예를 들어 &quot;캠페인&quot; 레코드 유형을 Workfront 프로젝트와 연결하고 프로젝트의 계획된 완료 일자 필드를 Workfront 계획 레코드로 가져오도록 선택하면 캠페인에 대해 연결된 필드(프로젝트의 계획된 완료 일자)가 자동으로 생성됩니다. 연결된 이 필드는 수동으로 편집할 수 없습니다. 계획된 완료 일자(프로젝트 시작) 필드에는 연결된 프로젝트의 계획된 완료 일자가 표시됩니다.

     >[!IMPORTANT]
     >
     >작업 영역에 대한 보기 이상의 권한이 있는 모든 사용자는 연결된 객체 유형의 응용 프로그램에서 자신의 권한 또는 액세스 수준에 관계없이 연결된 필드에서 정보를 볼 수 있습니다.

* 연결된 레코드 필드 앞에는 관계 아이콘 ![](assets/relationship-field-icon.png)이(가) 있습니다.

  연결된 필드 앞에는 필드 유형을 식별하는 아이콘이 표시됩니다. 예를 들어 연결된(또는 조회) 필드 앞에는 필드가 숫자, 단락 또는 날짜임을 나타내는 아이콘이 표시됩니다.

* 조회 필드 앞에는 필드에 표시되는 정보 유형을 나타내는 아이콘이 표시됩니다.

## 연결 유형

두 레코드 유형 간에 또는 다른 응용 프로그램의 레코드와 개체 유형 간에 연결을 설정한 후 연결된 레코드 필드에 레코드를 추가할 수 있습니다.

연결에 추가할 수 있는 레코드 수에 따라 레코드 유형을 연결할 때 선택할 수 있는 연결 유형은 다음과 같습니다.

* [일대다](#one-to-many-connection-type)
* [일대일](#many-to-one-connection-type)
* [다대일](#many-to-one-connection-type)
* [다대다](#many-to-many-connection-type)

<!-- add screen shots for each type of connection below-->

### 일대다 연결 유형

레코드 유형 간에 일대다 연결 유형을 선택하면 나중에 연결하려는 여러 레코드가 있는 하나의 레코드를 연결할 수 있습니다.

예를 들어 캠페인을 프로젝트와 연결하는 경우 하나의 캠페인을 여러 프로젝트와 연결할 수 있습니다. 그러나 하나의 프로젝트는 하나의 캠페인에만 연결될 수 있습니다.

이 연결 유형을 선택하면 나중에 다대다 연결 유형으로만 변경할 수 있습니다.

### 일대일 연결 유형

레코드 종류 간에 일대일 연결 유형을 선택하면 나중에 하나의 레코드를 연결하려는 다른 레코드와 연결할 수 있습니다.

예를 들어 캠페인을 프로젝트와 연결하는 경우 하나의 캠페인과 하나의 프로젝트를 연결할 수 있습니다. 하나의 프로젝트는 하나의 캠페인에만 연결할 수 있습니다.

이 연결 유형을 선택하면 나중에 다른 연결 유형으로 변경할 수 있습니다.

### 다대일 연결 유형

레코드 유형 간에 다대일 연결 유형을 선택하면 나중에 연결 중인 레코드 하나만 있는 여러 레코드를 연결할 수 있습니다.

예를 들어 캠페인을 프로젝트와 연결하는 경우 여러 캠페인을 하나의 프로젝트와 연결할 수 있습니다. 하나의 프로젝트를 여러 캠페인에 연결할 수 있습니다.

이 연결 유형을 선택하면 나중에 다대다 연결 유형으로만 변경할 수 있습니다.

### 다대다 연결 유형

레코드 유형 간에 다대다 연결 유형을 선택하면 나중에 연결 중인 여러 레코드가 있는 여러 레코드를 연결할 수 있습니다.

예를 들어 캠페인을 프로젝트와 연결하는 경우 여러 캠페인을 여러 프로젝트와 연결할 수 있습니다. 여러 프로젝트를 여러 캠페인에 연결할 수도 있습니다.

이 연결 유형을 선택하면 저장한 후 연결 유형을 변경할 수 없습니다.