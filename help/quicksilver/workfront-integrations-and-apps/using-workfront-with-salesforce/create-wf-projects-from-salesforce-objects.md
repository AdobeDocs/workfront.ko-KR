---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: 만들기 [!DNL Adobe Workfront] 프로젝트 위치 [!DNL Salesforce] 개체
description: 설치 후 [!DNL Adobe Workfront] Salesforce의 경우 [!DNL Workfront] 특정 기준이 충족될 때 프로젝트 [!DNL Salesforce] 기회 및 계정
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '1507'
ht-degree: 3%

---

# 만들기 [!DNL Adobe Workfront] 프로젝트 위치 [!DNL Salesforce] 개체

설치 후 [!DNL Adobe Workfront] Salesforce의 경우 [!DNL Workfront] 특정 기준이 충족될 때 프로젝트 [!DNL Salesforce] [!UICONTROL 기회] 및 [!UICONTROL 계정].

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

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

을(를) 제출하려면 [!DNL Workfront] 다음에서 요청 [!DNL Salesforce] [!UICONTROL 기회] 또는 계정이 환경에 다음 항목이 있는지 확인합니다.

* 사용자 [!DNL Workfront] 관리자가 설치됨 [!DNL Workfront for Salesforce].\
   설치에 대한 자세한 정보 [!DNL Workfront for Salesforce]를 참조하십시오. [설치 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 사용자 [!DNL Workfront] 관리자가 추가되었습니다. [!DNL Workfront] 섹션에 대한 섹션을 참조하십시오. [!UICONTROL 기회] 및 계정 페이지 레이아웃.\
   추가 정보에 대한 자세한 정보 [!DNL Workfront] 페이지 레이아웃에 대한 자세한 내용은 [구성 [!DNL Adobe Workfront] 섹션 [!DNL Salesforce] 사용자](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* 다음을 수행합니다. [!DNL Workfront] 계정 및에서 로그인할 수 있습니다. [!DNL Workfront] 섹션 내부 [!UICONTROL 기회] 또는 계정 을 참조하십시오.

## 만들기 구성 [!DNL Workfront] 프로젝트 출처 [!DNL Salesforce]

* [프로젝트 자동 생성 이해](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [트리거 구성](#configuring-triggers-configuring-triggers)
* [프로젝트 이름 이해](#understanding-project-names-understanding-project-names)

### 프로젝트 자동 생성 이해 {#understanding-the-automatic-creation-of-projects}

로서의 [!DNL Salesforce] 시스템 관리자는 [!DNL Workfront] 다음의 상황이 발생하는 경우 [!DNL Salesforce]:

* 다음 [!UICONTROL 단계] / [!UICONTROL 기회] 가 업데이트됩니다.
* 다음 [!UICONTROL 유형] 의 계정이 업데이트됩니다.

트리거는 설치한 후에만 구성할 수 있습니다 [!DNL Workfront for Salesforce].  \
설치에 대한 자세한 정보 [!DNL Workfront for Salesforce]를 참조하십시오. [설치 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

트리거를 구성하여 자동으로 만들 때 다음 사항을 고려하십시오 [!DNL Workfront] 프로젝트 시 [!DNL Salesforce] 항목이 만들어지거나 업데이트되었습니다.

* 넌 [!DNL Salesforce] 그리고 [!DNL Workfront] 트리거를 구성할 시스템 관리자
* 트리거를 구성하고 나면 [!UICONTROL 단계] / [!UICONTROL 기회] 또는 [!UICONTROL 유형] 계정 생성 [!DNL Workfront] 프로젝트. 여기에는 다음이 포함됩니다 [!DNL Salesforce] 없는 사용자 [!DNL Workfront] 계정이 필요합니다.
* 가질 수 있는 트리거의 수에 제한이 없습니다.
* 동일한 조건을 기준으로 여러 트리거를 만들 수 없습니다. 트리거는 기본적으로 고유합니다.
* 프로젝트가 생성되면 해당 프로젝트가 생성된 영업 기회 또는 계정에 자동으로 연결됩니다. 설정된 링크는 끊어지지 않습니다.
* 하나의 기회나 계정을 [!DNL Workfront] 트리거된 조건이 영업 기회 또는 계정에서 여러 번 충족된 경우.

   예를 들어, [!UICONTROL 단계] 대상 [!UICONTROL 기회] 프로젝트를 트리거하기 위해 해당 기회의 수명 동안 기회가 도달하는 모든 정의된 단계에 대해 프로젝트가 만들어집니다. 또한 [!UICONTROL 단계] / [!UICONTROL 기회] 정의된 한 단계에서 다른 스테이지로 업데이트한 다음 다시 정의된 스테이지로 업데이트하면 두 번째 프로젝트를 업데이트한 후에 두 번째 프로젝트가 만들어집니다 [!UICONTROL 단계] 필드를 동일한 정의된 단계에 추가합니다.

* 에 프로젝트 한 개 [!DNL Workfront] 의 한 개 또는 한 개 계정에만 연결할 수 있습니다. [!DNL Salesforce] 언제든지, 동시에 둘 다 그렇지 않습니다.

### 트리거 구성 {#configuring-triggers}

트리거를 구성하고 나면 생성 프로세스를 만듭니다 [!DNL Workfront] 두 프로젝트 모두에 대해 프로젝트가 활성화되어 있습니다. [!UICONTROL Salesforce Classic] 또는 [!DNL Lightning Experience] 프레임워크.

에서 트리거를 구성하려면 [!UICONTROL Salesforce]:

1. 에 로그인합니다. [!DNL Salesforce] 시스템 관리자로 사용됩니다.
1. (조건부) in [!DNL Salesforce Classic]를 클릭합니다. **[!UICONTROL 설정]**&#x200B;및 **[!UICONTROL 빌드]** 섹션, 확장 **[!UICONTROL 번개 볼트]**.

   또는

   in [!DNL Salesforce] 번개 경험에서 **[!UICONTROL 설정] 아이콘**, 그런 다음 **[!UICONTROL 설정]**, 및 아래 **[!UICONTROL 플랫폼 도구]** 확장 **[!UICONTROL 앱]**.

1. 클릭 **[!UICONTROL 설치된 패키지]**.

   다음 사항에 주의하십시오. **[!DNL Workfront]** 패키지가 설치되었습니다.

1. 클릭 **[!UICONTROL 구성]** 다음 **[!DNL Workfront]**.

1. 에 로그인합니다. [!DNL Workfront] 시스템 관리자

   다음 **[!UICONTROL Triggers]** 페이지가 표시됩니다.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. 클릭 **[!UICONTROL 새 트리거]**.
1. 에서 **[!UICONTROL [!DNL Salesforce]개체]** 드롭다운 메뉴에서 **[!UICONTROL 기회]**.

   필수 필드입니다.

1. (조건부) 다음을 지정합니다.

   1. 에서 **[!UICONTROL 단계]** 드롭다운 메뉴에서 **[!UICONTROL 단계]**.\

      기회가 에 도달하면 [!UICONTROL 단계] 여기에 지정된 프로젝트는에서 생성됩니다 [!DNL Workfront]. 필수 필드입니다.

   1. 에서 **[!UICONTROL Portfolio 또는 프로그램]** 필드에서 프로젝트를 배치할 Portfolio 또는 프로그램의 이름을 입력합니다 [!DNL Workfront]를 선택한 다음 목록에 나타나면 선택합니다.\

      Portfolio 또는 프로그램을 지정하지 않으면 새 프로젝트가 생성되고 [!UICONTROL 프로젝트 소유] 로그인한 사용자 목록 [!DNL Workfront] 트리거 구성 시. 이 사용자는 새 프로젝트의 프로젝트 소유자입니다.

   1. 새 템플릿에 연결할 템플릿의 이름을 입력합니다 [!DNL Workfront] 프로젝트를 선택한 다음 목록에 표시될 때 선택합니다.\

      필수 필드입니다.


      >[!NOTE]
      >
      >이 통합에 사용할 템플릿에 템플릿 소유자를 지정한 경우 해당 템플릿 소유자가 새 프로젝트의 프로젝트 소유자가 됩니다. 새 프로젝트는 [!UICONTROL 프로젝트 소유] 템플릿에 따라 새 프로젝트의 소유자인 사용자 목록입니다.

   1. (선택 사항) **[!UICONTROL 판매된 각 제품 유형에 대해 새 프로젝트를 만듭니다] 필드**&#x200B;를 지정하는 경우, 하나의 영업 기회에 판매되는 모든 유형의 제품에 대해 새 프로젝트를 생성하려는 경우
   1. (조건부) **[!UICONTROL 제품]** 에서 **[!UICONTROL 제품]** 드롭다운 메뉴

      필수 필드입니다.

   1. (조건부) 이름 입력을 시작합니다 **[!UICONTROL 템플릿]** 새 [!DNL Workfront] 지정된 제품이 [!UICONTROL 기회]. 목록에 있으면 선택합니다.

      필수 필드입니다.

      새 제품이 [!DNL Salesforce] 영업 기회는 영업 기회에 대해 선택한 동일한 Portfolio 또는 프로그램에 배치됩니다.

      >[!IMPORTANT]
      >
      >프로젝트는 스테이지가 [!UICONTROL 기회]. 스테이지 필드가 업데이트될 때 지정된 각 제품에 대해 고유한 프로젝트가 생성되며, 제품이 추가되지 않습니다 [!UICONTROL 기회].

1. (선택 사항) **[!UICONTROL 새 트리거]**.
1. (선택 사항) **[!UICONTROL [!DNL Salesforce]개체]** 드롭다운 메뉴에서 **계정 **을 선택합니다.

   필수 필드입니다.
1. (조건부) 다음을 지정합니다.

   1. 선택 **[!UICONTROL 유형]** 에서 **[!UICONTROL 유형]** 드롭다운 메뉴

      **Account **가 **[!UICONTROL 유형]** 여기에 지정 [!DNL Salesforce], **[!UICONTROL 프로젝트]** 에 작성되어 있습니다. [!DNL Workfront].

      필수 필드입니다.

   1. (선택 사항) 이름 입력을 시작합니다 **[!UICONTROL Portfolio]** 또는 **[!UICONTROL 프로그램]** 프로젝트를 배치할 위치 [!DNL Workfront] 에서 **[!UICONTROL Portfolio 또는 프로그램]** 필드를 선택한 다음 목록에 표시될 때 선택합니다.

      Portfolio 또는 프로그램을 지정하지 않으면 새 프로젝트가 생성되고 **[!UICONTROL 프로젝트 소유]** 로그인한 사용자 목록 [!DNL Workfront] 변환 전: [!DNL Salesforce]. 사용자는 새 프로젝트의 프로젝트 소유자입니다.

   1. 이름 입력 시작 **[!UICONTROL 템플릿]** 새 [!DNL Workfront] 프로젝트를 선택한 다음 목록에 있으면 선택합니다.

      필수 필드입니다.

      >[!NOTE]
      >
      >이 통합에 사용할 템플릿에 템플릿 소유자를 지정한 경우 해당 템플릿 소유자가 새 프로젝트의 프로젝트 소유자가 됩니다. 새 프로젝트는 **[!UICONTROL 프로젝트 소유]** 템플릿에 따라 새 프로젝트의 소유자인 사용자 목록입니다.
   ![salesforce_triggers_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   [!DNL Workfront] 이제 트리거가 충족될 때마다 프로젝트가 생성됩니다.

### 프로젝트 이름 이해 {#understanding-project-names}

생성된 프로젝트에 대한 트리거에 따라 프로젝트의 이름 [!DNL Workfront] 다음 패턴 중 하나를 따를 수 있습니다.

* Opportunity 또는 Account Trigger를 기반으로 프로젝트를 생성하는 경우 프로젝트의 이름은 다음과 같습니다. *`<Salesforce object name>`: `<Project template name>` (사용 시) [!DNL Salesforce])*.
* 새 제품의 추가도 포함하는 기회 트리거를 기반으로 프로젝트를 생성하는 경우 프로젝트의 이름은 다음과 같습니다. *`<Salesforce object name>`: `<Salesforce product name>` (사용 시) [!DNL Salesforce])*.

## 보기 [!DNL Workfront] 프로젝트

만약 [!DNL Workfront] 관리자가 추가됨 [!DNL Workfront] 섹션에 대한 섹션을 참조하십시오. [!UICONTROL 기회] 또는 계정 페이지 레이아웃에서 자동으로 만든 프로젝트를 볼 수 있습니다. [!UICONTROL 프로젝트] 이 섹션의 탭입니다.\
추가 정보에 대한 자세한 정보 [!DNL Workfront] 섹션에 있는 페이지의 [!UICONTROL 기회] 또는 계정 은(는) [구성 [!DNL Adobe Workfront] 섹션 [!DNL Salesforce] 사용자](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

다음을 수행해야 합니다. [!DNL Workfront] 계정 및에 로그인 [!DNL Workfront] 를 클릭하여 [!UICONTROL 프로젝트] 탭.

에서 생성된 프로젝트를 보려면 [!UICONTROL 기회] 또는 계정 :

1. 로 이동 [!UICONTROL 기회] 또는 계정 을 참조하십시오.
1. 로 이동합니다. **[!DNL Workfront]** 섹션을 참조하십시오.

   >[!NOTE]
   >
   >사용자의 [!DNL Workfront] 관리자가 이 섹션을 구성했는데 다른 이름이 있을 수 있습니다.

1. 을(를) 선택합니다 **[!UICONTROL 프로젝트]** 탭.

   정의된 트리거로 만든 모든 프로젝트가 이 탭에 나열됩니다. 의 모든 사용자 [!DNL Salesforce] 또한 [!DNL Workfront] 계정 및 액세스 권한이 있는 사람이 [!DNL Workfront] 또한 이러한 기능이 [!DNL Salesforce] 대상 [!UICONTROL 기회] 또는 생성한 계정입니다.

   ![[!DNL salesforce_projects_tab_with_projects_listed].png](assets/salesforce-projects-tab-with-projects-listed-350x150.png)

   통합에서 만든 프로젝트에 대한 다음 정보를 볼 수 있습니다.

   * 프로젝트 이름
   * 참조 번호
   * 시작 날짜
   * 소유자의 이름
   * 상태
   * 상황
   * 계획된 완료 일자
   * 완료율

      이 정보는에서 업데이트됩니다. [!DNL Workfront], 이 목록에서 업데이트된 필드를 확인할 수 있습니다.

1. (선택 사항) 프로젝트 이름을 클릭하여 Workfront에서 엽니다.
1. (선택 사항) [!UICONTROL **[!UICONTROL Salesforce로 이동]**] 에서 [!UICONTROL 프로젝트 세부 사항] 영역에 액세스할 수 있는 프로젝트 헤더 [!UICONTROL 기회] 또는 프로젝트가 시작된 계정입니다. 시스템 또는 그룹 관리자가 [!UICONTROL 통합] 필드를 레이아웃 템플릿에 추가하여 프로젝트 헤더에서 찾을 수 있습니다.

   >[!NOTE]
   >
   >다음 [!UICONTROL Salesforce로 이동] 링크가 모두 표시됩니다 [!DNL Workfront] 프로젝트를 볼 수 있는 사용자입니다. 다음을 수행해야 합니다. [!DNL Salesforce] 이(가) [!DNL Salesforce] 프로젝트가 생성된 Opportunity 또는 Account
