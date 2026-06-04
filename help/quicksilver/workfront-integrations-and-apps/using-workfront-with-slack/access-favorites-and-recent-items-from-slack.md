---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: ' [!DNL Slack]에서 즐겨찾기 및 최근 항목에 액세스'
description: Slack용  [!DNL Adobe Workfront] 을(를) 설치 및 구성한 후에는 Workfront 즐겨찾기 및 최근 항목을 보고 Slack의 목록에 있는 항목에 액세스할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4bf62192-66fe-42a7-b8c0-23b7bdef45e8
TQID: https://experienceleague.adobe.com/Fqy-Tqgyza2C4STR6qD78-HsyKDiydUM1NTnzLY1-FE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 323
ht-degree: 6%

---

# [!DNL Slack]에서 즐겨찾기 및 최근 항목에 액세스

[!DNL Adobe Workfront for Slack]을(를) 설치 및 구성한 후에는 [!UICONTROL Workfront] 즐겨찾기 및 최근 항목을 보고 [!DNL Slack]의 목록에서 항목에 액세스할 수 있습니다.

[!DNL Workfront with Slack] 구성에 대한 자세한 내용은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>Any</p>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL Slack]에서 즐겨찾기 및 최근 항목에 액세스하려면 먼저 다음을 수행해야 합니다.

* 구성 [!DNL Workfront for Slack]\
   [!DNL Workfront for Slack] 구성에 대한 지침은 [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)을 참조하십시오.

## [!DNL Slack]에서 [!UICONTROL 즐겨찾기] 목록에 액세스

1. [!DNL Slack] 인스턴스에 로그인하고 [!DNL Slack]에서 [!DNL Workfront]에 로그인합니다.\
   [!DNL Slack]에서 [!DNL Workfront]에 로그인하는 방법에 대한 자세한 내용은 [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)의 &quot;[!DNL Slack]에서 [!DNL Workfront]에 로그인&quot; 섹션을 참조하십시오.

1. 모든 채널에서 [!UICONTROL message] 필드에 다음 명령을 입력하십시오. `/workfront favorites`

   >[!NOTE]
   >
   >명령은 대/소문자를 구분합니다. `/workfront` 대신 `/wf`(으)로 명령을 시작할 수 있습니다.

   즐겨찾기 목록이 표시됩니다.

1. (선택 사항) 더 많은 즐겨찾기를 나열하려면 **[!UICONTROL 자세히 표시]**&#x200B;를 클릭합니다.
1. 즐겨찾기의 이름을 클릭하여 새 브라우저 탭에서 [!DNL Workfront]에서 엽니다.

## [!DNL Slack]에서 최근 항목 목록에 액세스

1. [!DNL Slack] 인스턴스에 로그인하고 Slack에서 [!DNL Workfront]에 로그인합니다.\
   [!DNL Slack]에서 [!DNL Workfront]에 로그인하는 방법에 대한 자세한 내용은 [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)의 &quot;[!DNL Slack]에서 [!DNL Workfront]에 로그인&quot; 섹션을 참조하십시오.

1. 모든 채널에서 [!UICONTROL message] 필드에 다음 명령을 입력하십시오. `/workfront recent`

   >[!NOTE]
   >
   >명령은 대/소문자를 구분합니다. `/workfront` 대신 `/wf`(으)로 명령을 시작할 수 있습니다.

   최근 항목 목록은 마지막으로 액세스한 순서대로 표시되며 가장 최근 항목은 맨 위에 표시됩니다. 항목은 한 번에 세 개 나열되며 개체 유형별로 그룹화됩니다.\

1. (선택 사항) 최신 항목을 더 나열하려면 **[!UICONTROL 자세히 표시]**&#x200B;를 클릭합니다.
1. (선택 사항) 최근에 액세스한 항목의 이름을 클릭하여 [!DNL Workfront]에서 새 브라우저 탭에서 엽니다.
