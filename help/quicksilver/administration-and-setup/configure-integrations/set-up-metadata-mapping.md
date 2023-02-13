---
title: 메타데이터 매핑 설정
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 메타데이터는 문서와 관련된 설명 정보입니다. 다음을 설정할 수 있습니다 [!DNL Adobe Workfront] 에 전송된 문서에 메타데이터를 포함합니다. [!DNL Workfront] 응용 프로그램.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# 메타데이터 매핑 설정

메타데이터는 문서와 관련된 설명 정보입니다. 다음을 설정할 수 있습니다 [!DNL Adobe Workfront] 에 전송된 문서에 메타데이터를 포함합니다. [!DNL Workfront] 응용 프로그램.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 정보 [!DNL Workfront] 메타데이터

의 문서에 대한 메타데이터 [!DNL Workfront] 관련 프로젝트명, 태스크 설명 또는 계획 완료 일자와 같은 정보를 포함할 수 있습니다. 로서의 [!DNL Workfront] 관리자, 구성 [!DNL Workfront] 에서 보낸 문서에 메타데이터를 포함합니다. [!DNL Workfront] 아래와 같이 변경하는 것을 의미합니다 [!DNL Workfront] 애플리케이션:

* [!DNL Workfront DAM]

문서와 함께 메타데이터를 전송하려면 먼저 포함할 메타데이터를 지정하거나 매핑해야 합니다. 에 사용되는 모든 필드를 매핑할 수 있습니다 [!DNL Workfront]. 메타데이터 매핑을 설정하면 업로드된 모든 문서가 [!DNL Workfront] 응용 프로그램에 매핑된 메타데이터가 포함됩니다.

사용자가 [!DNL Workfront] 변환 후 [!DNL Workfront] 응용 프로그램에서 매핑된 메타데이터는 문서에 따라 전송됩니다. 반면에 [!DNL Workfront] 응용 프로그램이 [!DNL Workfront]의 문서 메타데이터에 대한 변경 사항 [!DNL Workfront] 에서는 문서의 메타데이터에 반영되지 않습니다 [!DNL Workfront] 응용 프로그램. 에 매핑된 필드가 있는 경우 [!DNL Workfront] 이(가) 변경된 경우 업데이트된 메타데이터가 있는 문서의 새 버전을 [!DNL Workfront] 응용 프로그램.

>[!NOTE]
>
>메타데이터는 한 방향으로만 매핑할 수 있습니다. 변환 전: [!DNL Workfront] to [!DNL Workfront DAM]. 에 연결된 문서의 메타데이터 [!DNL Workfront] 변환 전: [!DNL Workfront DAM] Workfront으로 전송할 수 없습니다.

동일한 [!DNL Workfront] 의 다양한 메타데이터 필드에 필드를 추가합니다. [!DNL Workfront DAM]그러나 여러 애플리케이션에 대해서는 메타데이터 필드를 사용할 수 없습니다 [!DNL Workfront] 메타데이터 필드.

여러 항목을 구성하려면 [!DNL Workfront] 의 한 메타데이터 필드로 내보낼 필드 [!DNL Workfront] 먼저 애플리케이션에서 계산된 사용자 지정 필드를 만듭니다. [!DNL Workfront] 개체의 모든 개별 사용자 지정 필드를 표시합니다. 그런 다음 계산된 지표를 매핑합니다 [!DNL Workfront] 필드의 메타데이터 필드를 [!DNL Workfront] 응용 프로그램. 계산된 사용자 지정 필드에 대한 자세한 내용은 [사용자 지정 양식에 계산된 데이터 추가](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

메타데이터 매핑 프로세스에 대한 필드를 매핑하려면 먼저, [!DNL Workfront]. 자세한 내용은 [문서 통합 구성](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## 구성 [!DNL Workfront] 메타데이터 보내기

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 메타데이터 매핑]**.

   ![](assets/metadata-mapping.png)

1. 에서 **[!UICONTROL 매핑할 소스 필드 선택]** 상자에서 매핑할 Workfront 필드의 이름을 입력합니다 [!DNL Workfront DAM]그런 다음 목록에 표시되면 선택합니다.
1. 에서 **[!UICONTROL 매핑할 Target 필드 선택]** 상자에서 선택한 항목의 정보로 채울 필드를 선택합니다 [!DNL Workfront] 필드.

1. 클릭 **[!UICONTROL 매핑 추가]**.

   매핑된 필드는 페이지 하단에 나열된 매핑된 필드에 표시됩니다.

1. 원하는 모든 것을 추가할 때까지 5단계와 6단계를 반복합니다 [!DNL Workfront] 필드 및 해당 [!DNL Workfront DAM] 필드.

## 매핑된 필드 삭제

1. 에 로그인합니다. [!DNL Workfront] 관리자로.
1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 메타데이터 매핑]**.

1. 매핑된 필드 목록의 메타데이터 매핑에서 제거할 필드를 선택합니다.
1. 클릭 **[!UICONTROL 삭제]**.

   지정된 필드가 더 이상 매핑되지 않습니다. 이제 사용자가 [!DNL Workfront] to [!DNL Workfront DAM]를 반환하면 삭제된 필드 내에 포함된 메타데이터는 문서와 함께 전송되지 않습니다.

   매핑된 필드를 삭제하기 전에 보낸 문서는 삭제된 필드의 메타데이터를 포함하여 이와 함께 보낸 원래 메타데이터를 유지합니다.
