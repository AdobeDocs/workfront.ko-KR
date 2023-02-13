---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: GitLab 모듈
description: Adobe Workfront Fusion에는 Adobe Workfront 라이선스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: d55ddd97a69f00a1f42d84dc55a12d2017855776
workflow-type: tm+mt
source-wordcount: '4370'
ht-degree: 0%

---


# [!UICONTROL GitLab] 모듈

Adobe Workfront Fusion에는 Adobe Workfront 라이선스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!UICONTROL GitLab]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

>[!NOTE]
>
>이 문서에서는 API 설명서 및 [!DNL GitLab] 기능을 일반적으로 사용합니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Connect [!DNL GitLab] to [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. 어떤 경우에서도 [!DNL Workfront Fusion] [!DNL Gitlab] 모듈 **[!UICONTROL 추가]** 연결 필드 옆에 있습니다.
1. 다음 필드를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 연결 이름]</td> 
      <td> <p>연결의 이름을 입력합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>의 URL을 입력합니다 [!DNL GitLab] 인스턴스.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 액세스 토큰]</td> 
      <td><p>[!UICONTROL Private Token] 또는 [!UICONTROL Personal Access Token]을 입력합니다.</p><p>에서 개인 액세스 토큰을 찾거나 만드는 방법에 대한 자세한 내용은 [!DNL GitLab]의 "개인 액세스 토큰 만들기"를 참조하십시오. <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">개인 액세스 토큰</a> 에서 [!DNL GitLab] 설명서.</p></td> 
     </tr> 
    </tbody> 
   </table>


1. 클릭 **[!UICONTROL 계속]**.
1. 클릭 **[!UICONTROL 권한 부여]** 연결을 만들고 모듈로 돌아가려면 를 클릭합니다.

## [!DNL GitLab] 모듈 및 해당 필드

구성 시 [!DNL GitLab] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL GitLab] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

+++**[!UICONTROL 빌드 상태 보기]**

이 인스턴트 트리거 모듈은 빌드 상태가 변경될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>빌드 상태 변경을 웹 후크에서 감시하려는 프로젝트</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 커밋/MR/문제/코드 조각 주석 보기]**

이 인스턴트 트리거 모듈은 커밋, 병합 요청, 문제 또는 코드 조각에 대한 주석이 만들어질 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 주석을 확인할 프로젝트입니다</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 시청 커밋(밀어넣기)]**

이 인스턴트 트리거 모듈은 커밋이 리포지토리에 푸시되면 시나리오를 시작합니다. 이 모듈은 태그를 푸시할 때 시나리오를 시작하지 않습니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 커밋을 감시하려는 프로젝트</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 문제 설명 보기]**

이 인스턴트 트리거 모듈은 문제에 대한 댓글이 있을 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 문제 주석을 확인할 프로젝트입니다</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 문제 보기]**

이 [!UICONTROL 인스턴트 트리거] 모듈은 문제가 만들어지거나 기존 문제가 업데이트, 닫기 또는 다시 열릴 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 문제를 감시하려는 프로젝트</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 병합 요청 보기]**

이 인스턴트 트리거 모듈은 다음 중 하나가 발생하면 시나리오를 시작합니다.

* 새 병합 요청이 만들어집니다
* 기존 병합 요청이 업데이트, 병합 또는 닫힙니다
* 소스 분기에 커밋이 추가됩니다


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크가 병합 요청을 감시하도록 할 프로젝트</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 병합 요청 주석 보기]**

이 인스턴트 트리거 모듈은 병합 요청에 대한 주석이 만들어질 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 병합 요청 주석을 확인할 프로젝트입니다</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 파이프라인 상태 보기]**

이 인스턴트 트리거 모듈은 파이프라인의 상태가 변경될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 파이프라인 상태 변경을 감시하려는 프로젝트</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 프로젝트 보기]**

이 예약된 트리거 모듈은 인증된 사용자가 멤버인 새 프로젝트가 추가되면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL GitLab] 계정 대상 [!DNL Workfront] 융합을 참조하십시오. <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] 융착</a> 참조하십시오.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">최대 결과</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈에서 볼 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 저장소 분기 보기]**

이 예약된 트리거 모듈은 새 분기가 저장소에 추가될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL GitLab] 계정 대상 [!DNL Workfront] 융합을 참조하십시오. <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] 융착</a> 참조하십시오.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">최대 결과</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈에서 볼 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 저장소 태그 보기]**

이 인스턴트 트리거 모듈은 저장소에서 태그를 만들거나 삭제할 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 태그를 감시하려는 프로젝트</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 코드 조각 설명 보기]**

이 인스턴트 트리거 모듈은 코드 조각에 새 설명이 만들어지면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 주석을 확인할 프로젝트입니다</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 시계 도구]**

이 예약된 트리거 모듈은 새 todo가 추가되면 시나리오를 시작합니다. 필터가 적용되지 않으면 보류 중인 새 todo가 추가되면 트리거가 실행됩니다.

필드에 대한 자세한 내용은 [할 작업 목록 가져오기](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL Wiki 페이지 보기]**

이 인스턴트 트리거 모듈은 Wiki 페이지를 만들거나 편집할 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>이 트리거에 사용할 웹 후크를 선택하거나 새 웹 후크를 추가합니다. </p><p>새 웹 후크를 추가하려면 <ol><li>클릭 <b>[!UICONTROL Add]</b> 를 클릭하십시오.</li><li>다음을 입력합니다. <ul><li>웹 후크의 이름</li><li>이 웹 후크에 사용할 연결</li><li>웹 후크에서 Wiki 페이지를 확인할 프로젝트입니다</li></ul></li><li>클릭 <b>[!UICONTROL Save]</b> 웹 후크를 저장하고 모듈로 돌아가려면 를 클릭합니다. </td> 
   </tr> 
   </tbody> 
</table>

+++

### 액션

+++**[!UICONTROL 병합 요청 수락]**

이 작업 모듈은 제출된 변경 내용을 주어진 병합 요청과 병합합니다.

필드에 대한 자세한 내용은 [병합 요청 수락](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 빌드 취소]**

이 작업 모듈은 프로젝트의 단일 빌드를 취소합니다.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL GitLab] 계정 대상 [!DNL Workfront] 융합을 참조하십시오. <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] 융착</a> 참조하십시오.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID]</td> 
   <td> <p>취소할 빌드가 포함된 프로젝트를 선택하거나 매핑합니다.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL 빌드 ID]</td> 
   <td>취소할 빌드를 선택하거나 매핑합니다.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL 병합 커밋 메시지]</td> 
   <td> 병합할 커밋 메시지를 입력하거나 매핑합니다.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL 소스 분기를 제거해야 함]</td> 
   <td>병합이 완료되면 소스 분기를 제거할지 여부를 선택합니다.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">빌드가 성공하면 [!UICONTROL 병합]</td> 
   <td>빌드가 완료되는 즉시 병합 요청을 병합할지 여부를 선택합니다.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>있는 경우 이 SHA는 소스 분기의 HEAD과 일치해야 합니다. 일치하지 않으면 병합이 실패합니다.</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 파이프라인 빌드 취소]**

이 작업 모듈은 단일 파이프라인에 대한 빌드를 취소합니다.

필드에 대한 자세한 내용은 [파이프라인의 작업 취소](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 파이프라인이 성공하면 병합 취소]**

파이프라인이 성공하면 병합 요청을 병합하도록 설정하면 이 작업 모듈이 해당 작업을 취소합니다.

필드에 대한 자세한 내용은 [파이프라인이 성공하면 병합 취소](https://docs.gitlab.com/ee/api/merge_requests.html) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 체리를 택해라]**

이 액션모듈 체리는 주어진 나뭇가지에 대한 커밋을 선택합니다.

필드에 대한 자세한 내용은 [체리를 택해라](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 레이블 만들기]**

이 작업 모듈은 주어진 저장소에 대한 새 레이블을 만듭니다.

필드에 대한 자세한 내용은 [새 레이블 만들기](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 파이프라인 만들기]**

이 작업 모듈은 주어진 프로젝트에 대한 새 파이프라인을 만듭니다.

필드에 대한 자세한 내용은 [새 파이프라인 만들기](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 릴리스 만들기]**

이 작업 모듈은 기존 Git 태그에 릴리스 노트를 추가합니다.

필드에 대한 자세한 내용은 [릴리스 만들기](https://docs.gitlab.com/ee/api/releases/#create-a-release) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 태그 만들기]**

이 작업 모듈은 제공된 참조를 가리키는 새 태그를 저장소에 만듭니다.

필드에 대한 자세한 내용은 [새 태그 만들기](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 할 일 만들기]**

이 작업 모듈은 선택한 문제에 대해 현재 사용자에게 할 일을 만듭니다. 현재 사용자는 이 모듈에 사용되는 연결에 대한 자격 증명으로 식별되는 사용자입니다.

필드에 대한 자세한 내용은 [할 작업 만들기](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 병합 요청에 대한 작업을 만듭니다.]**

이 작업 모듈은 선택한 병합 요청에 대해 현재 사용자에 대한 작업을 만듭니다. 현재 사용자는 이 모듈에 사용되는 연결에 대한 자격 증명으로 식별되는 사용자입니다.

필드에 대한 자세한 내용은 [할 일 만들기](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 병합 요청 만들기]**

이 작업 모듈은 프로젝트에 대한 새 병합 요청을 만듭니다.

필드에 대한 자세한 내용은 [병합 요청 만들기](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 저장소에서 새 파일 만들기]**

이 작업 모듈은 선택한 저장소에 새 파일을 만듭니다.

필드에 대한 자세한 내용은 [저장소에서 새 파일 만들기](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 문제 노트 만들기]**

이 작업 모듈은 단일 프로젝트 문제에 대한 문제 메모를 만듭니다.

필드에 대한 자세한 내용은 [새 문제 노트 만들기](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 병합 요청 메모 만들기]**

이 작업 모듈은 단일 병합 요청에 대한 메모를 만듭니다.

필드에 대한 자세한 내용은 [새 병합 요청 메모 만들기](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 이정표 만들기]**

이 작업 모듈은 프로젝트에 대한 새 이정표를 만듭니다.

필드에 대한 자세한 내용은 [새 이정표 만들기](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 코드 조각 메모 만들기]**

이 작업 모듈은 단일 코드 조각에 대한 새 메모를 만듭니다. 코드 조각 메모는 사용자가 코드 조각에 게시할 수 있는 주석입니다.

필드에 대한 자세한 내용은 [새 코드 조각 메모 만들기](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 저장소 분기 만들기]**

이 작업 모듈은 단일 저장소 분기를 만듭니다.

필드에 대한 자세한 내용은 [저장소 분기 만들기](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 빌드 변수 만들기]**

이 작업 모듈은 새 빌드 변수를 만듭니다.

필드에 대한 자세한 내용은 [변수 만들기](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 병합 요청 삭제]**

이 작업 모듈은 관리자 및 프로젝트 소유자만 사용할 수 있습니다. 문제가 있는 병합 요청을 삭제합니다

필드에 대한 자세한 내용은 [병합 요청 삭제](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 저장소에서 기존 파일 삭제]**

이 작업 모듈은 저장소에서 기존 파일을 삭제합니다.

필드에 대한 자세한 내용은 [저장소에서 기존 파일 삭제](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 저장소 분기 삭제]**

이 작업 모듈은 저장소에서 분기를 삭제합니다.

필드에 대한 자세한 내용은 [저장소 분기 삭제](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 문제 편집]**

이 작업 모듈은 기존 프로젝트 문제를 업데이트합니다. 이 호출은 문제를 종결된 것으로 표시하는 데에도 사용됩니다.

필드에 대한 자세한 내용은 [문제 편집](https://docs.gitlab.com/ee/api/issues.html#edit-issue) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 이정표 편집]**
이 작업 모듈은 기존 프로젝트 이정표를 업데이트합니다.

필드에 대한 자세한 내용은 [이정표 편집](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 빌드 지우기]**

이 작업 모듈은 프로젝트 빌드를 지웁니다(작업 아티팩트와 작업 로그 제거).

필드에 대한 자세한 내용은 [작업 지우기](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 도구 목록 가져오기]**

이 검색 모듈은 할 일 항목 목록을 검색합니다.

필드에 대한 자세한 내용은 [할 작업 목록 가져오기](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 빌드 가져오기]**

이 작업 모듈은 프로젝트의 단일 작업을 검색합니다.

필드에 대한 자세한 내용은 [단일 작업 받기](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 저장소 태그 가져오기]**

이 작업 모듈은 이름으로 결정된 특정 저장소 태그를 검색합니다.

필드에 대한 자세한 내용은 [단일 저장소 태그 가져오기](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 특정 배포 받기]**

이 작업 모듈은 특정 배포를 검색합니다.

필드에 대한 자세한 내용은 [특정 배포 받기](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 이정표에 지정된 모든 문제 가져오기]**

이 검색 모듈은 단일 프로젝트 이정표에 지정된 모든 문제를 검색합니다.

필드에 대한 자세한 내용은 [단일 이정표에 지정된 모든 문제 가져오기](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 저장소에서 파일 가져오기]**

이 작업 모듈은 이름, 크기 또는 컨텐츠와 같은 저장소의 파일에 대한 정보를 검색합니다.

필드에 대한 자세한 내용은 [저장소에서 파일 가져오기](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 사용자 가져오기]**

이 검색 모듈은 프로젝트 사용자를 검색합니다.

필드에 대한 자세한 내용은 [프로젝트 사용자 가져오기](https://docs.gitlab.com/ee/api/projects.html#get-project-users) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 문제 가져오기]**

이 작업 모듈은 문제 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>새 연결을 만들려면 다음을 참조하십시오 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] Workfront Fusion으로 변환]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td> <p>세부 사항을 검색할 문제가 포함된 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문제 ID]</td> 
   <td> <p>세부 사항을 검색할 문제의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 단일 문제 노트 가져오기]**

이 작업 모듈은 특정 프로젝트 문제에 대한 단일 메모를 검색합니다.

필드에 대한 자세한 내용은 [단일 문제 노트 가져오기](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 병합 요청 가져오기]**

이 작업 모듈은 단일 병합 요청에 대한 정보를 검색합니다.

필드에 대한 자세한 내용은 [단일 병합 요청 가져오기](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 병합 요청 변경 내용 가져오기]**

이 검색 모듈은 파일 및 변경 사항을 포함한 병합 요청에 대한 정보를 검색합니다.

필드에 대한 자세한 내용은 [단일 병합 요청 변경 내용 가져오기](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 병합 요청 커밋 가져오기]**

이 작업 모듈은 병합 요청 커밋 목록을 검색합니다.

필드에 대한 자세한 내용은 [단일 병합 요청 커밋 가져오기](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 병합 요청 노트 가져오기]**

이 작업 모듈은 주어진 병합 요청에 대한 단일 메모를 반환합니다.

필드에 대한 자세한 내용은 [단일 병합 요청 노트 가져오기](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 이정표 가져오기]**

이 작업 모듈은 이정표 세부 사항을 검색합니다.

필드에 대한 자세한 내용은 [단일 이정표 가져오기](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 프로젝트 가져오기]**

이 작업 모듈은 프로젝트 세부 사항을 검색합니다.

필드에 대한 자세한 내용은 [단일 프로젝트 가져오기](https://docs.gitlab.com/ee/api/projects.html#get-single-project) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 단일 저장소 분기 가져오기]**

이 작업 모듈은 저장소 분기 세부 정보를 검색합니다.

필드에 대한 자세한 내용은 [단일 저장소 분기 가져오기](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 코드 조각 메모 가져오기]**

이 모듈은 주어진 코드 조각에 대한 단일 메모를 검색합니다.

필드에 대한 자세한 내용은 [단일 코드 조각 참고 사항 가져오기](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 커밋 주석 가져오기]**

이 검색 모듈은 프로젝트에서 커밋의 주석을 검색합니다.

필드에 대한 자세한 내용은 [커밋 주석 가져오기](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 커밋 비교 받기]**

이 작업 모듈은 프로젝트에서 커밋의 차이를 가져옵니다.

필드에 대한 자세한 내용은 [커밋 비교 받기](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 아티팩트 유지]**

만료를 설정할 때 아티팩트가 삭제되지 않도록 합니다.

필드에 대한 자세한 내용은 [아티팩트 유지](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 모든 병합 요청 노트 나열]**

이 검색 모듈은 단일 병합 요청에 대한 모든 메모 목록을 검색합니다.

필드에 대한 자세한 내용은 [모든 병합 요청 노트 나열](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 모든 코드 조각 메모 나열]**

이 모듈은 단일 코드 조각에 대한 모든 참고 사항 목록을 가져옵니다. 코드 조각 메모는 사용자가 코드 조각에 게시할 수 있는 주석입니다.

필드에 대한 자세한 내용은 [??](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 커밋 빌드 나열]**

이 검색 모듈은 프로젝트의 특정 커밋에 대한 빌드 목록을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>새 연결을 만들려면 다음을 참조하십시오 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] Workfront Fusion으로 변환]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID]</td> 
   <td> <p>빌드를 나열할 커밋이 포함된 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 범위]</td> 
   <td> 특정 상태로 검색을 빌드하도록 제한하려면 상태를 선택합니다. 이 필드를 비워 두면 커밋의 모든 빌드가 반환됩니다.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 목록 문제]**

이 검색 모듈은 지정된 필터 설정으로 모든 문제를 반환합니다.

필드에 대한 자세한 내용은 [목록 문제](https://docs.gitlab.com/ee/api/issues.html#list-issues) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 병합 시 끝나는 문제 나열]**

이 검색 모듈은 제공된 병합 요청을 병합하여 닫을 모든 문제를 검색합니다.

필드에 대한 자세한 내용은 [병합 시 닫을 문제 나열](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 목록 레이블]**

이 검색 모듈은 프로젝트의 모든 레이블을 검색합니다.

필드에 대한 자세한 내용은 [목록 레이블](https://docs.gitlab.com/ee/api/labels.html#list-labels) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 병합 요청 나열]**

이 검색 모듈은 필터 설정으로 모든 병합 요청을 검색합니다.

필드에 대한 자세한 내용은 [병합 요청 나열](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 소유한 프로젝트 나열]**

이 검색 모듈은 인증된 사용자가 소유자로 설정된 프로젝트를 검색합니다.

필드에 대한 자세한 내용은 [사용자 프로젝트 나열](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 빌드 나열]**

이 검색 모듈은 프로젝트의 빌드 목록을 검색합니다.

필드에 대한 자세한 내용은 [프로젝트 작업 나열](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 배포 나열]**

이 검색 모듈은 프로젝트의 배포 목록을 검색합니다.

필드에 대한 자세한 내용은 [프로젝트 배포 나열](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 문제 정보 나열]**

이 검색 모듈은 단일 문제에 대한 모든 참고 목록을 검색합니다.

필드에 대한 자세한 내용은 [프로젝트 문제 정보 나열](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 문제 나열]**

이 검색 모듈은 지정된 프로젝트의 모든 문제를 반환합니다.

필드에 대한 자세한 내용은 [프로젝트 문제 나열](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 이정표 나열]**

이 검색 모듈은 프로젝트의 모든 이정표를 검색합니다.

필드에 대한 자세한 내용은 [프로젝트 이정표 나열](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 파이프라인 나열]**

이 검색 모듈은 프로젝트의 모든 파이프라인을 검색합니다.

필드에 대한 자세한 내용은 [프로젝트 파이프라인 나열](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 저장소 태그 나열]**

이 검색 모듈은 프로젝트에서 저장소 태그 목록을 검색합니다. 이름별로 알파벳순으로 정렬됩니다.

필드에 대한 자세한 내용은 [프로젝트 저장소 태그 나열](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 변수 나열]**

이 검색 모듈은 프로젝트 변수 목록을 검색합니다.

필드에 대한 자세한 내용은 [프로젝트 변수 나열](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 프로젝트 나열]**

이 검색 모듈은 인증된 사용자가 멤버인 모든 프로젝트를 검색합니다.

필드에 대한 자세한 내용은 [모든 프로젝트 나열](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 목록 저장소 분기]**

이 모듈은 검색어별로 저장소 분기를 검색합니다.

필드에 대한 자세한 내용은 [목록 저장소 분기](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 목록 리포지토리 커밋]**

이 검색 모듈은 프로젝트의 저장소 커밋 목록을 검색합니다.

필드에 대한 자세한 내용은 [목록 리포지토리 커밋](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 리포지토리 기여자 나열]**

이 검색 모듈은 저장소 기여자 목록을 검색합니다.

필드에 대한 자세한 내용은 [기여자](https://docs.gitlab.com/ee/api/repositories.html#contributors) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 저장소 트리 나열]**

이 검색 모듈은 프로젝트의 저장소 파일 및 디렉토리 목록을 검색합니다.

필드에 대한 자세한 내용은 [저장소 트리 나열](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 완료한 대로 할 일을 표시하십시오]**

이 작업 모듈은 현재 사용자에 대해 해당 ID가 지정한 하나의 보류 중인 할 일 항목을 완료 상태로 표시합니다.

필드에 대한 자세한 내용은 [작업을 수행할 항목을 표시합니다.](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 기존 문제 참고 수정]**

문제에 대한 기존 메모를 수정합니다.

필드에 대한 자세한 내용은 [기존 문제 참고 수정](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 기존 병합 요청 메모 수정]**

병합 요청의 기존 메모를 수정합니다.

필드에 대한 자세한 내용은 [기존 병합 요청 메모 수정](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 기존 코드 조각 메모 수정]**

이 작업 모듈은 코드 조각의 기존 메모를 수정합니다.

필드에 대한 자세한 내용은 [기존 코드 조각 메모 수정](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 새 문제]**

이 작업 모듈은 새 프로젝트 문제를 만듭니다.

필드에 대한 자세한 내용은 [새 문제](https://www.integromat.com/en/help/app/gitlab) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 빌드 재생]**

이 작업 모듈은 수동 작업을 트리거하여 작업을 시작합니다.

필드에 대한 자세한 내용은 [작업 재생](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 커밋할 댓글 게시]**

이 작업 모듈은 커밋에 주석을 추가합니다.

필드에 대한 자세한 내용은 [커밋할 댓글 게시](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 변수 제거]**

이 작업 모듈은 프로젝트의 변수를 제거합니다.

필드에 대한 자세한 내용은 [변수 제거](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 빌드 다시 시도]**

이 작업 모듈은 커밋에서 단일 빌드를 다시 시도합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>새 연결을 만들려면 다음을 참조하십시오 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] Workfront Fusion으로 변환]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 프로젝트 ID]</td> 
   <td> <p>다시 시도할 빌드가 포함된 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 빌드 ID]</td> 
   <td> 다시 시도할 빌드를 선택합니다. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 파이프라인에서 실패한 작업 다시 시도]**

이 작업 모듈은 파이프라인에서 빌드를 다시 시도하지 못했습니다.

필드에 대한 자세한 내용은 [파이프라인에서 작업 다시 시도](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 변수 가져오기]**

이 모듈은 프로젝트의 특정 변수에 대한 세부 정보를 검색합니다.

필드에 대한 자세한 내용은 [변수 세부 사항 표시](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 릴리스 업데이트]**

이 작업 모듈은 릴리스를 업데이트합니다.

필드에 대한 자세한 내용은 [릴리스 업데이트](https://docs.gitlab.com/ee/api/releases/#update-a-release) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 병합 요청 업데이트]**

이 작업 모듈은 기존 병합 요청을 업데이트합니다. 대상 분기, 제목을 변경하거나 MR을 닫을 수도 있습니다.

필드에 대한 자세한 내용은 [병합 요청 업데이트](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) 에서 [!DNL GitLab] 설명서.

+++

+++**[!UICONTROL 변수 업데이트]**

이 작업 모듈은 프로젝트의 변수를 업데이트합니다.

필드에 대한 자세한 내용은 [변수 업데이트](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) 에서 [!DNL GitLab] 설명서.

+++
