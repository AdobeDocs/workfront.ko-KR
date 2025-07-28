---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: ' [!DNL Adobe Workfront] 개체에서  [!DNL Salesforce] 프로젝트 만들기'
description: Salesforce용  [!DNL Adobe Workfront] 을(를) 설치한 후  [!DNL Workfront] 기회 및 계정에서 특정 기준을 충족할 때  [!DNL Salesforce] 프로젝트를 만드는 트리거를 정의할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1581'
ht-degree: 3%

---

# [!DNL Adobe Workfront] 개체에서 [!DNL Salesforce] 프로젝트 만들기

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 Salesforce용 Workfront 통합을 사용할 수 없습니다.
>
>조직의 Salesforce 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Salesforce용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Salesforce 모듈](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules)을 참조하십시오.

Salesforce용 [!DNL Adobe Workfront]을(를) 설치한 후 [!DNL Workfront] [!DNL Salesforce]기회[!UICONTROL &#x200B; 및 &#x200B;]계정[!UICONTROL 에서 특정 기준이 충족되면 &#x200B;] 프로젝트를 만드는 트리거를 정의할 수 있습니다.

## 액세스 요구 사항

이 문서에 설명된 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL 계획]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 전제 조건

[!DNL Workfront] [!DNL Salesforce]기회[!UICONTROL &#x200B; 또는 계정에서 &#x200B;] 요청을 제출하려면
환경에 다음 사항이 있는지 확인합니다.

* [!DNL Workfront] 관리자가 [!DNL Workfront for Salesforce]을(를) 설치했습니다.\
   [!DNL Workfront for Salesforce] 설치에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)를 참조하십시오

* [!DNL Workfront] 관리자가 [!DNL Workfront]영업 기회[!UICONTROL &#x200B; 및 계정에 &#x200B;] 섹션을 추가했습니다.
페이지 레이아웃입니다.\
   페이지 레이아웃에 [!DNL Workfront] 섹션을 추가하는 방법에 대한 자세한 내용은 [사용자를 위한  [!DNL Adobe Workfront] 섹션 구성 [!DNL Salesforce] 을 참조하십시오](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* [!DNL Workfront] 계정이 있으며 [!DNL Workfront]기회[!UICONTROL &#x200B; 또는 계정 내의 &#x200B;] 섹션에서 로그인할 수 있습니다.
.

## [!DNL Workfront]에서 [!DNL Salesforce] 프로젝트 만들기 구성

* [프로젝트 자동 생성 이해](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [트리거 구성](#configuring-triggers-configuring-triggers)
* [프로젝트 이름 이해](#understanding-project-names-understanding-project-names)

### 프로젝트 자동 생성 이해 {#understanding-the-automatic-creation-of-projects}

[!DNL Salesforce] 시스템 관리자는 [!DNL Workfront]에서 다음 상황이 발생할 때 [!DNL Salesforce]에서 프로젝트를 자동으로 만들 수 있는 트리거를 정의할 수 있습니다.

* [!UICONTROL 기회]의 [!UICONTROL 단계]이(가) 업데이트되었습니다.
* 계정의 [!UICONTROL 유형]
이(가) 업데이트되었습니다.

[!DNL Workfront for Salesforce]을(를) 설치한 후에만 트리거를 구성할 수 있습니다.  \
[!DNL Workfront for Salesforce] 설치에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)를 참조하십시오.

[!DNL Workfront]개 항목을 만들거나 업데이트할 때 [!DNL Salesforce]개 프로젝트를 자동으로 만들도록 트리거를 구성할 때는 다음 사항을 고려하십시오.

* 트리거를 구성하려면 [!DNL Salesforce] 및 [!DNL Workfront] 시스템 관리자여야 합니다.
* 트리거를 구성하고 나면 [!UICONTROL Opportunity]의 [!UICONTROL Stage] 또는 계정의 [!UICONTROL Type]을(를) 업데이트하는 모든 사용자가
[!DNL Workfront] 프로젝트 만들기를 트리거할 수 있습니다. 여기에는 [!DNL Salesforce] 계정이 없는 [!DNL Workfront]명의 사용자가 포함됩니다.
* 가질 수 있는 트리거 수에 제한은 없습니다.
* 동일한 조건을 기준으로 여러 트리거를 만들 수 없습니다. 트리거는 기본적으로 고유합니다.
* 프로젝트가 생성되면 생성된 영업 기회 또는 계정에 자동으로 연결됩니다. 일단 설정되면 이 링크를 끊을 수 없습니다.
* [!DNL Workfront]의 여러 프로젝트에 연결된 기회 또는 계정은 해당 기회 또는 계정의 수명 동안 트리거된 조건이 여러 번 충족될 때 연결될 수 있습니다.

  예를 들어, 프로젝트를 트리거하기 위해 [!UICONTROL 기회]에 대해 [!UICONTROL 단계]를 두 개 이상 정의하는 경우 해당 기회의 수명 동안 기회가 도달하는 정의된 모든 단계에 대해 프로젝트가 만들어집니다. 또한 [!UICONTROL Opportunity]의 [!UICONTROL Stage]을(를) 정의된 단계에서 다른 단계로 업데이트한 다음 다시 정의된 단계로 업데이트하면 [!UICONTROL Stage] 필드를 정의된 동일한 단계로 두 번째로 업데이트할 때 두 번째 프로젝트가 만들어집니다.

* [!DNL Workfront]의 프로젝트 중 하나는 지정된 시간에 한 개의 영업 기회 또는 [!DNL Salesforce]의 한 계정에만 연결할 수 있지만 두 계정과 동시에 연결할 수는 없습니다.

### 트리거 구성 {#configuring-triggers}

트리거를 구성하고 나면 [!DNL Workfront]Salesforce Classic[!UICONTROL &#x200B; 또는 &#x200B;] 프레임워크 모두에서 [!DNL Lightning Experience] 프로젝트를 만드는 프로세스를 사용할 수 있습니다.

[!UICONTROL Salesforce]에서 트리거를 구성하려면:

1. 시스템 관리자로 [!DNL Salesforce]에 로그인합니다.
1. (조건부) [!DNL Salesforce Classic]에서 **[!UICONTROL 설정]**&#x200B;을 클릭하고 **[!UICONTROL 빌드]** 섹션에서 **[!UICONTROL 번개 볼트]**&#x200B;를 확장합니다.

   또는

   [!DNL Salesforce] 번개 경험에서 **[!UICONTROL 설정] 아이콘**&#x200B;을 클릭한 다음 **[!UICONTROL 설정]**&#x200B;을 클릭하고 **[!UICONTROL 플랫폼 도구]**&#x200B;에서 **[!UICONTROL 앱]**&#x200B;을 확장합니다.

1. **[!UICONTROL 설치된 패키지]**&#x200B;를 클릭합니다.

   **[!DNL Workfront]** 패키지가 설치되었습니다.

1. **[!UICONTROL 옆에 있는]**&#x200B;구성&#x200B;**[!DNL Workfront]**&#x200B;을 클릭합니다.

1. 시스템 관리자로 [!DNL Workfront]에 로그인합니다.

   **[!UICONTROL 트리거]** 페이지가 표시됩니다.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. **[!UICONTROL 새 트리거]**&#x200B;를 클릭합니다.
1. **[!UICONTROL [!DNL Salesforce]개체]** 드롭다운 메뉴에서 **[!UICONTROL 기회]**&#x200B;를 선택합니다.

   필수 필드입니다.

1. (조건부) 다음을 지정합니다.

   1. **[!UICONTROL 단계]** 드롭다운 메뉴에서 **[!UICONTROL 단계]**&#x200B;을(를) 선택합니다.\

      기회가 여기에 지정된 [!UICONTROL 단계]에 도달하면 프로젝트가 [!DNL Workfront]에 만들어집니다. 필수 필드입니다.

   1. **[!UICONTROL Portfolio 또는 프로그램]** 필드에서 프로젝트를 [!DNL Workfront]에 배치할 Portfolio 또는 프로그램의 이름을 입력한 다음 목록에 표시될 때 선택합니다.\

      Portfolio 또는 프로그램을 지정하지 않으면 새 프로젝트가 만들어지고 트리거를 구성할 때 [!UICONTROL 에 로그인한 사용자의 &#x200B;]내가 소유한 프로젝트[!DNL Workfront] 목록에 추가됩니다. 이 사용자는 새 프로젝트의 프로젝트 소유자이기도 합니다.

   1. 새 [!DNL Workfront] 프로젝트와 연결할 템플릿 이름을 입력한 다음 목록에 표시될 때 선택하십시오.\

      필수 필드입니다.


      >[!NOTE]
      >
      >이 통합에 사용할 템플릿에 템플릿 소유자를 지정한 경우 이 소유자가 새 프로젝트의 프로젝트 소유자가 됩니다. 새 프로젝트는 템플릿에 따라 새 프로젝트의 소유자인 사용자의 [!UICONTROL 내가 소유한 프로젝트] 목록에 표시됩니다.

   1. (선택 사항) 한 번의 기회에 판매된 모든 제품 유형에 대해 새 프로젝트를 만들려면 **[!UICONTROL 판매된 각 제품 유형에 대해 새 프로젝트 만들기] 필드**&#x200B;를 선택합니다.
   1. (조건부) **[!UICONTROL 제품]** 드롭다운 메뉴에서 **[!UICONTROL 제품]**&#x200B;을(를) 선택합니다.

      필수 필드입니다.

   1. (조건부) 지정한 제품이 **[!UICONTROL 기회]**&#x200B;에 있는 경우 새 [!DNL Workfront] 프로젝트와 연결할 [!UICONTROL 템플릿]의 이름을 입력하세요. 목록에 나타나면 선택합니다.

      필수 필드입니다.

      [!DNL Salesforce] 영업 기회에 새 제품을 추가할 때 만들어진 프로젝트는 해당 영업 기회에 대해 선택한 동일한 Portfolio 또는 프로그램에 배치됩니다.

      >[!IMPORTANT]
      >
      >[!UICONTROL 기회]에 단계가 업데이트될 때만 프로젝트가 만들어집니다. [!UICONTROL Opportunities]에 추가된 제품이 아니라 단계 필드를 업데이트할 때 지정된 각 제품에 대해 고유한 프로젝트가 만들어집니다.

1. (선택 사항) **[!UICONTROL 새 트리거]**&#x200B;를 클릭합니다.
1. (선택 사항) **[!UICONTROL [!DNL Salesforce]Object]** 드롭다운 메뉴에서 **Account)를 선택합니다
**.

   필수 필드입니다.
1. (조건부) 다음을 지정합니다.

   1. **[!UICONTROL Type]** 드롭다운 메뉴에서 **[!UICONTROL Type]**&#x200B;을(를) 선택합니다.

      **계정
**2&rbrace;에 지정된 &#x200B;** [!UICONTROL Type]&#x200B;**(으)로 지정되었으며 [!DNL Salesforce]에 &#x200B;** [!UICONTROL Project]**&#x200B;이(가) 만들어집니다.[!DNL Workfront]

      필수 필드입니다.

   1. (선택 사항) 프로젝트를 **[!UICONTROL Portfolio 또는 프로그램]** 필드의 **[!UICONTROL 에 배치할]** Portfolio[!DNL Workfront] 또는 **[!UICONTROL 프로그램]**&#x200B;의 이름을 입력한 다음 목록에 표시될 때 선택합니다.

      Portfolio 또는 프로그램을 지정하지 않으면 새 프로젝트가 만들어지고 **[!UICONTROL 에서]**&#x200B;에 로그인한 사용자의 [!DNL Workfront]내가 소유한 프로젝트[!DNL Salesforce] 목록에 추가됩니다. 사용자는 새 프로젝트의 프로젝트 소유자이기도 합니다.

   1. 새 **[!UICONTROL 프로젝트와 연결할]**&#x200B;템플릿[!DNL Workfront]의 이름을 입력한 다음 목록에 표시될 때 선택하십시오.

      필수 필드입니다.

      >[!NOTE]
      >
      >이 통합에 사용할 템플릿에 템플릿 소유자를 지정한 경우 이 소유자가 새 프로젝트의 프로젝트 소유자가 됩니다. 새 프로젝트는 템플릿에 따라 새 프로젝트의 소유자인 사용자의 **[!UICONTROL 내가 소유한 프로젝트]** 목록에 표시됩니다.

   ![salesforce_triggers_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 트리거가 충족될 때마다 [!DNL Workfront]개의 프로젝트가 생성됩니다.

### 프로젝트 이름 이해 {#understanding-project-names}

프로젝트를 생성한 트리거에 따라 [!DNL Workfront]의 프로젝트 이름이 다음 패턴 중 하나를 따를 수 있습니다.

* 영업 기회 또는 계정 트리거를 기반으로 프로젝트를 만드는 경우 프로젝트 이름은 *`<Salesforce object name>`: `<Project template name>`([!DNL Salesforce]을 통해)*&#x200B;입니다.
* 새 제품의 추가도 포함하는 영업 기회 트리거를 기반으로 프로젝트를 만드는 경우 프로젝트 이름은 *`<Salesforce object name>`: `<Salesforce product name>`([!DNL Salesforce]을 통해)*&#x200B;입니다.

## [!DNL Workfront]개 프로젝트 보기

[!DNL Workfront] 관리자가 [!DNL Workfront]기회[!UICONTROL &#x200B; 또는 계정에 &#x200B;] 섹션을 추가한 경우
페이지 레이아웃에서는 이 섹션의 [!UICONTROL 프로젝트] 탭에서 자동으로 만들어진 프로젝트를 볼 수 있습니다.\
[!DNL Workfront]Opportunity[!UICONTROL &#x200B; 또는 계정의 페이지 레이아웃에 &#x200B;] 섹션을 추가하는 방법에 대한 자세한 정보
, [사용자 [!DNL Adobe Workfront] 를 위한  [!DNL Salesforce] 섹션 구성](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)을 참조하십시오.

[!DNL Workfront]프로젝트[!DNL Workfront] 탭을 보려면 [!UICONTROL &#x200B; 계정이 있어야 하며 &#x200B;]에 로그인해야 합니다.

[!UICONTROL 영업 기회] 또는 계정에서 만든 프로젝트를 보려면
:

1. [!UICONTROL 기회] 또는 계정으로 이동
.
1. **[!DNL Workfront]** 섹션으로 이동합니다.

   >[!NOTE]
   >
   >[!DNL Workfront] 관리자가 이 섹션을 구성한 방법에 따라 다른 이름을 사용할 수 있습니다.

1. **[!UICONTROL 프로젝트]** 탭을 선택합니다.

   정의된 트리거에서 만든 모든 프로젝트가 이 탭에 나열됩니다. [!DNL Salesforce]의 사용자 중 [!DNL Workfront] 계정을 가지고 있고 [!DNL Workfront]에서 이러한 프로젝트를 볼 수 있는 권한이 있는 모든 사용자는 [!DNL Salesforce]에서 [!UICONTROL Opportunity] 또는 계정에 대해서도 볼 수 있습니다
그것이 그들을 생성했습니다.

   통합으로 생성된 프로젝트에 대한 다음 정보를 볼 수 있습니다.

   * 프로젝트 이름
   * 참조 번호
   * 입력 일자
   * 소유자 이름
   * 상태
   * 조건
   * 계획된 완료 일자 기준
   * 완료율

     [!DNL Workfront]에서 이 정보가 업데이트되면 이 목록에서 업데이트된 필드를 볼 수 있습니다.

1. (선택 사항) 프로젝트 이름을 클릭하여 Workfront에서 엽니다.
1. (선택 사항) [!UICONTROL **[!UICONTROL 프로젝트 세부 정보]**] 영역 또는 프로젝트 헤더에서 [!UICONTROL Salesforce으로 이동]을 클릭하여 [!UICONTROL 기회] 또는 계정에 액세스합니다
프로젝트가 시작된 위치입니다. 시스템 또는 그룹 관리자가 레이아웃 템플릿에 [!UICONTROL 통합] 필드를 추가하여 프로젝트 헤더에서 찾아야 합니다.

   >[!NOTE]
   >
   >[!UICONTROL Salesforce으로 이동] 링크가 프로젝트를 볼 수 있는 모든 [!DNL Workfront] 사용자에게 표시됩니다. 프로젝트가 생성된 위치에서 [!DNL Salesforce] 영업 기회 또는 계정으로 이동할 수 있으려면 [!DNL Salesforce] 계정이 있어야 합니다.
