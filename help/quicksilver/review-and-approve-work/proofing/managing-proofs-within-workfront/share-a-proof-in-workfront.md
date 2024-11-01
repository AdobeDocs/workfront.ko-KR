---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Adobe Workfront 내에서 증명 공유
description: 문서를 공유하거나 증명에 사용자를 추가하여 Adobe Workfront 내에서 증명 문서를 공유할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: aaf5beb8692b2fdbb797ba908796d78b4ee8866c
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# Adobe Workfront 내에서 증명 공유

문서를 공유하거나 증명에 사용자를 추가하여 Adobe Workfront 내에서 증명 문서를 공유할 수 있습니다.

이 문서에 설명된 대로 증명을 공유하는 경우 수신자는 문서와 증명에 대해 동일한 액세스 권한을 갖습니다. 또한 수신자에게 증명 승인을 요청할 수 있습니다.

>[!TIP]
>
>증명 뷰어 내에서 증명을 공유할 수도 있습니다. 자세한 내용은 [증명 뷰어에서 증명 공유](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 플랜: Pro 이상</p> <p>또는</p> <p>기존 플랜: Select 또는 Premium</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자에 대해 증명이 활성화되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">교정쇄 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">교정쇄 역할</td> 
   <td>작성자 또는 중재자</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

+++

## 증명 링크 공유

증명 링크를 공유하면 Workfront 사용자에게 보기 액세스 권한이 부여됩니다. 사용자는 Workfront 로그인 자격 증명을 사용하여 증명에 댓글을 달고 증명에 대한 이메일 알림을 구독할 수 있습니다. 증명이 없는 사용자는 이메일 주소와 디스플레이 이름을 사용하여 댓글을 달고 구독할 수 있습니다.

>[!IMPORTANT]
>
>공개 URL 또는 포함 코드를 통한 증명 공유 허용 설정을 활성화해야 합니다.

1. 사용자와 공유할 증명이 포함된 문서를 선택합니다.

   문서를 하나만 선택할 수 있습니다. 여러 문서에 대한 링크를 동시에 공유할 수 없습니다.

1. **공유** > **증명 링크**&#x200B;를 클릭합니다.
1. 표시되는 **증명 링크** 상자에서 다음 중 하나를 수행합니다.

   * 클립보드에 링크를 복사하려면 **링크 복사**&#x200B;를 클릭하세요.

     이제 채팅 또는 이메일 애플리케이션과 같은 서드파티 도구를 통해 링크를 배포할 수 있습니다.

   * Adobe Workfront에서 직접 링크를 이메일로 보내려면 다음을 수행합니다.

      1. **또는**(으)로 연결된 전자 메일 링크에서 입력을 시작하고 받는 사람의 이름을 선택합니다. 또는 공유할 외부 사용자의 이메일 주소를 지정합니다.

         >[!NOTE]
         >
         >증명을 공유할 때 별칭 이메일이 표시되는 경우, 해당 별칭 이메일이 있는 경우 원본 이메일을 입력하여 새 게스트 사용자를 만들지 마십시오.

      1. 다음 옵션 중에서 선택합니다.

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">공개 링크 보내기</td>
            <td><p>이메일 알림에 사용자가 사용 중인 증명 뷰어 내의 증명으로 사용자를 안내하고 보기 액세스 권한을 부여하는 버튼을 포함합니다.</p><p>증명에 대해 <strong>공개 URL 또는 포함 코드를 통해 증명 구독</strong>이 꺼져 있으면 사용자가 Workfront 로그인 자격 증명으로 로그인하여 증명에 주석을 추가할 수 있습니다. 이 기능이 켜지면 이메일 주소와 이름을 제공하는 모든 사람(암호 필요 없음)이 서명하고 증명에 주석을 추가할 수 있습니다.</p></td>
           </tr>
           <tr>
            <td role="rowheader">다운로드 링크 보내기</td>
            <td>사용자에게 파일 세부 사항, 파일 이름 및 파일 크기를 제공하고 파일이 인라인으로 표시되는 다운로드 페이지로 안내하는 이메일 알림의 버튼을 포함합니다. 사용자는 다운로드 페이지에서 다운로드 링크를 클릭하여 파일을 다운로드할 수 있습니다.</td>
           </tr>
           <tr>
            <td role="rowheader">사용자 정의 메시지 추가</td>
            <td>이메일 알림에 대한 사용자 정의 제목과 본문을 지정할 수 있습니다.</td>
           </tr>
          </tbody>
         </table>

      1. **보내기**&#x200B;를 클릭합니다.

         수신자는 증명 및 포함하기로 선택한 버튼에 대한 정보가 포함된 이메일 알림을 받게 됩니다.

         ![](assets/proof-share-email-350x87.png)

## 증명에 사용자 추가

증명에 대한 편집 권한이 있는 경우 모든 Workfront 사용자를 증명에 추가할 수 있습니다. 증명에 여러 단계가 있는 경우 사용자를 개별 단계에 추가합니다

>[!WARNING]
>
>이 문서에 나열된 방법 외에도 기존 증명의 업데이트 탭에 있는 댓글에 사용자를 태그 지정하여 증명에 사용자를 추가할 수 있습니다. 그러나 이러한 방식으로 증명에 추가된 사용자는 증명의 워크플로우에 추가된 후 다시 태그가 지정되지 않으면 이메일 알림을 받지 못합니다.
>
>따라서 댓글에 태그를 지정하지 말고 아래 나열된 방법 중 하나를 통해 증명에 사용자를 추가하는 것이 좋습니다.
>

>[!NOTE]
>
>사용자에 대해 증명을 활성화 및 비활성화할 수 있는 기존 Workfront 플랜을 사용하는 경우 다음 사항을 염두에 두십시오.
>
>* 증명을 검토하기 위해 수신자가 증명을 활성화할 필요가 없습니다.
>* 자동화된 워크플로가 활성화되고 Workfront에서 증명이 활성화되지 않은 사용자를 증명에 추가하면 자동화된 워크플로 내에 새 단계가 생성됩니다. 추가하려는 사용자가 증명을 처음 볼 때 이 새 단계에 자동으로 추가됩니다. 자세한 내용은 [자동화된 워크플로 개요](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)를 참조하십시오.
>

### 문서 탭에서 기존 증명에 사용자 추가

1. 사용자를 추가할 증명이 포함된 문서를 선택합니다.
1. 증명에 자동화된 워크플로(단계)가 없는 경우 단계 1 섹션의 오른쪽 위 모서리에 있는 **자세히** 아이콘을 클릭한 다음 드롭다운 메뉴에서 **공유**&#x200B;를 클릭합니다.

   또는

   증명에 자동화된 워크플로가 있는 경우 검토자를 추가할 단계의 오른쪽 위 모서리에 있는 **자세히** 아이콘을 클릭한 다음, 드롭다운 메뉴에서 **공유**&#x200B;를 클릭합니다.

1. **공유**&#x200B;에 표시되는 **이 버전 공유** 상자에서 증명을 공유할 사용자의 이름 또는 전자 메일 주소를 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.

1. (선택 사항) 증명에 여러 사용자를 추가하려면 이 단계를 반복합니다.
1. (선택 사항) 검토자에 대한 기한을 설정합니다.
1. (선택 사항) 검토자에게 증명에 추가했음을 알리려면 **전자 메일로 사람들에게 알림**&#x200B;을 선택해야 합니다.
1. (선택 사항) 전자 메일에 **사용자 지정 메시지를 추가**&#x200B;합니다.
1. 모든 검토자를 추가했으면 **공유**&#x200B;를 클릭합니다.

### 증명 뷰어에서 기존 증명에 사용자 추가

웹 증명 뷰어와 데스크탑 증명 뷰어에서 증명을 검토하는 동안 증명에 사용자를 추가할 수 있습니다.

자세한 내용은 문서 [증명 뷰어에서 증명 공유](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)에서 [사용자를 추가하여 증명 공유](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)를 참조하십시오.

## 증명 승인에 대한 보고서

Workfront 내에서 공유된 증명 승인에 대해 보고하는 보고서를 만들 수 있습니다. 이 보고서는 시스템에 다음과 같은 증명 승인 정보를 제공합니다.

* 승인을 위해 제출된 문서
* 승인자 이름
* 증명 버전
* 교정쇄 ID
* 증명 생성일

[사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)에 설명된 대로 개체를 기반으로 보고서를 만들 때 이 승인에 액세스합니다.

증명 승인 개체 보고서에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)의 [개체에 대한 보고서](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 섹션을 참조하십시오.

## 공유 증명 승인

사용자가 증명에 귀하를 추가하고 자동화된 워크플로를 사용하여 승인자 역할 또는 검토자 및 승인자 역할을 부여하면 홈 영역의 내 승인 위젯에 승인 요청이 표시됩니다. 그런 다음 증명을 보고 Workfront에서 직접 증명에 대한 승인 결정을 내릴 수 있습니다.

내 승인 위젯에서 승인 결정을 내리는 방법에 대한 자세한 내용은 [작업 승인](../../../review-and-approve-work/manage-approvals/approving-work.md)에서 [홈 영역에서 작업 승인](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) 또는 [작업 승인](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area)을 참조하십시오.
