---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 구성 [!DNL Adobe Workfront for Jira]
description: 다음을 사용할 수 있습니다. [!DNL Adobe Workfront for Jira] 를 [!DNL Jira] 및 [!DNL Workfront] 시스템.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '2373'
ht-degree: 0%

---

# 구성 [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->

다음을 사용할 수 있습니다. [!DNL Adobe Workfront for Jira] 를 [!DNL Jira] 및 [!DNL Workfront] 시스템.

추가 기능을 설치한 후 다음을 만드는 워크플로를 정의할 수 있습니다. [!DNL Jira] 다음과 같은 경우 자동으로 문제 발생 [!DNL Workfront] 작업 항목이 만들어집니다. 두 응용 프로그램의 항목이 연결되고 일부 정보는 두 시스템에서 자동으로 업데이트됩니다.

의 모든 사용자 [!DNL Workfront] 및 [!DNL Jira] 은 이 통합의 이점을 얻을 수 있습니다. 가장 많이 사용하는 시스템에 대한 라이선스만 있으면 되고 두 시스템 모두에 대한 라이선스는 필요하지 않습니다.

이 추가 기능은 다음 두 경우에 모두 사용할 수 있습니다. [!UICONTROL 서버] 및 [!UICONTROL OnDemand] (또는 [!UICONTROL 클라우드]) 버전 [!DNL Jira] 소프트웨어.

의 목록 [!DNL Jira] 버전 [!DNL Workfront for Jira] 현재 지원됨, 참조 [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 위치: [!DNL Atlassian Marketplace].

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] 플랜]</td> 
   <td><p>새로 만들기: 모두</p>
       <p>또는</p>
       <p>현재: [!UICONTROL Pro] 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: [!UICONTROL Standard] </p>
       <p>또는</p> 
       <p>현재: [!UICONTROL Plan] </p>
   </td>
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

을(를) 구성하기 전에 [!DNL Workfront for Jira], 다음을 수행해야 합니다.

* 설치 [!DNL Workfront for Jira].
설치에 대한 지침 [!DNL Workfront for Jira], 참조 [설치 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 구성 [!DNL Workfront for Jira]

다음을 구성함으로써 [!DNL Workfront for Jira], 다음 작업을 수행할 수 있습니다.

* 생성할 트리거 정의 [!DNL Jira] 다음과 같은 경우 항목 [!DNL Workfront] 항목이 만들어집니다.
* 사이에 연결된 항목 간에 동기화할 필드 지정 [!DNL Jira] 및 [!DNL Workfront].

>[!NOTE]
>
>* 를 구성한 후 [!DNL Workfront for Jira] 다음에 대한 [!DNL Jira] 환경, 모두 [!DNL Jira] 사용자에게 보기 [!DNL Workfront] 모든 항목의 오른쪽 패널 [!DNL Jira] 개 항목. 패널에는 링크할 수 있는 항목에 대한 정보가 포함되어 있습니다 [!DNL Workfront] 또는 을 지정하지 않도록 지정합니다. [!DNL Workfront] 항목이 다음에 링크됨 [!DNL Jira] 개 항목.
>* 사용 시 [!DNL Jira Server] 설치 시 Workfront 통합에 대한 트리거로 식별된 프로젝트와 관련된 문제만 Workfront 패널이 표시됩니다. 에 대한 트리거 설정에 대한 자세한 내용은 [!DNL Workfront to Jira] 워크플로우, 참조 [다음 사이에 항목을 자동으로 연결하기 위한 트리거 구성 [!DNL Jira] 및 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

구성하려면 [!DNL Workfront for Jira]:

1. 에 로그인 [!DNL Jira] as a [!DNL Jira] 관리자.
1. 클릭 **[!UICONTROL 설정]** 기본 [!DNL Jira] 메뉴 아래의 제품에서 사용할 수 있습니다.
1. 클릭 **[!UICONTROL 추가 기능]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 추가 기능 관리]**.

1. 확장 **[!DNL Workfront]** 추가 기능.
1. 클릭 **[!UICONTROL 구성]**.
1. 프롬프트의 안내에 따라 다음으로 로그인합니다. [!DNL Workfront].

   >[!NOTE]
   >
   >사용자에게 유효한 권한이 있어야 합니다. `apiKey` 위치: [!UICONTROL Workfront] 을 클릭하여 성공적인 연결을 만듭니다.

   에 로그인해야 합니다. [!DNL Workfront] as a [!DNL Workfront] 관리자를 사용하여 구성을 계속합니다.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] 에 연결 [!DNL Jira] 사용자의 인증 및 권한 부여를 위해 대부분의 웹 기반 통합에서 사용하는 표준인 OAuth 2.0을 사용합니다.
   >* 의 도메인을 입력하라는 메시지가 표시되면 [!DNL Workfront] 계정, 다음 형식을 사용하여 입력: *yourCompany&#39;sDomain.my.workfront.com*. 회사의 도메인은 일반적으로 회사의 이름입니다.
   >* 향상된 인증은 [!DNL Workfront] 관리자가 이 통합을 위해 활성화합니다.

1. Jira에서 **[!UICONTROL 트리거]** 의 자동 생성을 구성하는 탭 [!DNL Jira] 새 항목으로 항목 [!DNL Workfront] 항목이 만들어집니다.

   Workfront 트리거 설정에 대한 자세한 내용은 [!DNL Jira] 워크플로우, 참조 [다음 사이에 항목을 자동으로 연결하기 위한 트리거 구성 [!DNL Jira] 및 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. 다음 항목 선택 **[!UICONTROL 설정]** 링크된 필드 간의 필드 동기화를 구성하는 탭 [!DNL Jira] 및 [!DNL Workfront] 개 항목.

   간 필드 동기화 설정에 대한 자세한 정보 [!DNL Jira] 및 [!DNL Workfront], 참조 [간 필드 동기화 구성 [!DNL Jira] 및 [!DNL Workfront] 항목](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >두 응용 프로그램 간에 트리거와 필드 동기화를 정의하면 [!DNL Workfront] 작업 또는 문제를 만들 수 있는 사용자가에 항목 만들기를 트리거할 수 있음 [!DNL Jira]. 사용자는 자신이 만드는 항목의 기준이 의 트리거와 일치하는 경우 항목을 만들 수 있습니다. [!DNL Jira], 사용자에게 이 없는 경우에도 [!DNL Jira] 라이센스. 또한 [!DNL Jira] 사용자는 다음 작업을 즉시 시작할 수 있습니다. [!DNL Jira] 항목과 해당 업데이트가 [!DNL Workfront], 다음을 포함하지 않음 [!DNL Workfront] 라이센스. 의 모든 업데이트 [!DNL Workfront] 또한에 표시 [!DNL Jira] 개 항목.

1. (선택 사항) **[!UICONTROL 활동 로그]** 을 탭하여 통합 중에 발생했을 수 있는 오류를 검토합니다.

   에 대한 자세한 내용은 [!UICONTROL 활동 로그], 참조 [보기 [!DNL Jira] [!UICONTROL 활동 로그]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## 다음 사이에 항목을 자동으로 연결하기 위한 트리거 구성 [!DNL Jira] 및 [!DNL Workfront]

다음으로: [!DNL Jira] 시스템 관리자는에서 문제를 자동으로 생성하는 트리거를 정의할 수 있습니다. [!DNL Jira] 항목이 있는 경우 [!DNL Workfront] 특정 기준을 충족합니다.

>[!NOTE]
>
>통합이에서 새 문제를 만드는 데 최대 10분이 소요될 수 있습니다. [!DNL Jira].

생성 트리거를 구성할 때는 다음 사항을 고려하십시오. [!DNL Jira] 다음으로 항목: [!DNL Workfront] 항목이 만들어집니다.

* 통합은 단방향입니다. 생성하는 항목만 트리거할 수 있습니다. [!DNL Workfront] 에서 자동으로 만들어짐 [!DNL Jira]. 에서 만드는 항목은 트리거할 수 없습니다. [!DNL Jira] 다음 위치에 자동으로 생성: [!DNL Workfront].
* 가질 수 있는 트리거 수에 제한은 없습니다.
* 에서 생성하는 항목인 경우 [!DNL Workfront] 둘 이상의 트리거와 일치하는에 하나의 항목만 만들어집니다. [!DNL Jira]. 항목이 작성되는 위치: [!DNL Jira] 첫 번째 트리거에 따라(정의된 순서대로) [!DNL Jira]). 다른 모든 트리거는 무시됩니다.
* 의 항목 하나만 [!DNL Workfront] jira의 한 항목에 연결할 수 있습니다. 연결할 수 없습니다. [!DNL Workfront] 항목을 여러 개로 변환 [!DNL Jira] 문제 또는 하나 [!DNL Jira] 다중 문제 [!DNL Workfront] 개 항목.

에서 항목을 자동으로 만들기 위한 트리거를 구성하려면 [!DNL Jira]:

1. 에 로그인 [!DNL Jira] 시스템 관리자입니다.
1. 클릭 **[!UICONTROL 설정]** 기본 [!DNL Jira] 메뉴 아래의 제품에서 사용할 수 있습니다.
1. 클릭 **[!UICONTROL 추가 기능]**, 그런 다음 **[!UICONTROL 추가 기능 관리]**.
1. 확장 **[!DNL Workfront]** 추가 기능.
1. 클릭 **[!UICONTROL 구성]**.
1. 에 로그인 [!DNL Workfront] 시스템 관리자입니다.

   다음 **[!UICONTROL 트리거]** jira에서는 기본적으로 탭이 선택됩니다.

1. 클릭 **[!UICONTROL 트리거 추가]** 새 트리거를 추가합니다.
1. 다음에서 **[!UICONTROL Workfront 팀/사용자/역할]** 필드, 이름 지정 [!DNL Workfront] 팀, 사용자 또는 작업 역할을 선택한 다음 목록에 표시될 때 클릭하여 선택합니다.

   >[!NOTE]
   >
   >동일한 팀, 사용자 또는 역할에 여러 트리거를 사용할 수 없습니다.

   누군가가 작업 또는 문제를 만들어 이러한 엔터티 중 하나에 할당하면 [!DNL에서 문제가 자동으로 만들어집니다 [!DNL Jira]].

1. 다음에서 **[!UICONTROL [!DNL Jira]프로젝트]** 필드, 이름 입력 시작 [!DNL Jira] 프로젝트를 클릭한 다음 목록에 표시될 때 클릭하여 선택합니다.

   다음의 경우 [!DNL Jira] 문제가 생성되면 여기에서 선택한 프로젝트에 배치됩니다.

1. 선택 **I[!UICONTROL 문제 유형]** 드롭다운 메뉴에서 을(를) 선택합니다.

   에서 생성된 문제 유형을 나타냅니다. [!DNL Jira] 의 특정 프로젝트에 대한 설정을 기반으로 이 트리거의 조건이 충족되는 경우 [!DNL Jira].

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이 구성을 사용하면 [!DNL Workfront] 사용자가 지정된 트리거와 일치하는 항목을 만들면에서 새 문제가 만들어집니다. [!DNL Jira].

## 간 필드 동기화 구성 [!DNL Jira] 및 [!DNL Workfront] 항목

다음으로: [!DNL Jira] 관리자, 링크된 항목에서 자동으로 동기화할 필드를 정의할 수 있습니다. [!DNL Workfront] 그리고 지라 특정 필드는 [!DNL Workfront] (으)로 [!DNL Jira] 항목과 다른 항목은 Jira에서 Workfront으로 동기화됩니다.

두 애플리케이션 간에 연결된 항목에 대해 자동으로 동기화할 필드를 정의하려면

1. 에 로그인 [!DNL Jira] Jira 관리자로서.
1. 클릭 **[!UICONTROL 설정]** 기본 [!DNL Jira] 메뉴 아래의 제품에서 사용할 수 있습니다.
1. 클릭 **[!UICONTROL 추가 기능]**, 그런 다음 **[!UICONTROL 추가 기능 관리]**.
1. 확장 **[!DNL Workfront]** 추가 기능.
1. 클릭 **[!UICONTROL 구성]**.
1. 에 로그인 [!DNL Workfront] Workfront 관리자입니다.
1. Jira에서 **[!UICONTROL 설정]** 탭.
1. 다음에서 **[!UICONTROL Workfront에서 Jira로 동기화]** 섹션에서 업데이트할 필드를 선택합니다 [!DNL Jira] Workfront에서 업데이트된 경우.

   1. 필드가 동기화되는 다음 빈도 중 하나를 선택합니다.

      <table style="table-layout:auto">
         <tr>
              <td>만들 때 [!UICONTROL]</td>
              <td>지정하는 필드는 연결된 Workfront과 간에 동기화됩니다. [!DNL Jira] 항목이 Workfront에서 만들어지는 경우입니다.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>지정하는 필드는 연결된 Workfront과 간에 동기화됩니다. [!DNL Jira] Workfront에서 필드를 업데이트할 때의 항목입니다. </td>
          </tr>
          <tr>
              <td>[!UICONTROL 사용 안 함]</td>
              <td>지정한 필드는 연결된 필드 간에 동기화되지 않습니다 [!DNL Workfront] 및 [!DNL Jira] 개 항목. 에 표시가 없습니다. [!DNL Jira] 필드가 업데이트된 위치 [!DNL Workfront]. </td>
          </tr>
      </table>

   1. 다음 중 하나를 선택하여 의 필드를 동기화하십시오. [!DNL Workfront] 끝 [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL 이름]</td>
         <td><p>의 작업 또는 문제 이름 [!DNL Workfront] 은 이 문제가 연결된 문제의 이름이 됩니다 [!DNL Jira].</p><p>참고: 새 항목이에 생성될 때 [!DNL Jira] 자동으로, [!DNL Workfront] 이름은 항상 다음에 대해 업데이트됩니다. [!DNL Jira] 항목(이 필드가 여기에서 활성화되는지 여부에 관계없이) 다음과 같은 경우 [!DNL Jira] 항목이 수동으로 다음에 연결됨 [!DNL Workfront] 항목, 이름 [!DNL Workfront] 항목만 다음 위치에서 업데이트됨 [!DNL Jira] 을(를) 선택할 때 <strong>항상</strong> 이 필드를 동기화합니다. 수동으로 또는 자동으로 항목 연결에 대한 자세한 내용은 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">다음 사이에 항목 연결 [!DNL Adobe Workfront] 및 [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 설명]</td>
         <td>의 작업 또는 문제에 대한 설명 [!DNL Workfront] 는 연결된 문제에 대한 설명이 됩니다. [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">문서</td>
         <td><p>의 작업 또는 문제에 첨부된 문서 [!DNL Workfront] jira에서 연결되어 있는 문제에도 첨부되어 있습니다. 의 새 문서 버전 [!DNL Workfront] 는 별도의 문서로 Jira에 추가되고 <i>_v&lt;version number=""&gt;</i> Workfront에서 번호가 매겨진 버전을 나타냅니다. </p><p>예를 들어 의 문서 이름이 [!DNL Workfront] 은(는) <strong>메인 광고</strong>및에서 새 버전을 추가합니다. [!DNL Workfront], 새 버전이 (으)로 전송됩니다. [!DNL Jira] 을(를) 이름이 인 새 문서로 <strong>기본 Ad_v2</strong>.</p><p>중요 사항: <p>문서를 동기화할 때는 다음 사항을 고려하십시오.</p>
           <ul>
            <li><p>5MB가 넘는 문서는 동기화되지 않습니다. 문서가 너무 커서 문서 동기화에 실패하면 오류가 활동 로그에 기록됩니다. </p><p>작업 로그에 대한 자세한 내용은 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Jira 활동 로그 보기</a>.</p></li>
            <li><p>외부 서버의 작업 및 문제에 연결된 문서는 [!DNL Jira] 개 항목. 의 작업 또는 문제에 직접 업로드된 문서만 [!DNL Workfront] 에서 연결된 문제로 전송됨 [!DNL Jira].</p></li>
            <li><p>문서에서 증명을 만들려면 다음 위치에서 증명을 생성해야 합니다. [!DNL Workfront]. </p><p>증명 생성에 대한 자세한 내용은 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">기존 문서에 대한 증명 만들기 </a>위치: <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">문서에 대한 증명 만들기</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 계획된 완료 일자]</td>
         <td><p>의 작업 또는 문제에 대한 [!UICONTROL 계획된 완료 일자] [!DNL Workfront] 이(가) 연결된 문제의 [!UICONTROL 기한]이 됩니다. [!DNL Jira].</p><p>참고: 다음을 표시합니다 <strong>[!UICONTROL 기한]</strong> 날짜 [!DNL Jira] 문제, 이 값을 동기화해야 합니다.</p></td>
        </tr>
       </tbody>
      </table>

1. 다음에서 **[!UICONTROL 다음에서 동기화 [!DNL Jira] 끝[!DNL Workfront]]** 섹션에서 업데이트할 필드를 선택합니다 [!DNL Workfront] 업데이트 시기 [!DNL Jira].

   1. 필드가 동기화되는 다음 빈도 중 하나를 선택합니다.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>지정한 필드는 항상 연결된 필드 간에 동기화됩니다. [!DNL Workfront] 및 [!DNL Jira] 다음에서 필드가 업데이트될 때 항목: [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 사용 안 함]</td>
         <td><p>지정한 필드는 연결된 필드 간에 동기화되지 않습니다 [!DNL Workfront] 및 [!DNL Jira] 개 항목. 에 표시가 없습니다. [!DNL Workfront] 필드가 업데이트된 위치 [!DNL Jira]. </p><p>참고: 절대 안 함을 선택하면 [!DNL Workfront] 필드는 다음에서 계속 수동으로 업데이트할 수 있습니다. [!DNL Jira] 왼쪽에서 [!DNL Workfront] 패널 [!DNL Jira] 문제. 이러한 업데이트는 다음에만 표시됩니다. [!DNL Workfront] 의 항목 [!DNL Jira] 및 [!DNL Workfront] 및 다음에 없음 [!DNL Jira] 개 항목.</p></td>
        </tr>
       </tbody>
      </table>

   1. 에서 다음 필드 중 하나를 동기화하려면 선택하십시오. [!DNL Jira] 끝 [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL 상태]</td>
         <td>에서 문제에 대한 [!UICONTROL 상태] [!DNL Jira] 이(가) 연결된 작업 또는 문제의 [!UICONTROL 상태]가 됩니다. [!DNL Workfront].<br>에 대한 자세한 내용 [!DNL Workfront] 상태, 참조 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">상태 만들기 또는 편집</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 담당자]</td>
         <td><p>의 문제에 대한 [!UICONTROL Assignee] [!DNL Jira] 이(가) 연결된 작업 또는 문제의 [!UICONTROL Assignee](이)가 됩니다. [!DNL Workfront].</p><p>중요:에서 품목을 지정할 때 [!DNL Jira] 이(가) 없는 사용자에게 [!DNL Workfront] 계정, 통합은에서 새 활성 사용자를 만듭니다. [!DNL Workfront] 다음과 같은 경우에만 <strong>에서 자동으로 사용자 만들기 [!DNL Workfront] 다음과 같은 경우 [!DNL Jira] 사용자에게 이(가) 없음 [!DNL Workfront] account</strong> 이(가) (으)로 설정됨 <strong>[!UICONTROL Always]</strong>. 이 사용자는 [!DNL Workfront] 라이센스. 활성 사용자를 의 작업 항목에 할당할 수 있습니다. [!DNL Workfront], 업데이트에 포함될 수 없습니다. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 첨부 파일]</td>
         <td>의 문제 첨부 파일 [!DNL Jira] 연결된 작업 또는 문제에도 첨부됩니다. [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>에 대한 댓글 [!DNL Jira] 문제가 또한 [!DNL Workfront] [!UICONTROL Updates] 영역의 항목입니다. 반대로 의 [!UICONTROL Updates] 영역에 게시된 주석은 [!DNL Workfront] 작업 또는 문제를 (으)로 동기화 [!DNL Jira]연결된 문제에 대한 의 기본 댓글 스트림입니다. </p><p>다음으로 설정됨: <strong>[!UICONTROL Always]</strong> 기본적으로. 다음을 선택하는 경우 <strong>[!UICONTROL 사용 안 함]</strong> 여기에서 연결된 항목에 주석을 수동으로 게시할 수 있습니다. [!DNL Workfront] 또는 [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. 다음에서 **[!UICONTROL 기타]** 섹션에서 연결된 항목 사이에 업데이트할 추가 필드를 선택합니다.

   1. 옵션을 선택하여 지정한 필드를 사용할지 여부를 결정합니다 **[!UICONTROL 항상]** 또는 **[!UICONTROL 사용 안 함]** 업데이트 위치 [!DNL Jira] 또는 [!DNL Workfront] 수정 시.

   1. 다음 필드 및 업데이트 중에서 선택합니다.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL 사본 [!DNL Workfront] 의 오른쪽 패널에 있는 사용자 정의 데이터 [!DNL Jira]]</td>
         <td><p>다음을 표시합니다. [!DNL Workfront] 에 있는 항목의 사용자 지정 데이터 [!DNL Workfront] 오른쪽 패널.</p><p>참고: 사용자 정의 양식 섹션은 [!DNL Workfront] 의 액세스 수준이 있는 오른쪽 패널 [!DNL Workfront] 시스템 관리자.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 사본 [!DNL Workfront] 의 오른쪽 패널에 있는 우선 순위 [!DNL Jira]]</td>
         <td>다음을 표시합니다. [!DNL Workfront] 에 있는 항목의 우선 순위 [!DNL Workfront] 오른쪽 패널.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 업데이트 추가 [!DNL Workfront] 의 기한 변경에 대한 업데이트 탭 [!DNL Jira]]</td>
         <td>의 [!UICONTROL Update] 탭에 주석을 추가합니다. [!DNL Workfront] 링크된 항목의 [!UICONTROL 기한]이 변경될 때 항목 [!DNL Jira] 항목.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL에서 자동으로 사용자 만들기 [!DNL Workfront] 다음과 같은 경우 [!DNL Jira] 사용자에게 이(가) 없음 [!DNL Workfront] account]</td>
         <td><p>다음과 같은 시나리오가 있습니다.</p>
          <ul>
           <li>다음을 선택할 때 <strong>[!UICONTROL Always]</strong>, 통합을 활성화하여 매번 새 Workfront 사용자를 만듭니다. [!DNL Jira] 이(가) 없는 사용자 [!DNL Workfront] 계정은 연결된 항목에 대해 다음 작업을 수행합니다 [!DNL Jira] 문제:
            <ul>
             <li>이(가)에게 할당되었습니다. [!DNL Jira] 문제</li>
             <li><p>에 시간 기록 [!DNL Jira] 문제</p><p>이 새 사용자는 [!DNL Workfront] 라이센스. 기본 설정은 항상 입니다. 사용자가에서 이러한 방식으로 생성됨 [!DNL Workfront] 이름에 "[!UICONTROL Jira]"가 추가되었습니다.</p></li>
            </ul></li>
           <li>다음을 선택할 때 <strong>[!UICONTROL 사용 안 함]</strong>, 다음과 같은 상황이 발생합니다.
            <ul>
             <li>아무 것도 볼 수 없습니다. [!DNL Jira] 다음에 대한 할당 [!DNL Workfront] 개 항목. 이 경우 할당만 [!DNL Workfront] 다음에 표시 [!DNL Workfront] 개 항목.</li>
             <li>연결된 (으)로 기록된 시간 [!DNL Jira] 이(가) 없는 사용자에 의한 문제 [!DNL Workfront] 계정이 연결된 계정으로 자동 전송되지 않음 [!DNL Workfront] 항목. 에 시간을 기록할 수 있습니다. [!DNL Workfront] 의 오른쪽 패널에 있는 항목 [!DNL Jira] 문제.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 사용자가 다음 중 하나의 항목에 대해 이 구성에 지정된 필드를 업데이트할 때마다 [!DNL Jira] 또는 [!DNL Workfront]로 설정되어 있는 경우 다른 애플리케이션의 연결된 항목도 업데이트됩니다.

## 문제 해결

### 항목은에서 만들 수 없습니다. [!DNL Jira] (이)가 &quot;&quot;로 표시된 트리거 필드로 인해[!UICONTROL 을(를) 찾을 수 없음]&quot;

#### 문제

에 오류가 발생하는 경우 [!DNL Workfront for Jira] 애플리케이션, [!DNL Workfront] 추가 합병증을 방지하기 위해 트리거를 비활성화합니다. 이러한 트리거가 비활성화되면 &quot;&quot;로 표시됩니다.[!UICONTROL 을(를) 찾을 수 없음].&quot;

#### 솔루션

트리거를 비활성화한 오류를 찾습니다. 다음에서 오류를 찾을 수 있습니다. [!DNL Workfront for Jira] [!UICONTROL 활동 로그].

이 동작의 가장 일반적인 원인은 오류 입니다.[!UICONTROL 필드 &#39;duedate&#39;를 설정할 수 없습니다. 적절한 화면이 아니거나 알 수 없습니다.]&quot;

이 오류는 &quot; &quot;을(를) 동기화하려고 함을 의미합니다.[!UICONTROL 계획된 완료 일자]&quot; 출처: [!DNL Workfront] 끝 [!DNL Jira]. 이렇게 하려면 다음을 확인해야 합니다. [!DNL Jira] 개체에는 라는 필드가 있습니다.[!UICONTROL 기한].&quot; 이 필드가 없으면 [!DNL Workfront] 은(는) 다음 시점부터 계획된 완료 일자를 동기화할 수 없습니다. [!DNL Workfront] 트리거를 비활성화합니다.

이 오류를 해결하려면 다음 중 하나를 시도해 보십시오.

* 다음 사용자에게 묻기 [!DNL Jira] 관리자가 영향을 받는 을(를) 업데이트할 수 있음 [!DNL Jira] 기한 필드가 있는지 확인하기 위한 개체입니다.
* 동기화 비활성화 [!DNL Workfront]Workfront에서의 의 계획된 완료 일자 [!UICONTROL 설정] 페이지를 가리키도록 업데이트하는 중입니다.
