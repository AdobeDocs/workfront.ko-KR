---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 여러 페이지로 된 증명 만들기
description: 여러 파일을 하나의 다중 페이지 증명으로 결합할 수 있습니다. 검토자는 증명 뷰어의 탐색 도구를 사용하여 다중 페이지 증명에서 페이지를 탐색할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# 여러 페이지로 된 증명 만들기

여러 파일을 하나의 다중 페이지 증명으로 결합할 수 있습니다. 검토자는 증명 뷰어의 탐색 도구를 사용하여 다중 페이지 증명에서 페이지를 탐색할 수 있습니다.

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

&#42;보유 중인 플랜, 라이선스 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

+++

## 여러 페이지로 된 증명 만들기

이 옵션을 활성화하면 하나의 증명에서 정적 파일 및 웹 사이트를 사용할 수 있습니다. 이 옵션이 비활성화되면 모든 문서와 웹 사이트가 개별 증명으로 생성되며 한 번에 최대 100개의 파일을 업로드할 수 있습니다.

다중 페이지 증명을 만들려면 다음 작업을 수행하십시오.

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 섹션을 클릭합니다.
1. **새로 추가** > **증명** 을 클릭합니다.
1. 파일을 드래그 앤 드롭하거나 파일 탐색기에서 찾아 선택합니다. 한 번에 최대 50개의 파일을 업로드할 수 있습니다. 파일 제한에 대한 자세한 내용은 이 문서의 [고려 사항](#considerations) 섹션을 참조하십시오.

   >[!NOTE]
   >
   >비디오 및 대화형 웹 사이트를 포함한 대화형 파일은 하나의 증명으로 결합할 수 없습니다.

1. **단일 증명**&#x200B;에서 옵션을 사용하도록 설정합니다. **호환되는 모든 파일을 단일 증명으로 결합**.
1. **증명 이름** 필드에 결합된 증명의 새 이름을 지정하십시오.
1. (선택 사항) 업로드한 파일 목록에서 파일을 드래그하여 순서를 변경합니다. 파일 순서는 결합된 증명의 페이지 순서입니다.
1. (선택 사항) 새 증명 페이지에서 단일 파일을 제거하려면 파일 위로 마우스를 가져간 후 오른쪽에 나타나는 **휴지통** 아이콘을 클릭합니다.

   또는

   업로드된 모든 파일을 한 번에 삭제하려면 목록의 오른쪽 상단에 있는 **모두 삭제**&#x200B;를 클릭합니다.

1. 모든 파일이 업로드되면 기본 증명을 구성할 것인지 아니면 자동화된 증명을 구성할 것인지 결정해야 합니다.

   * 기본 증명을 사용하여 증명을 원하는 만큼 추가할 수 있지만 단계로 구성되지 않습니다. 추가하는 모든 검토자는 증명을 만든 직후에 액세스할 수 있습니다. 기본 증명을 구성하려면 [기본 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)를 참조하십시오.
   * 자동화된 증명을 사용하면 증명이 여러 단계에서 이동하고 Adobe Workfront에서 검토할 시점이 되면 각 사용자에게 알립니다. 자동화된 증명을 구성하려면 [자동화된 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)를 참조하십시오.

## 고려 사항 {#considerations}

파일을 하나의 증명으로 결합할 때는 다음 사항을 고려하십시오.

* 최대 500개의 개별 파일을 업로드할 수 있습니다.
* 서로 다른 유형의 정적 파일(예: PDF, JPG, DOC, PPT, EXC)을 최대 2,000페이지까지 결합할 수 있습니다.
* 정적 웹 캡처를 결합할 수 있습니다.
* GIF 파일을 결합할 수 있지만 애니메이션 GIF은 정적 파일로 처리됩니다.
* AV 파일과 대화형 웹 캡처를 결합할 수 없습니다.
* 증명의 썸네일 이미지는 증명의 첫 페이지에서 가져온 것입니다([Workfront Proof에서 증명 세부 정보 관리](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) 참조).
* 증명 세부 정보 페이지에서 증명을 만들기 위해 결합된 파일 이름을 확인할 수 있습니다. 자세한 내용은 [Workfront Proof에서 증명 세부 정보 관리](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)를 참조하십시오.
* 증명에 원본 파일을 다운로드하는 옵션이 활성화되어 있으면 증명을 .zip 파일로 만들기 위해 결합된 모든 파일을 다운로드할 수 있습니다. 자세한 내용은  [Workfront Proof에 저장된 파일을 다운로드합니다](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
