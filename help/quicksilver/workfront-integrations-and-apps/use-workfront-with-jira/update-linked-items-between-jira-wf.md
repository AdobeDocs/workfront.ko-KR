---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: ' [!DNL Jira] 에서 [!DNL Adobe Workfront] 사이의 연결된 항목 업데이트'
description: ' [!DNL Jira] 문제를  [!DNL Adobe Workfront] 작업 또는 문제에 연결하면 사용자는 한 응용 프로그램에서 항목을 업데이트할 수 있으며 해당 항목의 상대도 두 번째 응용 프로그램에서 작업하는 사용자에 대해 업데이트됩니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '1657'
ht-degree: 0%

---

# [!DNL Jira]에서 [!DNL Adobe Workfront] 사이의 연결된 항목 업데이트

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 Jira용 Workfront 통합을 사용할 수 없습니다.
>
>Jira와 조직의 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Jira용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Jira 소프트웨어 모듈](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)을 참조하십시오.

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

[!DNL Jira] 문제를 [!DNL Adobe Workfront] 작업 또는 문제에 연결하면 사용자가 한 응용 프로그램에서 항목을 업데이트할 수 있으며 해당 항목의 상대가 두 번째 응용 프로그램에서 작업 중인 사용자에 대해서도 업데이트됩니다.

[!DNL Workfront]과(와) [!DNL Jira] 사이의 항목 연결에 대한 자세한 내용은 [Adobe Workfront과(와) Jira 사이의 항목 연결](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md)을 참조하십시오.

[!DNL Workfront]에 대해 [!DNL Jira]을(를) 설정할 때 [!DNL Jira] 시스템 관리자는 한 응용 프로그램에서 특정 필드를 구성하여 다른 응용 프로그램에서 연결된 항목의 필드와 동기화할 수 있습니다.

연결된 [!DNL Jira]개 항목과 [!DNL Workfront]개 항목 간의 필드 동기화에 대한 자세한 내용은 [구성 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>임의</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준 </p>
       <p>플랜 </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira 액세스</td> 
   <td> <p>시스템 관리자 액세스</p> <p>중요: 사용자에게 첨부할 수 있는 기존 계정을 사용하는 대신 Jira 및 Workfront에서 별도의 시스템 관리자 계정을 만들어 이 통합 전용을 하는 것이 좋습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

[!DNL Workfront]에서 [!DNL Jira] 사이의 항목을 연결하려면 먼저 다음을 수행해야 합니다.

* [!DNL Workfront for Jira] 설치.

  [!DNL Workfront for Jira] 설치에 대한 지침은 [설치 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)를 참조하십시오.

* [!DNL Workfront for Jira] 구성.

  [!DNL Workfront for Jira] 구성에 대한 지침은 [구성 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)을 참조하십시오.

* [!DNL Workfront]과(와) [!DNL Jira] 사이의 항목을 연결합니다.

  자세한 내용은 [다음 항목 연결 [!DNL Adobe Workfront] 과(와) [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md)을 참조하세요.

## [!DNL Workfront]에서 연결된 항목 업데이트

주로 [!DNL Workfront]에서 작업하는 경우 [!DNL Workfront]에서 작업 항목을 업데이트할 수 있으며 [!DNL Jira]의 해당 항목도 업데이트할 수 있습니다. 이 업데이트는 [!DNL Workfront] 라이선스가 필요 없는 [!DNL Jira]에 대한 [!DNL Jira]의 통합을 통해 이루어집니다.

[!DNL Workfront] 관리자가 연결된 항목 간의 필드를 동기화하도록 [!DNL Workfront for Jira]을(를) 구성한 한, [!DNL Workfront]에서 업데이트하는 특정 필드도 연결된 [!DNL Jira] 문제에 대해 업데이트됩니다. [!DNL Workfront]에서 항목을 업데이트하는 방법에 대한 자세한 내용은 [문제 편집](../../manage-work/issues/manage-issues/edit-issues.md) 및 [작업 편집](../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하십시오.

다음 목록은 연결된 항목의 [!DNL Workfront] 필드와 동기화하는 [!DNL Jira] 필드를 보여줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>업데이트된 [!DNL Workfront] 필드</strong> </th> 
   <th><strong>동기화된 [!DNL Jira] 필드/ 업데이트</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 문제 또는 작업 이름]</td> 
   <td> <p>[!UICONTROL 문제 이름]</p> <p>이름 변경에 대한 댓글이 <strong>[!DNL Workfront]</strong> 문제의 [!DNL Jira] 탭에 추가됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문제 또는 작업 설명]</td> 
   <td> <p> [!UICONTROL 문제 설명]</p> <p>업데이트된 설명에 대한 댓글이 <strong>[!DNL Workfront]</strong> 문제의 [!DNL Jira] 탭에 추가됩니다.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL 업로드된 문서]</p> <p>참고: 외부 서버의 [!DNL Workfront] 항목에 연결된 문서는 [!DNL Jira] 문제로 전송되지 않습니다. [!DNL Workfront]개 항목에 직접 업로드된 문서만 연결된 [!DNL Jira] 문제로 업데이트됩니다. </p> </td> 
   <td> <p>[!UICONTROL 첨부 파일]</p> <p>업로드한 첨부 파일에 대한 댓글이 <strong>[!DNL Workfront]</strong> 문제의 [!DNL Jira] 탭에 추가됩니다.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 완료 일자]</td> 
   <td> <p>[!UICONTROL 기한]</p> <p>변경된 [!UICONTROL 기한]에 대한 댓글이 [!DNL Workfront] 문제의 [!DNL Jira] 탭에 추가됩니다. </p> <p>참고: [!UICONTROL Jira]에서 업데이트된 이 필드를 보려면 <strong> 문제에 대해 </strong>[!UICONTROL 기한]&#x200B;[!DNL Jira]을(를) 활성화해야 합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>사용자 지정 Forms 및 사용자 지정 필드</td> 
   <td> <p> [!DNL Workfront] 문제의 [!DNL Jira] 오른쪽 패널에 표시합니다. <br>실제 값이 있는 사용자 지정 필드만 패널에 표시됩니다.<br></p> <p>참고: 사용자 정의 양식 섹션은 [!DNL Workfront] 관리자의 액세스 수준으로 표시됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문제 또는 작업 우선 순위]</td> 
   <td>[!DNL Workfront] 문제의 [!DNL Jira] 오른쪽 패널에 표시됩니다. <br>문제 <strong>의 </strong>[!UICONTROL 우선 순위]&#x200B;[!DNL Jira] 필드를 업데이트하지 않습니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log Time] </td> 
   <td> <p>기록된 시간에 대한 댓글이 <strong>[!DNL Workfront]</strong> 문제의 [!DNL Jira] 탭에 추가됩니다. 여기에는 시간을 기록한 사용자의 이름과 시간이 다른 경우 기록된 사용자가 포함됩니다. <strong>의 </strong>[!UICONTROL 작업 로그]&#x200B;[!DNL Jira] 탭에 기록된 시간이 없습니다.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>댓글이 <strong>[!DNL Workfront]</strong> 문제의 [!DNL Jira] 탭에 추가됩니다. <strong> 문제의 </strong>[!UICONTROL Comments]&#x200B;[!DNL Jira] 탭에 추가되지 않았습니다.</p> <p>참고: 두 개의 기존 항목을 수동으로 연결할 때 [!DNL Workfront]에 연결하기 전에 [!DNL Jira] 항목에 추가된 댓글은 [!DNL Jira] 문제와 동기화되지 않습니다. </p> <p>Jira 주석은 Workfront과 동기화됩니다.</td> 
  </tr> 
 </tbody> 
</table>

## [!DNL Jira]에서 연결된 항목 업데이트

주로 [!DNL Jira]에서 작업하는 경우 [!DNL Jira]에서 작업 항목을 업데이트할 수 있으며 [!DNL Workfront]의 해당 항목도 업데이트할 수 있습니다. [!DNL Workfront]에서 업데이트한 내용을 받기 위해 [!DNL Workfront] 문제와 연결된 [!DNL Jira] 항목에 대해 [!DNL Jira] 라이선스를 가지고 있지 않아도 됩니다.

[!DNL Workfront] 관리자가 연결된 항목 간의 필드를 동기화하도록 [!DNL Workfront]에 대해 [!DNL Jira]을(를) 구성한 경우 [!DNL Jira]에서 업데이트하는 특정 필드도 연결된 [!DNL Workfront] 항목에 대해 업데이트됩니다.

다음 목록은 연결된 항목의 [!DNL Jira] 필드와 동기화하는 [!DNL Workfront] 필드를 보여줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>업데이트된 [!DNL Jira] 필드</strong> </th> 
   <th><strong>동기화된 [!DNL Workfront] 필드/업데이트</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 문제 상태]</td> 
   <td> <p> [!UICONTROL 문제 또는 작업 상태]</p> <p>[!DNL Jira]의 문제 상태가 Workfront의 다음 상태 또는 다음 상태와 동일한 상태와 동기화됩니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL 진행 중] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>참고: [!DNL Jira] 상태는 적절한 상태와 일치하는 첫 번째 [!DNL Workfront] 상태와 동기화됩니다.</p> <p>[!DNL Workfront]에 있는 항목의 상태에 대한 자세한 내용은 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">상태 만들기 또는 편집</a>을 참조하세요.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL 문제 첨부 파일]</td> 
   <td> [!UICONTROL 문제 또는 작업 문서]<br>[!DNL Jira]의 새 문서 업로드에 대한 댓글이 [!DNL Workfront] 문제 또는 작업의 [!UICONTROL 업데이트] 탭에 추가됩니다.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기한]</td> 
   <td> <p> [!DNL Jira]의 [!UICONTROL 기한] 변경에 대한 댓글이 [!DNL Workfront] 문제 또는 작업의 [!UICONTROL 업데이트] 탭에 추가됩니다. </p> <p>참고: [!DNL Workfront] 문제 또는 작업에 대한 날짜가 변경되지 않습니다. </p> </td> 
  </tr> 
  <tr> 
   <td> [!DNL Workfront] 오른쪽 패널 또는 [!DNL Jira] 문제의 [!UICONTROL 기타] 메뉴에 시간을 기록하십시오.<br></td> 
   <td> <p>Hours<br>연결된 [!DNL Workfront] 항목에 Jira에 기록된 시간을 추가하는 것 외에도 [!DNL Workfront] 항목의 [!UICONTROL Updates] 탭에 로깅 시간에 대한 댓글이 추가됩니다.</p> <p>[!DNL Jira]에서 시간을 기록하는 [!DNL Jira] 사용자를 업데이트하는 등 연결된 [!DNL Workfront] 문제에 대한 시간 로깅에 대한 자세한 내용은 <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">연결된 [!DNL Jira] 및 [!DNL Workfront]개 항목에 대한 시간 기록</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td> 댓글 <br><br></td> 
   <td> <p>[!UICONTROL Setup] 탭의 [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] 섹션에서 [!DNL Workfront]&#x200B;[!UICONTROL Comments]<strong> 설정이 </strong>[!UICONTROL Always]<strong>인 경우 </strong> 문제 또는 작업의 [!UICONTROL Updates] 탭에 댓글이 추가됩니다.</p> <p>[!DNL Jira]에서 Workfront 설정을 구성하는 방법에 대한 자세한 내용은 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">구성 [!DNL Workfront for Jira]</a>을(를) 참조하십시오.</p> <p>연결된 [!DNL Jira] 문제의 항목에 대한 댓글에 대한 자세한 내용은 <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">연결된 [!DNL Jira] 문제의 댓글</a>을 참조하세요.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 연결된 [!DNL Jira] 문제의 로그 시간

[!DNL Jira]에서 시간을 기록한 위치에 관계없이 [!DNL Jira]에서 [!DNL Workfront] 항목에 대해 기록한 시간도 연결된 [!DNL Jira] 항목으로 전송됩니다.\
[!DNL Workfront] 패널의 Jira에 시간을 기록할 때 시간은 [!DNL Workfront]에만 기록됩니다.\
[!DNL Workfront]에 기록한 시간은 [!DNL Jira]에 연결된 문제의 시간에 영향을 주지 않습니다.

>[!NOTE]
>
>시간이 [!DNL Jira] 작업에 연결된 [!DNL Workfront] 항목에 추가된 경우 [!UICONTROL 의 &#x200B;]시간 유형[!DNL Workfront]은(는) [!UICONTROL 작업 시간]입니다. 시간이 [!DNL Jira] 문제와 연결된 [!DNL Workfront] 항목에 추가된 경우 [!UICONTROL 의 &#x200B;]시간 유형[!DNL Workfront]은(는) [!UICONTROL 문제 시간]입니다.

시간 로깅을 기록하려면 **[!DNL Workfront]**&#x200B;의 [!DNL Jira] 탭과 **[!UICONTROL 의 항목의]**&#x200B;업데이트[!DNL Workfront] 탭에 댓글이 추가됩니다.\
시간은 **[!UICONTROL 항목의]**&#x200B;시간[!DNL Workfront] 탭에도 표시됩니다.

* [연결된 항목 [!DNL Jira] 및 [!DNL Workfront] 항목에 대한 로그 시간](#log-time-for-linked-jira-and-workfront-items)
* [&#x200B; [!DNL Jira] 부터  [!DNL Workfront] 항목까지 시간 기록](#log-time-from-jira-to-a-workfront-item)

### 연결된 [!DNL Jira] 및 [!DNL Workfront]개 항목에 대한 로그 시간

[!DNL Jira] 항목에 연결된 [!DNL Workfront] 문제의 시간을 기록할 수 있으며, 시간은 [!DNL Jira] 문제와 [!DNL Workfront] 항목에 모두 기록됩니다.

>[!IMPORTANT]
>
>[!DNL Jira]의 시간을 기록하는 사용자가 [!DNL Workfront]에 없는 경우 **[!UICONTROL 사용자에게 [!DNL Workfront] [!DNL Jira] 계정이 없는 &#x200B; 경우 *자동으로 [!DNL Workfront]에 사용자를 만듭니다]**&#x200B;이(가)**[!UICONTROL &#x200B; Always &#x200B;]**(으)로 설정되어 있는 경우&#x200B; 통합에서 Workfront에 새 활성 사용자를 만듭니다. 이 사용자는 [!DNL Workfront] 라이선스를 사용하지 않습니다. [!DNL Workfront]의 작업 항목에 활성 사용자를 할당할 수 있지만 업데이트에 포함할 수 없습니다. [!DNL Workfront]에서 [!DNL Jira]명의 사용자를 자동으로 만드는 구성에 대한 자세한 내용은 [구성 [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)을 참조하십시오.

[!DNL Jira]에 항목의 시간을 기록하여 [!DNL Jira] 및 [!DNL Workfront]에 모두 기록하려면 다음을 수행합니다.

1. [!DNL Jira]에 로그인합니다.
1. [!DNL Jira] 항목에 연결된 [!DNL Workfront] 문제로 이동합니다.
1. **[!UICONTROL 자세히]** 메뉴를 확장하고 **[!UICONTROL 작업 기록]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 체류 시간]** 필드에 이 문제에 대해 작업하는 데 걸린 시간을 지정하십시오. 다음 기간을 사용하여 시간을 지정해야 합니다.

   * [!UICONTROL 주]&#x200B;(w)
   * [!UICONTROL 일]&#x200B;(일)
   * [!UICONTROL 시간]&#x200B;(시간)

1. **[!UICONTROL 작업 설명]**&#x200B;을 포함하여 시간 항목에 정보를 계속 추가한 다음 **[!UICONTROL 로그]**&#x200B;를 클릭합니다.\
   시간은 **[!UICONTROL 항목의]**&#x200B;작업 로그[!DNL Jira] 탭과 연결된 [!DNL Workfront] 항목에 추가됩니다.\
   시간 항목에 대한 작업 설명이 [!DNL Workfront]의 시간 항목에 메모로 기록됩니다.

### [!DNL Jira]에서 [!DNL Workfront] 항목에 시간을 기록합니다.

이 시간을 [!DNL Workfront] 문제에 기록하지 않고 [!DNL Jira] 문제의 연결된 [!DNL Jira] 항목에 시간을 기록할 수 있습니다.

1. [!DNL Jira]에 로그인합니다.
1. [!DNL Jira] 항목에 연결된 [!DNL Workfront] 문제로 이동합니다.

   [!DNL Workfront] 항목에 대한 세부 정보가 문제의 [!DNL Workfront] 오른쪽 패널에 표시됩니다.

1. **[!UICONTROL 로그 시간]** 아이콘을 클릭합니다.

1. 문제에 대해 기록할 **[!UICONTROL 시간]**&#x200B;과(와) **[!UICONTROL 분]**&#x200B;의 양을 지정하십시오.

1. **[!UICONTROL 로그 시간]**&#x200B;을 클릭합니다.

   시간이 [!DNL Workfront] 항목에 추가됩니다.

   이 시간은 [!UICONTROL &#x200B; 문제의 &#x200B;]작업 로그[!DNL Jira] 탭에 추가되지 않습니다.

## 연결된 [!DNL Jira] 문제의 댓글 {#comment-from-a-linked-jira-issue}

[!DNL Jira]의 [!DNL Workfront] 오른쪽 패널에서 [!DNL Jira] 항목에 댓글을 달면 해당 댓글은 Workfront에 있는 연결된 항목의 [!UICONTROL 업데이트] 탭에도 추가됩니다.

[!DNL Jira]에서 [!DNL Workfront] 항목에 댓글을 달려면:

1. [!DNL Jira]에 로그인합니다.
1. [!DNL Jira] 항목에 연결된 [!DNL Workfront] 문제로 이동합니다.

   [!DNL Workfront] 항목에 대한 세부 정보가 문제의 [!DNL Workfront] 오른쪽 패널에 표시됩니다.

1. **[!UICONTROL 패널 또는]**&#x200B;설명[!DNL Workfront] 탭에서 **[!UICONTROL 설명]** 아이콘을 클릭합니다.

1. 댓글을 입력한 다음 **[!UICONTROL 보내기]**&#x200B;를 클릭합니다.

   주석이 다음에 추가됩니다.

   * **[!DNL Workfront]** 문제의 [!DNL Jira] 탭입니다.
   * **[!UICONTROL 문제의]**&#x200B;댓글[!DNL Jira] 탭입니다.
   * Workfront에서 연결된 항목의 **[!UICONTROL 업데이트]** 탭입니다.
