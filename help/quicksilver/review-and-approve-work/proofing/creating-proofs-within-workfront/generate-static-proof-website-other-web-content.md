---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 웹 사이트 또는 기타 웹 컨텐츠에 대한 정적 증명 만들기
description: 웹 컨텐츠에 대한 기존 정적 증명의 새 버전이나 새로운 정적 증명을 생성할 수 있습니다. 웹 컨텐츠에는 스트리밍 비디오, HTML 애니메이션 또는 대화형 배너가 있는 광고와 같은 것들이 포함될 수 있지만, 정적 방정이 가능하도록 여러 스크린샷으로 잘립니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# 웹 사이트 또는 기타 웹 컨텐츠에 대한 정적 증명 만들기

웹 컨텐츠에 대한 기존 정적 증명의 새 버전이나 새로운 정적 증명을 생성할 수 있습니다. 웹 컨텐츠에는 스트리밍 비디오, HTML 애니메이션 또는 대화형 배너가 있는 광고와 같은 것들이 포함될 수 있지만, 정적 방정이 가능하도록 여러 스크린샷으로 잘립니다.

웹 사이트나 기타 웹 컨텐츠에 대한 정적 증명을 만들 때에는 다음 사항을 고려하십시오.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Select 또는 Premium</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">증명 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 웹 사이트 또는 기타 웹 컨텐츠에 대한 정적 증명 만들기

정적 증명을 작성하려면 웹 사이트에 공개적으로 액세스할 수 있어야 합니다(방화벽이 아님). 그렇지 않으면 조직허용 목록에 추가하다의 도메인에 Workfront 도메인이 포함되어야 합니다. Workfront은 암호로 보호된 웹 사이트를 정적 증명으로 캡처할 수 없습니다.

>[!TIP]
>
>인증 및 암호로 보호된 페이지를 사용해야 하는 내부 페이지에 대한 정적 교정이 아닌 대화형 교정이 좋습니다. 자세한 내용은 [대화형 콘텐츠 증명 개요](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. 새 웹 사이트 증명을 만들거나 기존 웹 사이트의 새 버전을 만들 프로젝트, 작업 또는 문제로 이동합니다.
1. 클릭 **문서** 왼쪽 패널에서 을 클릭합니다.
1. (조건부) 새 증명을 만드는 경우 **새로 추가**&#x200B;를 클릭한 다음 **증명** 나타납니다.
1. (조건부) 기존 증명의 새 버전을 만드는 경우:

   1. 새 버전을 만들 URL 증명 위로 마우스를 가져간 다음 주위의 연한 파란색 배경을 클릭하여 선택합니다.

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. 클릭 **새로 추가** > **버전** > **증명**.

1. 증명을 제공할 웹 사이트의 URL을 **파일 추가** 영역, 누르기 **Enter 키**.

   URL은 입력한 상자 아래에 나타납니다.

   ![](assets/url-name-appears-below-350x142.png)

1. 추가한 URL을 클릭합니다.

   웹 사이트 증명 구성 옵션이 나타납니다.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (선택 사항) 증명 이름을 웹 사이트 URL에서 다른 이름으로 변경하려면 **증명 이름.**
1. 확인 **스크린샷 캡처** 이 선택되고 다음 옵션 중 하나를 사용합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>스크린샷 해상도</strong> </td> 
      <td> <p>검토자가 증명을 볼 때 콘텐츠의 해상도를 조정하여 휴대폰, 태블릿, 모니터 등 다양한 크기의 장치에 표시되는 방식을 확인할 수 있습니다.</p> <p>여러 해상도를 선택하면 선택한 각 해상도에 대해 별도의 증명이 만들어집니다.</p> <p>참고: 검토자가 증명에 주석을 달 때 주석에는 주석이 언제 만들어졌는지 알려주는 해상도가 포함되어 있으므로 다른 검토자가 댓글과 연결된 해상도를 알 수 있습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>하위 페이지 찾기</strong> </td> 
      <td> <p>웹 사이트의 하위 페이지와 기본 페이지를 캡처합니다. 모두 선택 을 클릭하여 모든 페이지를 포함하거나 포함할 특정 페이지만 클릭할 수 있습니다. 더하기 및 빼기 단추를 사용하면 웹 사이트에서 하위 페이지 영역을 확장하고 닫을 수 있습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >작성한 증명의 후속 버전에 대해서는 캡처 스크린샷 설정을 변경할 수 없습니다.

1. 클릭 **완료**.

   8단계에서 여러 스크린샷 해상도를 선택한 경우 각 해상도의 스크린샷 세트가 목록에 포함됩니다. 이러한 스크린샷을 별도의 증명으로 생성하거나 하나의 증명으로 결합할 수 있습니다( 참조). 특히 정적 웹 사이트 증명을 만드는 경우 결합하는 것이 좋습니다.

   >[!NOTE]
   >
   >기존 URL 증명에 새 버전을 추가하는 경우 원래 증명 또는 이전 버전에서 구성된 모든 옵션은 이 버전에서 유지됩니다.

1. 클릭 **증명 만들기** 검토 프로세스 없이 간단한 증명을 만들 수 있습니다.\
   또는\
   고급 증명을 구성하여 계속합니다.

   * [기본 워크플로우를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [자동화된 워크플로우를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
