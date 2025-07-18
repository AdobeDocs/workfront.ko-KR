---
title: 연결된 레코드 유형 개요
description: 개별 레코드 종류가 서로 관련되는 방식을 나타내는 방법은 해당 레코드 종류를 연결하는 것입니다. 또한 Adobe Workfront Planning 레코드 유형을 다른 애플리케이션의 객체 유형과 연결하여 사용자 경험을 향상시키고 한 애플리케이션에서 집중할 수 있습니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 1%

---

# 연결된 레코드 유형 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>   -->

개별 레코드 유형을 연결하여 서로 관련되거나 다른 응용 프로그램의 오브젝트와 관련됨을 나타낼 수 있습니다.

이 문서에서는 레코드 유형 연결에 대한 개요를 살펴보고 레코드와 개체 유형 간에 설정할 수 있는 연결 유형에 대해 설명합니다.

레코드 종류를 연결하는 방법에 대한 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

## 레코드 유형 연결에 대한 고려 사항

Workfront Planning에서 연결하는 단계는 두 가지가 있습니다.

1. 먼저 다른 응용 프로그램에서 두 레코드 형식 또는 레코드 형식과 개체 형식 간에 연결을 설정해야 합니다. 레코드 종류를 연결하는 방법에 대한 자세한 내용은 레코드 종류[ 연결을 참조하십시오](/help/quicksilver/planning/architecture/connect-record-types.md).
1. 둘째, 두 레코드 종류가 연결된 후 한 종류의 개별 레코드를 다른 종류의 레코드와 연결할 수 있습니다. 레코드 연결에 대한 자세한 내용은 레코드[ 연결을 참조하세요](/help/quicksilver/planning/records/connect-records.md).

레코드 종류 연결에 대해 다음 사항을 고려합니다.

* Adobe Systems Workfront Planning에서 다음 엔티티를 연결할 수 있습니다.

   * 두 가지 레코드 종류.

     기본적으로 동일한 작업 영역에서 두 개의 레코드 유형을 연결할 수 있습니다. 다른 작업 영역의 레코드 유형과 연결할 레코드 유형을 설정할 수도 있습니다. 자세한 내용은 [레코드 종류 편집](/help/quicksilver/planning/architecture/edit-record-types.md)을 참조하세요.
   * 다른 애플리케이션 레코드 형식 및 개체 형식

* Workfront Planning 레코드 유형을 다음 애플리케이션의 다음 객체 유형과 연결할 수 있습니다.

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
     >Adobe Experience Manager Assets 라이선스가 있어야 하며, Workfront Planning 레코드를 Adobe Experience Manager Assets에 연결하려면 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.
     >
     >Adobe Admin Console 온보딩에 대한 질문이 있는 경우 [Adobe 통합 경험 FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md)를 참조하십시오.

* 연결된 레코드 유형에 대한 레코드를 만든 후 연결된 레코드 필드를 통해 서로 연결할 수 있습니다.  자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

* 레코드 종류를 다른 레코드 종류나 다른 애플리케이션 개체의 개체 종류와 연결하면 다음과 같은 시나리오가 발생합니다.

   * **두 개의 Planning 레코드 종류**&#x200B;를 연결하는 경우: 연결하려는 레코드 종류에 연결된 레코드 필드가 만들어집니다. 연결하려는 레코드 종류에 유사한 연결된 레코드 필드가 만들어집니다.

     예를 들어 &quot;Campaign&quot; 레코드 종류를 &quot;Product&quot; 레코드 종류와 연결하면 &quot;Linked Product&quot;라는 이름의 연결된 레코드 필드(연결 필드)가 Campaign 레코드 종류에 만들어집니다. 자동으로 &quot;Campaign&quot;이라는 이름의 연결된 레코드 종류가 제품 레코드 종류에 만들어집니다.

   * **레코드 종류를 다른 애플리케이션** 개체 종류와 연결하는 경우:

      * 연결하려는 레코드 종류에 연결된 레코드 필드가 만들어집니다. 연결된 레코드 필드는 다른 응용 프로그램의 개체 유형에 자동으로 만들어지지 않습니다.
      * Workfront 오브젝트에서 Planning 레코드 필드에 액세스할 수 없습니다.
      * 계획 레코드는 Workfront 개체의 계획 탭 에서 볼 수 있습니다. 자세한 내용은 Workfront 객체[에서 레코드 연결 관리를 참조하세요](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * 연결 계획 사용자 정의 필드를 생성하여 Workfront 객체의 사용자 정의 양식에 첨부할 수 있습니다. 자세한 내용은 [사용자 지정 양식](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) 만들기 참조하십시오.
      * 계획 레코드 필드는 Workfront 관리자가 Workfront와 Adobe Experience Manager Assets 간의 통합을 통해 메타데이터 매핑을 구성할 때 Experience Manager 자산에서 액세스할 수 있습니다. 자세한 내용은 [Adobe Workfront과 Experience Manager Assets 간의 에셋 메타데이터 매핑 구성](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping)을 참조하십시오.


   * **연결된 레코드 또는 개체에서 조회 필드를 추가할 때**: 연결된 레코드 필드를 만들 수 있을 뿐만 아니라 연결된 레코드 또는 개체 형식의 필드에 연결할 수도 있습니다. 이 필드를 조회 필드라고 합니다. 연결하려는 레코드의 정보가 있는 연결된(또는 조회 필드) 필드는 연결하려는 레코드에 표시됩니다.

     다른 레코드 유형이나 다른 응용 프로그램 객체의 필드를 Workfront Planning 레코드 유형에 연결할 수 있습니다.

     연결된 필드는 읽기 전용이며 연결된 레코드의 정보를 자동으로 표시합니다.

     수식, 필터 또는 그룹화에서 다른 레코드 또는 개체 형식의 조회 필드를 참조할 수 있습니다.

     예를 들어 &quot;캠페인&quot; 레코드 유형을 Workfront 프로젝트와 연결하고 프로젝트의 계획된 완료 일자 필드를 Workfront 계획 레코드로 가져오도록 선택하면 캠페인에 대해 연결된 필드(프로젝트의 계획된 완료 일자)가 자동으로 생성됩니다. 이 링크된 필드는 수동으로 편집할 수 없습니다. 계획된 완료 날짜(프로젝트에서) 필드에는 링크된 프로젝트의 계획된 완료 날짜가 표시됩니다.

     >[!IMPORTANT]
     >
     >작업 영역에 대한 보기 이상의 사용 권한이 있는 모든 사용자는 연결된 개체 유형의 애플리케이션 또는 다른 작업 영역에서의 사용 권한에 관계없이 조회 필드의 정보를 볼 수 있습니다.

     연결된 레코드 필드 앞에는 관계 아이콘 ![관계 필드 아이콘](assets/relationship-field-icon.png)이 있습니다.

     링크된 필드 앞에는 필드 유형을 식별하는 아이콘이 표시됩니다. 예를 들어 연결된(또는 조회된) 필드 앞에는 필드가 숫자, 단락 또는 날짜임을 나타내는 아이콘이 있습니다.

     >[!TIP]
     >
     >Workfront 개체의 날짜 필드 정보는 Workfront에 표시되는 방식에 관계없이 Workfront Planning에서 24시간 형식으로 표시됩니다.
     >
     >예를 들어 Workfront에서 프로젝트의 계획된 시작 날짜가 오후 3:00 시로 표시되는 경우 가져온 조회 필드의 Workfront Planning에서는 15:00 로 표시됩니다.


## 연결 유형

두 레코드 종류 사이 또는 레코드와 다른 애플리케이션 오브젝트 종류 사이에 연결을 설정한 후 연결된 레코드 필드에 레코드를 추가할 수 있습니다.

연결된 레코드 필드에 추가할 수 있는 레코드 수에 따라 레코드 종류를 연결할 때 선택할 수 있는 연결 종류는 다음과 같습니다.

* [다대다](#many-to-many-connection-type)
* [일대다](#one-to-many-connection-type)
* [다대일](#many-to-one-connection-type)
* [일대일](#many-to-one-connection-type)

>[!WARNING]
>
>다음 연결 시 이러한 옵션을 사용할 수 없습니다.
>
>* 다른 작업 공간의 두 개 레코드
>
>* 레코드 유형 및 Experience Manager 에셋

### 다대다 연결 유형

![다대다 연결 선택기](assets/many-to-many-connection-picker.png)

레코드 유형 간에 다대다 연결을 만들면 두 레코드 유형의 연결 필드에서 여러 레코드를 선택할 수 있습니다.

예를 들어 캠페인과 프로젝트 간에 다대다 연결을 만드는 경우 각 캠페인에 대해 여러 프로젝트를 선택하고 각 프로젝트에 대해 여러 캠페인을 선택할 수 있습니다.

다대다 관계 유형의 실제 사례는 영화와 배우의 관계이다. 각 영화에는 여러 배우가 있을 수 있으며 각 배우는 여러 영화에서 연기할 수 있습니다.

이 연결 유형을 선택하면 저장 후 연결 유형을 변경할 수 없습니다.

### 일대다 연결 유형

![일대다 연결 선택기](assets/one-to-many-connection-picker.png)


레코드 종류 간에 일대다 연결을 만들 때 현재 레코드 종류의 연결 필드에서 여러 레코드를 선택할 수 있지만 연결하는 레코드 종류의 해당 연결 필드에서는 하나의 레코드만 선택할 수 있습니다. 두 번째 레코드 종류에 자동으로 생성되는 연결된 레코드 필드는 다대일 관계 유형으로 자동 설정됩니다.

예를 들어 캠페인과 프로젝트 간에 일대다 연결을 만드는 경우 각 캠페인에 대해 여러 프로젝트를 선택할 수 있지만 각 프로젝트는 하나의 캠페인에만 연결할 수 있습니다.

일대다 관계 유형의 실제 예는 도서관과 책 사이의 관계입니다 : 도서관에는 인벤토리에 많은 책이 있습니다. 그러나 하나의 특정 책은 특정 시점에 하나의 라이브러리에만 있을 수 있습니다.

이 연결 유형을 선택하면 나중에 다대다 연결 유형으로만 변경할 수 있습니다.

### 다대일 연결 유형

![다대일 연결 선택기](assets/many-to-one-connection-picker.png)


레코드 종류 간에 다대일 연결을 만들면 현재 레코드 종류의 각 레코드를 연결된 레코드 종류에서 하나의 레코드와만 연결할 수 있습니다. 두 번째 레코드 유형에서 자동으로 생성된 연결된 레코드 필드는 일대다 관계 유형으로 자동 설정됩니다.

예를 들어, 캠페인을 프로젝트와 연결하고 이 연결 유형을 선택하는 경우 캠페인에 프로젝트를 하나만 추가할 수 있습니다. 그러나 하나의 프로젝트에 여러 캠페인을 추가할 수 있습니다.

다대일 관계 유형의 실제 예는 많은 영화와 한 배우의 관계입니다. 한 배우는 많은 영화에 출연할 수 있지만 각 영화는 한 번만 특정 배우를 캐스팅할 수 있습니다.

이 연결 유형을 선택하면 나중에 다대다 연결 유형으로만 변경할 수 있습니다.

### 일대일 연결 유형

![일대일 연결 선택기](assets/one-to-one-connection-picker.png)

레코드 종류 간에 일대일 연결을 만들 때 두 레코드 종류 모두에서 각 레코드를 다른 레코드 종류의 레코드로만 연결할 수 있습니다.

예를 들어, 캠페인을 프로젝트와 연결하고 이 연결 유형을 선택하는 경우 하나의 캠페인과 하나의 프로젝트를 연결할 수 있습니다. 하나의 프로젝트는 하나의 캠페인에만 연결할 수 있습니다.

일대일 관계의 실제 예는 개인과 해당 국가의 고유 식별자(예: 사회 보장 번호, 여권 ID, 로컬 ID) 사이에 존재하는 것입니다. 각 개인에는 한 국가에 대한 고유 식별자가 하나만 있으며 각 고유 식별자는 한 개인에게만 연결할 수 있습니다.

이 연결 유형을 선택하면 나중에 다른 연결 유형으로 변경할 수 있습니다.
