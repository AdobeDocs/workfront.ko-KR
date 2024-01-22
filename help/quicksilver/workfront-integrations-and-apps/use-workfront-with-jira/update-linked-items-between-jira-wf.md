---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: '다음 기간 동안 연결된 항목 업데이트: [!DNL Jira] 및 [!DNL Adobe Workfront]'
description: 연결할 때 [!DNL Jira] 문제 대상 [!DNL Adobe Workfront] 작업 또는 문제는 사용자가 한 응용 프로그램의 항목을 업데이트할 수 있으며 해당 항목의 상대 작업도 두 번째 응용 프로그램에서 작업하는 사용자를 위해 업데이트됩니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 0%

---

# 다음 기간 동안 연결된 항목 업데이트: [!DNL Jira] 및 [!DNL Adobe Workfront]

연결할 때 [!DNL Jira] 문제 대상 [!DNL Adobe Workfront] 작업 또는 문제는 사용자가 한 응용 프로그램의 항목을 업데이트할 수 있으며 해당 항목의 상대 작업도 두 번째 응용 프로그램에서 작업하는 사용자를 위해 업데이트됩니다.

항목 연결에 대한 자세한 내용 [!DNL Workfront] 및 [!DNL Jira], 참조 [Adobe Workfront과 Jira 간의 항목 연결](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

설정 시 [!DNL Workfront] 대상 [!DNL Jira], as a [!DNL Jira] 시스템 관리자는 한 응용 프로그램에서 특정 필드를 구성하여 다른 응용 프로그램에서 연결된 항목의 필드와 동기화할 수 있습니다.

연결된 필드 간의 필드 동기화에 대한 자세한 정보 [!DNL Jira] 및 [!DNL Workfront] 항목, 참조 [구성 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td><p>새로 만들기: 모두</p>
       <p>또는</p>
       <p>현재: [!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
       <p>또는</p>
       <p>현재: [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 액세스</td> 
   <td> <p>시스템 관리자 액세스</p> <p>중요:에서 별도의 시스템 관리자 계정을 만드는 것이 좋습니다. [!DNL Jira] 및 [!DNL Workfront] 사용자에게 첨부할 수 있는 기존 통합 대신 이 통합 전용.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음이어야 합니다: [!DNL Workfront] 관리자.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 전제 조건

다음 사이에 항목을 연결하기 전에 [!DNL Workfront] 및 [!DNL Jira], 다음을 수행해야 합니다.

* 설치 [!DNL Workfront for Jira].

  설치에 대한 지침 [!DNL Workfront for Jira], 참조 [설치 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* 구성 [!DNL Workfront for Jira].

  구성에 대한 지침 [!DNL Workfront for Jira], 참조 [구성 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* 다음 사이에 항목 연결 [!DNL Workfront] 및 [!DNL Jira].

  자세한 내용은 [다음 사이에 항목 연결 [!DNL Adobe Workfront] 및 [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## 에서 연결된 항목 업데이트 [!DNL Workfront]

주로 다음 위치에서 작업하는 경우 [!DNL Workfront]에서 작업 항목을 업데이트할 수 있습니다. [!DNL Workfront] 및 의 상대 [!DNL Jira] 업데이트도 참조하십시오. 이 업데이트는 의 통합을 통해 수행됩니다. [!DNL Workfront] 대상 [!DNL Jira] 를 사용할 필요가 없습니다. [!DNL Jira] 라이센스.

의 한 [!DNL Workfront] 관리자가 구성함 [!DNL Workfront for Jira] 연결된 항목 간의 필드를 동기화하려면 업데이트되는 특정 필드 [!DNL Workfront] 연결된 의 업데이트도 참조하십시오 [!DNL Jira] 문제. 항목 업데이트에 대한 자세한 내용 [!DNL Workfront], 참조 [문제 편집](../../manage-work/issues/manage-issues/edit-issues.md) 및 [작업 편집](../../manage-work/tasks/manage-tasks/edit-tasks.md).

다음 목록은 다음 중 하나를 [!DNL Workfront] 필드가 와 동기화 [!DNL Jira] 연결된 항목의 필드:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>업데이트됨 [!DNL Workfront] 필드</strong> </th> 
   <th><strong>동기화됨 [!DNL Jira] 필드/업데이트</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 문제 또는 작업 이름]</td> 
   <td> <p>[!UICONTROL 문제 이름]</p> <p>이름 변경에 대한 댓글이 <strong>[!DNL Workfront]</strong> 의 탭 [!DNL Jira] 문제. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문제 또는 작업 설명]</td> 
   <td> <p> [!UICONTROL 문제 설명]</p> <p>업데이트된 설명에 대한 댓글이 <strong>[!DNL Workfront]</strong> 의 탭 [!DNL Jira] 문제.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL 업로드된 문서]</p> <p>참고: 링크된 문서 [!DNL Workfront] 외부 서버의 항목이 (으)로 전송되지 않음 [!DNL Jira] 문제. 에 바로 업로드된 문서만 [!DNL Workfront] 또한 항목이 연결된 [!DNL Jira] 문제. </p> </td> 
   <td> <p>[!UICONTROL 첨부 파일]</p> <p>업로드된 첨부 파일에 대한 댓글이 <strong>[!DNL Workfront]</strong> 의 탭 [!DNL Jira] 문제.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 계획된 완료 일자]</td> 
   <td> <p>[!UICONTROL 기한]</p> <p>변경된 [!UICONTROL 기한]에 대한 댓글이 [!DNL Workfront] 의 탭 [!DNL Jira] 문제. </p> <p>참고: 다음을 활성화해야 합니다. <strong>[!UICONTROL 기한]</strong> 에 대한 [!DNL Jira] [!UICONTROL Jira]에서 이 필드를 업데이트할 수 없는 문제입니다. </p> </td> 
  </tr> 
  <tr> 
   <td>사용자 지정 Forms 및 사용자 지정 필드</td> 
   <td> <p> 에 표시 [!DNL Workfront] 의 오른쪽 패널 [!DNL Jira] 문제. <br>실제 값이 있는 사용자 정의 필드만 패널에 표시됩니다.<br></p> <p>참고: 사용자 정의 양식 섹션은 [!DNL Workfront] 관리자. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 문제 또는 작업 우선 순위]</td> 
   <td>에 표시 [!DNL Workfront] 의 오른쪽 패널 [!DNL Jira] 문제. <br>문제가 업데이트되지 않습니다 <strong>[!UICONTROL 우선 순위]</strong> 의 필드 [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log Time] </td> 
   <td> <p>기록된 시간에 대한 댓글이 <strong>[!DNL Workfront]</strong> 의 탭 [!DNL Jira] 문제. 여기에는 시간을 기록한 사용자의 이름과 시간이 다른 경우 기록된 사용자가 포함됩니다. 에 기록된 시간이 없습니다. <strong>[!UICONTROL 작업 로그]</strong> 의 탭 [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>주석이 다음에 추가됩니다. <strong>[!DNL Workfront]</strong> 의 탭 [!DNL Jira] 문제. 에 추가되지 않습니다. <strong>[!UICONTROL Comments]</strong> 의 탭 [!DNL Jira] 문제</p> <p>참고: 두 개의 기존 항목을 수동으로 연결할 때 [!DNL Workfront] 링크하기 전의 항목 [!DNL Jira] 을(를) (으)로 동기화하지 않음 [!DNL Jira] 문제. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 에서 연결된 항목 업데이트 [!DNL Jira]

주로 다음 위치에서 작업하는 경우 [!DNL Jira]에서 작업 항목을 업데이트할 수 있습니다. [!DNL Jira] 및 의 상대 [!DNL Workfront] 업데이트도 참조하십시오. 다음 작업을 수행하지 않아도 됩니다. [!DNL Workfront] 에 대한 라이센스 [!DNL Workfront] 에 연결된 항목 [!DNL Jira] 에서 수행하는 업데이트를 수신할 문제 [!DNL Jira].

다음을 조건으로 [!DNL Workfront] 관리자가 구성함 [!DNL Workfront] 대상 [!DNL Jira] 연결된 항목 간에 필드를 동기화하려면 업데이트되는 특정 필드 [!DNL Jira] 연결된 의 업데이트도 참조하십시오 [!DNL Workfront] 항목.

다음 목록은 다음 중 하나를 [!DNL Jira] 필드가 와 동기화 [!DNL Workfront] 연결된 항목의 필드:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>업데이트됨 [!DNL Jira] 필드</strong> </th> 
   <th><strong>동기화됨 [!DNL Workfront] 필드/업데이트</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 문제 상태]</td> 
   <td> <p> [!UICONTROL 문제 또는 작업 상태]</p> <p>의 문제 상태 [!DNL Jira] Workfront에서 다음 상태 또는 다음 상태와 동일한 상태와 동기화합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL New]([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL 진행 중] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>참고: [!DNL Jira] 상태와 첫 번째 동기화 [!DNL Workfront] 적절한 상태와 동등한 상태.</p> <p>의 항목 상태에 대한 자세한 정보 [!DNL Workfront], 참조 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">상태 만들기 또는 편집</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL 문제 첨부 파일]</td> 
   <td> [!UICONTROL 문제 또는 작업 문서]<br>에서 새 문서 업로드에 대한 댓글 [!DNL Jira] 의 [!UICONTROL 업데이트] 탭에 추가됩니다. [!DNL Workfront] 문제 또는 작업  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기한]</td> 
   <td> <p> 의 [!UICONTROL 기한] 변경에 대한 댓글 [!DNL Jira] 의 [!UICONTROL 업데이트] 탭에 추가됩니다. [!DNL Workfront] 문제 또는 작업 </p> <p>참고: 다음에 대한 날짜는 변경되지 않음 [!DNL Workfront] 문제 또는 작업 </p> </td> 
  </tr> 
  <tr> 
   <td> 에 시간 기록 [!DNL Workfront] 오른쪽 패널 또는 의 [!UICONTROL 기타] 메뉴에서 [!DNL Jira] 문제<br></td> 
   <td> <p>시간<br>Jira에 로그인한 시간을 링크에 추가하는 것 외에도 [!DNL Workfront] 항목, 로깅 시간에 대한 주석이 의 [!UICONTROL Updates] 탭에 추가됩니다. [!DNL Workfront] 항목.</p> <p>연결 시 시간 로깅에 대한 자세한 정보 [!DNL Jira] 문제(업데이트 포함) [!DNL Jira] 에서 시간을 기록 중인 사용자 [!DNL Workfront], 참조 <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">연결된 시간 기록 [!DNL Jira] 및 [!DNL Workfront] 개 항목</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> 댓글 <br><br></td> 
   <td> <p>주석이 의 [!UICONTROL Updates] 탭에 추가됩니다. [!DNL Workfront] 다음과 같은 경우 문제 또는 작업 <strong>[!UICONTROL Comments]</strong> [!UICONTROL Setup] 탭의 [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] 섹션에서 다음을 설정합니다. <strong>[!UICONTROL Always]</strong>.</p> <p>Workfront 설정 구성에 대한 자세한 내용은 [!DNL Jira], 참조 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">구성 [!DNL Workfront for Jira]</a>.</p> <p>링크된 항목에 대한 댓글 달기에 대한 자세한 정보 [!DNL Jira] 문제, 참조 <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">연결된 댓글의 댓글 [!DNL Jira] 문제</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 연결 시간 기록 [!DNL Jira] 문제

에 대해 기록하는 시간 [!DNL Jira] 의 항목 [!DNL Jira] 은 연결된 [!DNL Workfront] 항목, 위치 불문 [!DNL Jira] 시간을 기록합니다.\
에서 Jira에 시간을 기록할 때 [!DNL Workfront] 패널, 시간은 에만 기록됩니다. [!DNL Workfront].\
레코딩 시간 [!DNL Workfront] 에서 연결된 문제의 시간에 영향을 주지 않음 [!DNL Jira].

>[!NOTE]
>
>시간이 다음에 추가되는 경우 [!DNL Jira] 에 연결된 항목 [!DNL Workfront] 작업, [!UICONTROL 시간 유형] 당분간 [!DNL Workfront] 은(는) [!UICONTROL 작업 시간]. 시간이 다음에 추가되는 경우 [!DNL Jira] 에 연결된 항목 [!DNL Workfront] 문제, [!UICONTROL 시간 유형] 당분간 [!DNL Workfront] 은(는) [!UICONTROL 문제 시간].

댓글이 다음에 추가됩니다. **[!DNL Workfront]** 의 탭 [!DNL Jira] 및 대상 **[!UICONTROL 업데이트]** 내 항목의 탭 [!DNL Workfront] 시간 기록을 위해.\
시간은에 표시됩니다. **[!UICONTROL 시간]** 의 탭 [!DNL Workfront] 항목.

* [연결된 시간 기록 [!DNL Jira] 및 [!DNL Workfront] 개 항목](#log-time-for-linked-jira-and-workfront-items)
* [다음에서 시간 기록 [!DNL Jira] (으)로 [!DNL Workfront] 항목](#log-time-from-jira-to-a-workfront-item)

### 연결된 시간 기록 [!DNL Jira] 및 [!DNL Workfront] 개 항목

다음에서 시간을 기록할 수 있습니다. [!DNL Jira] 에 연결된 문제 [!DNL Workfront] 항목과 시간은 모두 [!DNL Jira] 문제뿐만 아니라 [!DNL Workfront] 항목.

>[!IMPORTANT]
>
>사용자가 시간을 로그인하는 경우 [!DNL Jira] 이(가)에 존재하지 않음 [!DNL Workfront], 다음과 같은 경우 통합은 Workfront에서 새 활성 사용자를 만듭니다. **[!UICONTROL 에서 자동으로 사용자 만들기 [!DNL Workfront]다음과 같은 &#x200B; 경우 [!DNL Jira] 사용자에게 이(가) 없음&#x200B;*[!DNL Workfront]&#x200B; 계정]**가 로 설정되어 있습니다.**[!UICONTROL &#x200B;항상&#x200B;]**. 이 사용자는 [!DNL Workfront] 라이센스. 의 작업 항목에 활성 사용자를 할당할 수 있습니다. [!DNL Workfront], 하지만 업데이트에 포함할 수 없습니다. 의 자동 생성 구성에 대한 정보 [!DNL Workfront] 의 사용자 [!DNL Jira], 참조 [구성 [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

항목에 대한 시간을 기록하려면 [!DNL Jira] 및 다음 두 항목에 모두 기록 [!DNL Jira] 및 [!DNL Workfront]:

1. 에 로그인 [!DNL Jira].
1. 로 이동 [!DNL Jira] 에 연결된 문제 [!DNL Workfront] 항목.
1. 확장 **[!UICONTROL 자세히]** 메뉴 및 클릭 **[!UICONTROL 로그 작업]**.

1. 다음에서 **[!UICONTROL 체류 시간]** 필드에서는 이 문제에 대해 작업하는 데 걸린 시간을 지정합니다. 다음 기간을 사용하여 시간을 지정해야 합니다.

   * [!UICONTROL 주] (w)
   * [!UICONTROL 일] 라.
   * [!UICONTROL 시간] 아.

1. 다음을 포함하여 시간 항목에 정보를 계속 추가합니다. **[!UICONTROL 작업 설명]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 로그]**.\
   시간이 다음에 추가됩니다. **[!UICONTROL 작업 로그]** 의 탭 [!DNL Jira] 항목 및 [!DNL Workfront] 항목이 연결되어 있습니다.\
   시간 항목에 대한 작업 설명은 의 시간 항목에 대한 메모로 기록됩니다 [!DNL Workfront].

### 다음에서 시간 기록 [!DNL Jira] (으)로 [!DNL Workfront] 항목

연결된 항목에만 시간을 기록할 수 있습니다 [!DNL Workfront] 의 항목 [!DNL Jira] 이 시간을 (으)로 기록하지 않는 문제 [!DNL Jira] 문제.

1. 에 로그인 [!DNL Jira].
1. 다음으로 이동 [!DNL Jira] 에 연결된 문제 [!DNL Workfront] 항목.

   세부 정보 [!DNL Workfront] 항목이 다음에 표시되어야 함: [!DNL Workfront] 문제의 오른쪽 패널.

1. 다음을 클릭합니다. **[!UICONTROL 로그 시간]** 아이콘.

1. 금액 지정 **[!UICONTROL 시간]** 및 **[!UICONTROL 분]** 문제에 대해 기록하려고 합니다.

1. 클릭 **[!UICONTROL 로그 시간]**.

   시간이 다음에 추가됩니다. [!DNL Workfront] 항목.

   이 시간은 다음에 추가되지 않습니다. [!UICONTROL 작업 로그] 의 탭 [!DNL Jira] 문제.

## 연결된 댓글의 댓글 [!DNL Jira] 문제 {#comment-from-a-linked-jira-issue}

다음에 대한 댓글을 달 때 [!DNL Jira] 의 항목 [!DNL Workfront] 의 오른쪽 패널 [!DNL Jira]에 대한 주석도 추가됩니다. [!UICONTROL 업데이트] Workfront에 있는 연결된 항목의 탭입니다.

댓글을 달려면 [!DNL Jira] (으)로 [!DNL Workfront] 항목:

1. 에 로그인 [!DNL Jira].
1. 다음으로 이동 [!DNL Jira] 에 연결된 문제 [!DNL Workfront] 항목.

   세부 정보 [!DNL Workfront] 항목이 다음에 표시되어야 함: [!DNL Workfront] 문제의 오른쪽 패널.

1. 다음을 클릭합니다. **[!UICONTROL 댓글]** 아이콘 [!DNL Workfront] 패널 또는 **[!UICONTROL 댓글]** 탭.

1. 댓글을 입력한 다음 **[!UICONTROL 보내기]**.

   주석이 다음에 추가됩니다.

   * 다음 **[!DNL Workfront]** 의 탭 [!DNL Jira] 문제.
   * 다음 **[!UICONTROL 댓글]** 의 탭 [!DNL Jira] 문제.
   * 다음 **[!UICONTROL 업데이트]** Workfront에 있는 연결된 항목의 탭입니다.
