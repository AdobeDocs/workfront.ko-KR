---
title: 연결된 레코드 유형 개요
description: 개별 레코드 종류가 서로 관련되는 방식을 나타내는 방법은 해당 레코드 종류를 연결하는 것입니다. 또한 Adobe Workfront Planning 레코드 유형을 다른 애플리케이션의 객체 유형과 연결하여 사용자 경험을 향상시키고 한 애플리케이션에서 집중할 수 있습니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '1973'
ht-degree: 1%

---


<!--keep the 30 limit verbiage in yellow til Jan 2026-->

# 연결된 레코드 유형 개요

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>을 참조하세요.

개별 레코드 유형을 연결하여 서로 관련되거나 다른 응용 프로그램의 오브젝트와 관련됨을 나타낼 수 있습니다.

이 문서에서는 레코드 유형 연결에 대한 개요를 살펴보고 레코드와 개체 유형 간에 설정할 수 있는 연결 유형에 대해 설명합니다.

레코드 종류를 연결하는 방법에 대한 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

## 레코드 유형 연결에 대한 고려 사항

Workfront Planning에서 연결하는 단계는 두 가지가 있습니다.

1. 다른 응용 프로그램에서 두 레코드 형식 또는 레코드 형식과 개체 형식 간의 연결을 설정합니다.

   레코드 종류를 연결하는 방법에 대한 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

1. 두 레코드 유형이 연결된 후 한 유형의 개별 레코드를 다른 유형의 레코드와 연결합니다. 레코드 연결에 대한 자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하십시오.

레코드 유형 연결에 대해 다음 사항을 고려하십시오.

* <span class="preview">Workfront Planning에서 하나의 레코드 유형에 대해 최대 30개의 연결된 필드를 사용할 수 있습니다.</span>

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
     >Adobe Experience Manager Assets 라이선스가 있어야 하며, Workfront Planning 레코드를 Adobe Experience Manager Assets에 연결하려면 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.
     >
     >Adobe Admin Console 온보딩에 대한 질문이 있는 경우 [Adobe 통합 경험 FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md)를 참조하십시오.

* 레코드 유형에 대한 레코드를 만든 후 연결된 레코드 필드를 통해 서로 연결할 수 있습니다.

  자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.

* 레코드 유형을 다른 레코드 유형이나 다른 응용 프로그램의 개체 유형과 연결한 후에는 다음과 같은 시나리오가 있습니다.

   * **두 Planning 레코드 형식을 연결할 때**: 연결 중인 레코드 형식에 연결된 레코드 필드가 만들어집니다. 새 연결 탭에서 연결된 레코드 유형에 해당 필드 만들기 설정을 사용하도록 설정한 경우에만 연결 중인 레코드 유형에 유사한 연결된 레코드 필드가 만들어집니다.

     예를 들어 &quot;Campaign&quot; 레코드 유형을 &quot;Product&quot; 레코드 유형과 연결하는 경우 이름을 &quot;Linked Product&quot;로 지정한 연결된 레코드 필드(연결 필드)가 캠페인 레코드 유형에 만들어집니다. 제품 레코드 유형에 자동으로 &quot;캠페인&quot;이라는 연결된 레코드 유형이 만들어집니다.

     예를 들어 다음과 같은 시나리오가 있습니다.

      * 연결된 레코드 유형에 해당 필드 만들기 설정을 사용하도록 설정하고 &quot;캠페인&quot; 레코드 유형을 &quot;제품&quot; 레코드 유형과 연결하면 &quot;연결된 제품&quot;으로 지정한 연결된 레코드 필드(연결 필드)가 캠페인 레코드 유형에 만들어집니다. 제품 레코드 유형에 자동으로 &quot;캠페인&quot;이라는 연결된 레코드 유형이 만들어집니다.
      * 연결된 레코드 종류 설정에서 해당 필드 만들기 설정을 비활성화하고 &quot;캠페인&quot; 레코드 종류를 &quot;제품&quot; 레코드 종류에 연결하면, &quot;연결된 제품&quot;이라고 지정한 연결된 레코드 필드(연결 필드)가 캠페인 레코드 종류에 만들어집니다. 자동으로 &quot;Campaign&quot;으로 이름이 지정된 연결된 레코드 종류는 제품 레코드 종류에 만들어지지 않습니다.

     자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

   * **다른 응용 프로그램의 개체 형식과 레코드 형식을 연결하는 경우**:

      * 연결하는 레코드 종류에 연결된 레코드 필드가 만들어집니다. 연결된 레코드 필드는 다른 응용 프로그램의 개체 유형에 자동으로 만들어지지 않습니다.
      * Workfront 오브젝트에서 Planning 레코드 필드에 액세스할 수 없습니다.
      * 계획 레코드는 Workfront 오브젝트의 계획 탭에서 볼 수 있습니다. 자세한 내용은 [Workfront 개체에서 레코드 연결 관리](/help/quicksilver/planning/records/manage-records-in-planning-section.md)를 참조하십시오.
      * Planning 연결 사용자 정의 필드를 만들어 Workfront 객체의 사용자 정의 양식에 첨부할 수 있습니다. 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
      * Workfront 관리자가 Experience Manager과 Adobe Experience Manager Assets 간의 통합을 통해 메타데이터 매핑을 구성할 때 Workfront Assets에서 계획 레코드 필드에 액세스할 수 있습니다. 자세한 내용은 [Adobe Workfront과 Experience Manager Assets 간의 에셋 메타데이터 매핑 구성](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping)을 참조하십시오.


   * **연결된 레코드 또는 개체에서 조회 필드를 추가할 때**: 연결된 레코드 필드를 만들 수 있을 뿐만 아니라 연결된 레코드 또는 개체 형식의 필드에 연결할 수도 있습니다. 이 필드를 조회 필드라고 합니다. 연결하려는 레코드의 정보가 있는 연결된(또는 조회 필드) 필드는 연결하려는 레코드에 표시됩니다.

     다른 레코드 유형이나 다른 응용 프로그램 객체의 필드를 Workfront Planning 레코드 유형에 연결할 수 있습니다.

     연결된 필드는 읽기 전용이며 연결된 레코드의 정보를 자동으로 표시합니다.

     수식, 필터 또는 그룹화에서 다른 레코드 또는 개체 형식의 조회 필드를 참조할 수 있습니다.

     예를 들어 &quot;캠페인&quot; 레코드 유형을 Workfront 프로젝트와 연결하고 프로젝트의 계획된 완료 일자 필드를 Workfront 계획 레코드로 가져오도록 선택하면 캠페인에 대해 연결된 필드(프로젝트의 계획된 완료 일자)가 자동으로 생성됩니다. 연결된 이 필드는 수동으로 편집할 수 없습니다. 계획된 완료 일자(프로젝트 시작) 필드에는 연결된 프로젝트의 계획된 완료 일자가 표시됩니다.

     >[!IMPORTANT]
     >
     >작업 영역에 대한 보기 이상의 권한이 있는 모든 사용자는 링크된 객체 유형의 응용 프로그램에서 자신의 권한 또는 액세스 수준이나 다른 작업 영역에서 본인의 권한에 관계없이 조회 필드에서 정보를 볼 수 있습니다.

     연결된 레코드 필드 앞에는 관계 아이콘 ![관계 필드 아이콘](assets/relationship-field-icon.png)이(가) 있습니다.

     연결된 필드 앞에는 필드 유형을 식별하는 아이콘이 표시됩니다. 예를 들어 연결된(또는 조회) 필드 앞에는 필드가 숫자, 단락 또는 날짜임을 나타내는 아이콘이 표시됩니다.

     >[!TIP]
     >
     >Workfront 개체의 날짜 필드 정보는 Workfront에 표시되는 방식에 관계없이 Workfront Planning에서 24시간 형식으로 표시됩니다.
     >
     >예를 들어 프로젝트의 계획된 시작 일자가 Workfront에서 오후 3:00(으)로 표시되는 경우 가져온 조회 필드에서는 Workfront Planning에서 15:00(으)로 표시됩니다.


## 연결 유형

두 레코드 유형 간에 또는 다른 응용 프로그램의 레코드와 개체 유형 간에 연결을 설정한 후 연결된 레코드 필드에 레코드를 추가할 수 있습니다.

>[!WARNING]
>
>다음 연결 시 이러한 옵션을 사용할 수 없습니다.
>
>* 다른 작업 공간의 두 개 레코드
>
>* 레코드 유형 및 Experience Manager 에셋

한 번에 하나의 레코드를 여러 레코드에 연결할지 또는 한 번에 하나의 레코드를 서로 연결할지 선택할 수 있습니다.

다음은 레코드 유형을 연결할 때 선택할 수 있는 연결 유형입니다.

* **연결된 레코드 종류에 해당 필드 만들기** 설정을 사용하지 않도록 설정한 경우 다음 중에서 선택할 수 있습니다.

   * [다중 선택](#multi-select-connection-type)
   * [단일 선택](#single-select-connection-type)

* **연결된 레코드 종류에 해당 필드 만들기** 설정을 사용하면 다음 중에서 선택할 수 있습니다.

   * [다대다](#many-to-many-connection-type)
   * [일대다](#one-to-many-connection-type)
   * [다대일](#many-to-one-connection-type)
   * [일대일](#many-to-one-connection-type)

### 다중 선택 연결 유형

![여러 연결 유형 선택](assets/multi-select-connection-picker.png)

레코드 유형 간에 다중 선택 연결을 만들면 원래 레코드 유형의 연결 필드에서 연결된 여러 레코드를 선택할 수 있습니다.

예를 들어 캠페인과 프로젝트 간에 다중 선택 연결을 만드는 경우 하나의 캠페인에 대해 여러 프로젝트를 선택할 수 있습니다. 프로젝트 오브젝트 유형에 대해 Campaign 연결된 레코드 유형이 만들어지지 않습니다.

이 연결 유형을 선택한 후 다음 유형에 저장한 후에는 연결 유형을 변경할 수 없습니다.

* 단일 선택
* 일대다
* 다대일
* 일대일

### 단일 선택 연결 유형

![단일 연결 유형 선택](assets/single-select-connection-picker.png)

레코드 유형 간에 단일 선택 연결을 만들면 원래 레코드 유형의 연결 필드에서 하나의 레코드를 선택할 수 있습니다.

예를 들어 캠페인과 회사 간에 단일 선택 연결을 만드는 경우 하나의 캠페인에 대해 하나의 회사를 선택할 수 있습니다. 회사 오브젝트 유형에 대해 캠페인 연결 레코드 유형이 생성되지 않습니다.

이 연결 유형을 선택한 후 다음 중 하나에 저장한 후에는 연결 유형을 변경할 수 없습니다.

* 일대다
* 일대일

</div>


<!--
* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)
-->

### 다대다 연결 유형

![다대다 연결 선택기](assets/many-to-many-connection-picker.png)

레코드 유형 간에 다대다 연결을 만들면 두 레코드 유형의 연결 필드에서 여러 레코드를 선택할 수 있습니다.

예를 들어 캠페인과 프로젝트 간에 다대다 연결을 만드는 경우 각 캠페인에 대해 여러 프로젝트를 선택하고 각 프로젝트에 대해 여러 캠페인을 선택할 수 있습니다.

다대다 관계 유형의 실제 사례는 영화와 배우의 관계이다. 각 영화에는 여러 명의 배우가 출연할 수 있으며, 각 배우는 여러 영화에서 연기할 수 있다.

이 연결 유형을 선택하면 저장한 후 연결 유형을 변경할 수 없습니다.

### 일대다 연결 유형

![일대다 연결 선택기](assets/one-to-many-connection-picker.png)


레코드 유형 간에 일대다 연결을 만들 때 현재 레코드 유형의 연결 필드에서 여러 레코드를 선택할 수 있지만 연결하는 레코드 유형의 해당 연결 필드에서는 하나의 레코드만 선택할 수 있습니다. 두 번째 레코드 유형에서 자동으로 생성된 연결된 레코드 필드는 다대일 관계 유형으로 자동 설정됩니다.

예를 들어 캠페인과 프로젝트 간에 일대다 연결을 만드는 경우 각 캠페인에 대해 여러 프로젝트를 선택할 수 있지만 각 프로젝트는 하나의 캠페인에만 연결할 수 있습니다.

일대다 관계 유형의 실제 예는 라이브러리와 책 간의 관계입니다. 라이브러리에는 인벤토리에 많은 책이 있지만 특정 시간에 한 개의 특정 책만 한 라이브러리에 있을 수 있습니다.

이 연결 유형을 선택하면 나중에 다대다 연결 유형으로만 변경할 수 있습니다.

### 다대일 연결 유형

![다대일 연결 선택기](assets/many-to-one-connection-picker.png)


레코드 유형 간에 다대일 연결을 만들면 현재 레코드 유형의 각 레코드를 연결된 레코드 유형의 레코드와 연결할 수 있습니다. 두 번째 레코드 유형에서 자동으로 생성된 연결된 레코드 필드는 일대다 관계 유형으로 자동 설정됩니다.

예를 들어, 캠페인을 프로젝트와 연결하고 이 연결 유형을 선택하는 경우 캠페인에 프로젝트를 하나만 추가할 수 있습니다. 그러나 하나의 프로젝트에 여러 캠페인을 추가할 수 있습니다.

다대일 관계 유형의 실제 예는 많은 영화와 한 배우의 관계입니다. 한 배우는 많은 영화에 출연할 수 있지만 각 영화는 한 번만 특정 배우를 캐스팅할 수 있습니다.

이 연결 유형을 선택하면 나중에 다대다 연결 유형으로만 변경할 수 있습니다.

### 일대일 연결 유형

![일대일 연결 선택기](assets/one-to-one-connection-picker.png)

레코드 종류 간에 일대일 연결을 만들 때 두 레코드 종류 모두에서 각 레코드를 다른 레코드 종류의 레코드로만 연결할 수 있습니다.

예를 들어, 캠페인을 프로젝트와 연결하고 이 연결 유형을 선택하는 경우 하나의 캠페인과 하나의 프로젝트를 연결할 수 있습니다. 하나의 프로젝트는 하나의 캠페인에만 연결할 수 있습니다.

일대일 관계의 실제 예는 개인과 해당 국가의 고유 식별자(예: 사회 보장 번호, 여권 ID, 로컬 ID) 사이에 존재하는 것입니다. 각 개인에는 한 국가에 대한 고유 식별자가 하나만 있으며 각 고유 식별자는 한 개인에게만 연결할 수 있습니다.

이 연결 유형을 선택하면 나중에 다른 연결 유형으로 변경할 수 있습니다.
