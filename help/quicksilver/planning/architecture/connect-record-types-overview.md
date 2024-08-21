---
title: 연결된 레코드 유형 개요
description: 개별 레코드 종류가 서로 관련되는 방식을 나타내는 방법은 해당 레코드 종류를 연결하는 것입니다. 또한 Adobe Workfront Planning 레코드 유형을 다른 애플리케이션의 객체 유형과 연결하여 사용자 경험을 향상시키고 한 애플리케이션에서 집중할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# 연결된 레코드 유형 개요

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

개별 레코드 유형을 연결하여 서로 관련되거나 다른 응용 프로그램의 오브젝트와 관련됨을 나타낼 수 있습니다.

이 문서에서는 레코드 유형 연결에 대한 개요를 살펴보고 레코드와 개체 유형 간에 설정할 수 있는 연결 유형에 대해 설명합니다.

레코드 종류를 연결하는 방법에 대한 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

## 레코드 유형 연결에 대한 고려 사항

Workfront Planning에서 연결하는 단계는 두 가지가 있습니다.

1. 먼저 다른 응용 프로그램에서 두 레코드 형식 또는 레코드 형식과 개체 형식 간에 연결을 설정해야 합니다. 레코드 종류를 연결하는 방법에 대한 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.
1. 두 번째, 두 레코드 유형이 연결된 후 한 유형의 개별 레코드와 다른 유형의 레코드를 연결할 수 있습니다. 레코드 연결에 대한 자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하십시오.

레코드 유형 연결에 대해 다음 사항을 고려하십시오.

* Adobe Workfront Planning에서 다음 엔티티를 연결할 수 있습니다.

   * 두 가지 레코드 유형.

     기본적으로 동일한 작업 영역에서 두 개의 레코드 유형을 연결할 수 있습니다. 다른 작업 영역의 레코드 유형과 연결할 레코드 유형을 설정할 수도 있습니다. 자세한 내용은 [레코드 종류 편집](/help/quicksilver/planning/architecture/edit-record-types.md)을 참조하세요.
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

* 연결된 레코드 유형에 대한 레코드를 만든 후 연결된 레코드 필드를 통해 서로 연결할 수 있습니다.  자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

* 레코드 유형을 다른 레코드 유형이나 다른 응용 프로그램의 개체 유형과 연결한 후에는 다음과 같은 시나리오가 있습니다.

   * **두 Planning 레코드 형식을 연결할 때**: 연결 중인 레코드 형식에 연결된 레코드 필드가 만들어집니다. 연결하는 레코드 종류에 유사한 연결된 레코드 필드가 만들어집니다.

     예를 들어 &quot;Campaign&quot; 레코드 유형을 &quot;Product&quot; 레코드 유형과 연결하는 경우 이름을 &quot;Linked Product&quot;로 지정한 연결된 레코드 필드(연결 필드)가 캠페인 레코드 유형에 만들어집니다. 제품 레코드 유형에 자동으로 &quot;캠페인&quot;이라는 연결된 레코드 유형이 만들어집니다.

   * **다른 응용 프로그램의 개체 형식과 레코드 형식을 연결하는 경우**:

      * 연결하는 레코드 종류에 연결된 레코드 필드가 만들어집니다. 연결된 레코드 필드는 다른 응용 프로그램의 개체 유형에 자동으로 만들어지지 않습니다.
      * Workfront 오브젝트에서 Planning 레코드 필드에 액세스할 수 없습니다.
      * Workfront 관리자가 Workfront과 Adobe Experience Manager Assets 간의 통합을 통해 메타데이터 매핑을 구성할 때 Experience Manager 에셋에서 계획 레코드 필드에 액세스할 수 있습니다. 자세한 내용은 [Adobe Workfront과 Experience Manager Assets 간의 에셋 메타데이터 매핑 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)을 참조하십시오.
      * 계획 레코드는 Workfront 오브젝트의 계획 탭에서 볼 수 있습니다. 자세한 내용은 [Adobe Workfront 개체의 계획 섹션에서 레코드 관리](/help/quicksilver/planning/records/manage-records-in-planning-section.md)를 참조하십시오.

   * **연결된 레코드 또는 개체에서 조회 필드를 추가할 때**: 연결된 레코드 필드를 만들 수 있을 뿐만 아니라 연결된 레코드 또는 개체 형식의 필드에 연결할 수도 있습니다. 이 필드를 조회 필드라고 합니다. 연결하려는 레코드의 정보가 있는 연결된(또는 조회 필드) 필드는 연결하려는 레코드에 표시됩니다.

     다른 레코드 유형이나 다른 응용 프로그램 객체의 필드를 Workfront Planning 레코드 유형에 연결할 수 있습니다.

     연결된 필드는 읽기 전용이며 연결된 레코드의 정보를 자동으로 표시합니다.

     수식, 필터 또는 그룹화에서 다른 레코드 또는 개체 형식의 조회 필드를 참조할 수 있습니다.

     예를 들어 &quot;캠페인&quot; 레코드 유형을 Workfront 프로젝트와 연결하고 프로젝트의 계획된 완료 일자 필드를 Workfront 계획 레코드로 가져오도록 선택하면 캠페인에 대해 연결된 필드(프로젝트의 계획된 완료 일자)가 자동으로 생성됩니다. 연결된 이 필드는 수동으로 편집할 수 없습니다. 계획된 완료 일자(프로젝트 시작) 필드에는 연결된 프로젝트의 계획된 완료 일자가 표시됩니다.

     >[!IMPORTANT]
     >
     >작업 영역에 대한 보기 이상의 권한이 있는 모든 사용자는 링크된 객체 유형의 응용 프로그램에서 자신의 권한 또는 액세스 수준이나 다른 작업 영역에서 본인의 권한에 관계없이 조회 필드에서 정보를 볼 수 있습니다.

     연결된 레코드 필드 앞에는 관계 아이콘 ![](assets/relationship-field-icon.png)이(가) 있습니다.

     연결된 필드 앞에는 필드 유형을 식별하는 아이콘이 표시됩니다. 예를 들어 연결된(또는 조회) 필드 앞에는 필드가 숫자, 단락 또는 날짜임을 나타내는 아이콘이 표시됩니다.

<!--## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

Depending on how many records you can add to a connected record field, the following are the connection types you can choose from when connecting record types: 

* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)

>[!WARNING]
>
>These options are not available when connecting the following: 
>* Two records from different workspaces
>
>* A record type and Experience Manager assets

### Many-to-many connection type

![](assets/many-to-many-connection-picker.png)

When you create a many-to-many connection between record types, you can then select multiple records in the connection field from both record types. 

For example, if you create a many-to-many connection between campaigns and projects, you can select multiple projects for each campaign, and multiple campaigns for each project. 

A real-life example of a many-to-many relationship type is the relationship between movies and actors. Each movie can have multiple actors, and each actor can play in multiple movies. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![](assets/one-to-many-connection-picker.png)


When you create a one-to-many connection between record types, you can then select multiple records in the connection field in the current record type, but the corresponding connection field in the record type you connect to will allow selecting only one record. The connected record field that is automatically created on the second record type is automatically set to a many-to-one relationship type. 

For example, if you create a one-to-many connection between campaigns and projects, you can select multiple projects for each campaign, but each project can be connected to only one campaign.

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 

### Many-to-one connection type

![](assets/many-to-one-connection-picker.png)


When you create a many-to-one connection between record types, you can then connect each record in the current record type with only one record from the connected record type. The connected record field that is automatically created on the second record type is automatically set to a one-to-many relationship type. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![](assets/one-to-one-connection-picker.png)

When you create a one-to-one connection between record types, in both record types you can connect each record only with one record from the other record type.

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type. 

-->



