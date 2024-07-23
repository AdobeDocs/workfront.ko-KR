---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 웹 사이트 또는 기타 웹 컨텐츠에 대한 정적 증명 만들기
description: 웹 콘텐츠에 대한 새 정적 증명 또는 기존 정적 증명의 새 버전을 생성할 수 있습니다. 웹 콘텐츠에는 스트리밍 비디오가 포함된 광고, HTML 애니메이션 또는 대화형 배너 등이 포함될 수 있지만, 정적 증명을 위해 여러 스크린샷으로 잘립니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 웹 사이트 또는 기타 웹 컨텐츠에 대한 정적 증명 만들기

웹 콘텐츠에 대한 새 정적 증명 또는 기존 정적 증명의 새 버전을 생성할 수 있습니다. 웹 콘텐츠에는 스트리밍 비디오가 포함된 광고, HTML 애니메이션 또는 대화형 배너 등이 포함될 수 있지만, 정적 증명을 위해 여러 스크린샷으로 잘립니다.

웹 사이트 또는 기타 웹 컨텐츠에 대한 정적 증명을 만들 때 다음 사항을 고려하십시오.

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

+++

## 웹 사이트 또는 기타 웹 컨텐츠에 대한 정적 증명 만들기

정적인 증명을 만들려면 웹 사이트에 공개적으로 액세스해야 합니다(방화벽 뒤가 아님). 또는 조직의 허용 목록에 추가하다 도메인에 Workfront 도메인이 포함되어야 합니다. Workfront은 암호로 보호된 웹 사이트를 정적 증명으로 캡처할 수 없습니다.

>[!TIP]
>
>인증이 필요한 내부 페이지 및 암호로 보호된 페이지에는 정적 증명보다 대화형 증명이 좋습니다. 자세한 내용은 [대화형 콘텐츠 증명 개요](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)를 참조하십시오.

1. 새 웹 사이트 증명 또는 기존 웹 사이트의 새 버전을 만들 프로젝트, 작업 또는 문제로 이동합니다.
1. 왼쪽 패널에서 **문서**&#x200B;를 클릭합니다.
1. (조건부) 새 증명을 만드는 경우 표시되는 메뉴에서 **새로 추가**&#x200B;를 클릭한 다음 **증명**&#x200B;을 클릭합니다.
1. (조건부) 기존 증명의 새 버전을 만드는 경우:

   1. 새 버전을 만들 URL 증명을 마우스로 가리킨 다음, 해당 버전을 둘러싼 연한 파란색 배경을 클릭하여 선택합니다.

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. **새로 추가** > **버전** > **증명**&#x200B;을 클릭합니다.

1. **파일 추가** 영역에 증명하려는 웹 사이트의 URL을 입력한 다음 **Enter**&#x200B;를 누릅니다.

   >[!NOTE]
   >
   > URL은 1,000자 미만이어야 합니다.

1. 추가한 URL을 클릭합니다.

   웹 사이트 증명 구성 옵션이 표시됩니다.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (선택 사항) 웹 사이트 URL에서 증명 이름을 다른 이름으로 변경하려면 **증명 이름을 입력하십시오.**
1. **스크린샷 캡처**&#x200B;를 선택하고 다음 옵션을 사용하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>스크린샷 해상도</strong> </td> 
      <td> <p>검토자가 증명을 볼 때 콘텐츠의 해상도를 조정하여 휴대폰, 태블릿 및 모니터와 같이 다양한 크기의 장치에서 어떻게 표시되는지 볼 수 있습니다.</p> <p>여러 개의 해상도를 선택하면 선택한 각 해상도에 대해 별도의 증명이 만들어집니다.</p> <p>참고: 검토자가 증명에 댓글을 달면 댓글에는 댓글이 언제 작성되었는지 보여 주는 해결 방법이 포함되어 다른 검토자는 댓글과 연결된 해결 방법을 알 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>하위 페이지 찾기</strong> </td> 
      <td> <p>웹 사이트의 하위 페이지와 기본 페이지를 캡처합니다. 모두 선택 을 클릭하여 모든 페이지를 포함하거나, 포함하려는 특정 페이지만 클릭할 수 있습니다. 더하기 및 빼기 단추를 사용하여 웹 사이트의 하위 페이지 영역을 확장하고 닫을 수 있습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >생성한 증명의 후속 버전에 대해 캡처 스크린샷 설정을 변경할 수 없습니다.

1. **완료**&#x200B;를 클릭합니다.

   8단계에서 여러 스크린샷 해상도를 선택한 경우 각 해상도에 대한 스크린샷 세트가 목록에 포함됩니다. 이러한 스크린샷을 별도의 증명으로 생성하거나 하나의 증명으로 결합할 수 있습니다(참조)  .). 특히 정적 웹 사이트 증명을 만드는 경우 이러한 증명을 결합하는 것이 좋습니다.

   >[!NOTE]
   >
   >기존 URL 증명에 새 버전을 추가하는 경우 원래 증명 또는 이전 버전에 구성된 모든 옵션이 이 버전에서 유지됩니다.

1. 검토 프로세스가 없는 간단한 증명을 만들려면 **증명 만들기**&#x200B;를 클릭하십시오.\
   또는\
   고급 증명을 구성하여 계속합니다.

   * [기본 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [자동화된 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
