---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 연결 개요
description: 대부분의 앱에서 연결을 만들어야 합니다. 연결을 통해 [!DNL Adobe Workfront Fusion] 은 특정 시나리오의 설정에 따라 지정된 서드파티 서비스와 통신할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 연결 개요

<!-- Audited: 3/2024-->

대부분의 앱의 경우 [!DNL Workfront Fusion] 특정 시나리오의 설정에 따라 지정된 서드파티 서비스와 통신할 수 있는 연결이 필요합니다.

예를 들어, 다음 위치에서 정보를 검색하는 시나리오를 만들려는 경우 [!DNL Workfront], 다음에 대한 액세스 권한을 부여해야 합니다. [!DNL Workfront Fusion] 에 액세스 [!DNL Workfront] 계정입니다.

연결은 Fusion이 애플리케이션에 액세스하는 데 사용하는 권한 및 권한을 나타냅니다. 각 애플리케이션에 대해 하나 이상의 연결을 만들 수 있으며 여러 모듈 또는 시나리오에서 동일한 연결을 사용할 수 있습니다.

대부분의 연결은 단일 애플리케이션에 대해서만 사용됩니다. 예: [!DNL Workfront] 다음에서 연결을 사용할 수 없음: [!UICONTROL Salesforce] 모듈. 일부 [!DNL Adobe] 응용 프로그램은 연결을 공유할 수 있습니다. 자세한 내용은 다음 목록에 있는 해당 애플리케이션에 대한 문서를 참조하십시오. [앱 및 해당 모듈](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

연결은 팀 수준에서 관리됩니다. 팀의 모든 구성원은 팀의 연결에 액세스할 수 있으며 팀 외부의 사용자는 팀의 연결에 액세스할 수 없습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: [!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>레거시: 모두 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>신규:</p> <ul><li>[!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Workfront] 플랜: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] 플랜: [!DNL Workfront Fusion] 포함됩니다.</li></ul>
   <p>또는</p>
   <p>현재: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 액세스 권한

모든 연결에 대해 [!DNL Workfront Fusion] 은(는) 주어진 시나리오를 성공적으로 완료하는 데 필요한 액세스 권한만 필요로 합니다. 예를 들어 다음 위치의 문서를 나열할 시나리오를 만드는 경우 [!DNL Google Docs], [!DNL Workfront Fusion] 은 문서의 콘텐츠를 가져올 수 있는 권한을 요청하지 않습니다. 나중에 문서의 콘텐츠에 액세스해야 하는 경우 연결을 업데이트하거나 해당 콘텐츠에 액세스할 수 있는 새 연결을 만들 수 있습니다.

일부 서비스에서는 특정 작업에 대한 액세스를 제한할 수 없습니다. 이러한 경우, [!DNL Workfront Fusion] 은(는) 전체 액세스 권한이 있어야 합니다. 제한 방법에 대한 자세한 정보 [!DNL Workfront Fusion] 해당 서비스에 등록된 계정에 대한 액세스 권한은에 나열된 애플리케이션별 설명서를 참조하십시오. [앱 및 해당 모듈](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## 연결 관리

에서 모든 연결을 관리할 수 있습니다. [!UICONTROL 연결] 영역입니다.

>[!NOTE]
>
>연결은 팀에서 소유합니다. 찾고 있는 연결을 찾을 수 없는 경우 올바른 팀을 보고 있는지 확인하십시오.
>
>새 팀을 선택하려면 다음을 수행하십시오.
>
>* 왼쪽 탐색에서 팀 이름을 클릭하고 새 팀을 선택합니다.
>
>    또는
>
>* 왼쪽 탐색에서 팀 개요 를 클릭한 다음 페이지 상단 근처에 있는 팀 이름 옆에 있는 드롭다운 화살표를 클릭합니다. 새 팀을 선택하십시오.

1. 을(를) 열려면 [!UICONTROL 연결] 영역, 클릭 <b>[!UICONTROL 연결]</b> 왼쪽 탐색.
1. (선택 사항) 환경 및 유형 드롭다운을 클릭하고 옵션을 선택하여 연결 환경 및 유형을 나타냅니다.
1. (선택 사항) 제공된 권한을 보려면 [!DNL Workfront Fusion] 연결의 경우 보기 아이콘 을 클릭합니다 ![연결 권한 보기](assets/view-connection-permissions.png) 연결을 위한 것입니다.
1. (선택 사항) 연결 이름을 바꾸려면 연결 이름을 강조 표시하고 새 이름을 입력합니다.
1. (선택 사항) 연결을 재인증하려면 **재인증** 연결을 위한 것입니다.
1. (선택 사항) 연결을 삭제하려면 **삭제** 연결을 위한 것입니다.
1. (선택 사항) 서비스에 대한 연결이 성공적으로 설정되었는지 확인하려면 **확인** 연결용.



## 연결 갱신

[!DNL Workfront Fusion] 일반적으로 특정 서비스에 대한 액세스 권한을 무제한으로 가져옵니다. 일부 애플리케이션은 일정 기간 후에 액세스 권한을 갱신해야 합니다. 이러한 경우, [!DNL Workfront Fusion] 액세스 권한이 만료되기 직전에 이메일로 알립니다.

연결을 갱신하려면:

1. 다음을 클릭합니다. **[!UICONTROL 재인증]** 의 단추 **[!UICONTROL 연결]** 영역입니다.
