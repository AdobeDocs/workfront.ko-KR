---
title: 메타데이터 매핑 설정
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 메타데이터는 문서와 관련된 설명 정보입니다.  [!DNL Workfront] 응용 프로그램으로 보낸 문서에 메타데이터를 포함하도록  [!DNL Adobe Workfront] 을(를) 설정할 수 있습니다.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 1%

---

# 메타데이터 매핑 설정

메타데이터는 문서와 관련된 설명 정보입니다. [!DNL Workfront] 응용 프로그램으로 보낸 문서에 메타데이터를 포함하도록 [!DNL Adobe Workfront]을(를) 설정할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다. 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!DNL Workfront]개 메타데이터 정보

[!DNL Workfront]의 문서에 대한 메타데이터에는 관련 프로젝트 이름, 작업 설명 또는 계획된 완료 날짜와 같은 정보가 포함될 수 있습니다. [!DNL Workfront] 관리자는 [!DNL Workfront]에서 다음 [!DNL Workfront]개의 응용 프로그램으로 보낸 문서에 메타데이터를 포함하도록 [!DNL Workfront]을(를) 구성할 수 있습니다.

* [!DNL Workfront DAM]

문서를 사용하여 메타데이터를 전송하려면 먼저 포함할 메타데이터를 지정하거나 매핑해야 합니다. [!DNL Workfront]에서 사용되는 모든 필드를 매핑할 수 있습니다. 메타데이터 매핑을 설정하면 [!DNL Workfront] 응용 프로그램에 업로드된 모든 문서에 매핑된 메타데이터가 포함됩니다.

사용자가 [!DNL Workfront]에서 [!DNL Workfront] 응용 프로그램으로 문서를 보낼 때 매핑된 메타데이터가 문서와 함께 전송됩니다. [!DNL Workfront] 응용 프로그램의 문서 버전이 [!DNL Workfront]에 연결되어 있지만 [!DNL Workfront]에서 문서의 메타데이터에 대한 변경 내용은 [!DNL Workfront] 응용 프로그램의 문서 메타데이터에 반영되지 않습니다. [!DNL Workfront]의 매핑된 필드가 변경된 경우 업데이트된 메타데이터가 포함된 새 버전의 문서를 [!DNL Workfront] 응용 프로그램으로 보내야 합니다.

>[!NOTE]
>
>메타데이터는 [!DNL Workfront]에서 [!DNL Workfront DAM] 방향으로만 매핑할 수 있습니다. [!DNL Workfront DAM]에서 [!DNL Workfront]에 연결된 문서의 메타데이터를 Workfront으로 전송할 수 없습니다.

동일한 [!DNL Workfront] 필드를 [!DNL Workfront DAM]의 다양한 메타데이터 필드에 매핑할 수 있지만 여러 [!DNL Workfront] 메타데이터 필드에 대해 이들 응용 프로그램에서 메타데이터 필드를 사용할 수는 없습니다.

[!DNL Workfront] 응용 프로그램의 한 메타데이터 필드로 내보내도록 여러 [!DNL Workfront] 필드를 구성하려면 먼저 [!DNL Workfront]에서 계산된 사용자 정의 필드를 만들어 개체의 모든 개별 사용자 정의 필드를 표시합니다. 그런 다음 계산된 [!DNL Workfront] 필드를 [!DNL Workfront] 응용 프로그램의 메타데이터 필드에 매핑합니다. 계산된 사용자 지정 필드에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

메타데이터 매핑 프로세스에 대한 필드를 매핑하려면 먼저 [!DNL Workfront]에서 응용 프로그램을 활성화해야 합니다. 자세한 내용은 [문서 통합 구성](../../administration-and-setup/configure-integrations/configure-document-integrations.md)을 참조하십시오.

## 메타데이터를 보내도록 [!DNL Workfront] 구성

1. [!DNL Adobe Workfront]의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png)을 클릭합니다.

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 메타데이터 매핑]**&#x200B;을 클릭합니다.

   ![](assets/metadata-mapping.png)

1. **[!UICONTROL 매핑을 위한 Source 필드 선택]** 상자에서 [!DNL Workfront DAM]에 매핑할 Workfront 필드의 이름을 입력한 다음 목록에 표시되면 선택합니다.
1. **[!UICONTROL 매핑할 대상 필드 선택]** 상자에서 선택한 [!DNL Workfront] 필드의 정보로 채울 필드를 선택합니다.

1. **[!UICONTROL 매핑 추가]**&#x200B;를 클릭합니다.

   매핑된 필드는 페이지 하단에 나열된 매핑된 필드에 표시됩니다.

1. 원하는 [!DNL Workfront] 필드와 해당 [!DNL Workfront DAM] 필드를 모두 추가할 때까지 5단계와 6단계를 반복합니다.

## 매핑된 필드 삭제

1. [!DNL Workfront]에 관리자로 로그인합니다.
1. [!DNL Adobe Workfront]의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png)을 클릭합니다.

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 메타데이터 매핑]**&#x200B;을 클릭합니다.

1. 매핑된 필드 목록에서 메타데이터 매핑에서 제거할 필드를 선택합니다.
1. **[!UICONTROL 삭제]**&#x200B;를 클릭합니다.

   지정된 필드가 더 이상 매핑되지 않습니다. 이제 사용자가 [!DNL Workfront]에서 [!DNL Workfront DAM](으)로 문서를 보낼 때 삭제된 필드에 포함된 메타데이터는 문서와 함께 전송되지 않습니다.

   매핑된 필드를 삭제하기 전에 전송된 문서에는 삭제된 필드의 메타데이터를 포함하여 함께 전송된 원본 메타데이터가 유지됩니다.
