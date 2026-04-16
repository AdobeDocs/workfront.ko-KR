---
product-area: documents
navigation-topic: approvals
title: 콘텐츠 검토자를 위한 브랜드 만들기 및 관리
description: 콘텐츠 검토자를 위한 브랜드 만들기 및 관리
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 243aa2b0893e3034d37b959384a50b8a5e4a4bf0
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 3%

---

# 콘텐츠 검토자를 위한 브랜드 만들기 및 관리

콘텐츠 검토자는 브랜드 지침을 사용하여 검토 프로세스 중에 콘텐츠를 평가합니다. 브랜드 지침이 포함된 PDF 파일을 업로드하거나 브랜드 요소를 수동으로 입력하여 Workfront에서 브랜드를 만들 수 있습니다.

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
   <td> <p>표준</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자여야 합니다.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console 권한*</td> 
   <td> <p>GenStudio 브랜드 관리자여야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요구 사항

* Workfront 인스턴스에는 통합 승인이 활성화되어 있어야 합니다.

* 조직에 GenStudio Foundation이 있어야 합니다.
   * Workfront의 컨텐츠 검토자는 자산 검토 및 승인 워크플로에 GenStudio Foundation에서 사용할 수 있는 기능을 제공합니다. 작업을 완료하기 위해 GenStudio Foundation에 직접 액세스할 필요는 없습니다. 콘텐츠 검토자를 통해 GenStudio Foundation 기능에 대한 액세스는 Workfront 계약 조건에 해당됩니다.
* Adobe은 파일에 서명된 Adobe Gen AI 계약이 있어야 합니다.
계약 서명에 대한 자세한 내용은 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.


## 전제 조건

1. 브랜드를 만들려면 먼저 Admin Console 및 Workfront 액세스 수준에서 브랜드 권한에 대한 액세스 권한을 부여해야 합니다. 지침은 [브랜드 사용 권한에 대한 액세스 권한 부여](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)를 참조하십시오.


## PDF을 사용하여 브랜드 만들기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **검토 및 승인** > **브랜드**(으)로 이동합니다.
1. 화면 오른쪽 상단에서 **브랜드 추가**&#x200B;를 클릭합니다.
1. 브랜드 이름을 지정합니다.
1. 브랜드 파일을 업로드하려면 **PDF 업로드**를 클릭하세요.
   ![브랜드 pdf 업로드](assets/upload-PDF.png)
1. **계속**&#x200B;을 클릭합니다.
1. 브랜드 가이드라인이 포함된 PDF 파일을 하나 이상 업로드한 다음 **브랜드 추가**&#x200B;를 클릭합니다.
1. 파일이 업로드되면 추출한 브랜드 요소를 검토하여 브랜드 지침을 준수하는지 확인하십시오.

   >[!IMPORTANT]
   >
   >지침은 파일과 생성 AI 기술을 사용하여 생성되며 정확하지 않을 수 있습니다. 이 브랜드를 게시하기 전에 누락되거나 잘못된 세부 정보에 대해 추출된 지침을 검토하고 편집하십시오.

1. 완료되면 **게시**&#x200B;를 클릭하여 콘텐츠 검토자가 브랜드를 사용할 수 있도록 합니다.

## 수동으로 브랜드 만들기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **검토 및 승인** > **브랜드**(으)로 이동합니다.
1. 화면 오른쪽 상단에서 **브랜드 추가**&#x200B;를 클릭합니다.
1. 브랜드 이름을 지정합니다.
1. 개별 요소로 브랜드를 만들려면 **수동으로 추가**&#x200B;를 클릭하십시오.
1. 필요에 따라 브랜드 세부 사항을 입력합니다. 다음 요소를 추가할 수 있습니다.

   <table>
    <tr>
        <td>사용 시기</td>
        <td>마케터에게 이 브랜드를 사용할 시기를 알려주십시오.</td>
    </tr>
    <tr>
        <td>음성 지침</td>
        <td>브랜드 보이스의 음색과 스타일에 대한 지침을 제공합니다.</td>
    </tr>
    <tr>
        <td>이미지 지침</td>
        <td>브랜드 정체성에 맞는 이미지 유형을 지정합니다.</td>
    </tr>
    <tr>
        <td>채널 지침</td>
        <td>브랜드 커뮤니케이션에 적합한 채널에 대해 간략히 설명합니다.</td>
    </tr>
    <tr>
        <td>로고</td>
        <td>브랜드와 관련된 공식 로고를 포함합니다.</td>
    </tr>
    <tr>
        <td>색상</td>
        <td>브랜드 색상 팔레트를 지정합니다.</td>
    </tr>
    </table>

   ![수동으로 브랜드 요소 추가](assets/brand-elements.png)


1. 완료되면 **게시**&#x200B;를 클릭하여 콘텐츠 검토자가 브랜드를 사용할 수 있도록 합니다.


## 브랜드 지침 작성에 대한 우수 사례

*  측정 가능한 기준을 설명하는 브랜드 지침을 작성하십시오. 콘텐츠 검토자는 콘텐츠를 문자 그대로 평가하므로 객관적인 규칙이 주관적인 규칙보다 더 일관된 점수를 생성합니다.

* 지침에서 &quot;회피&quot;, &quot;유지&quot; 또는 &quot;확인&quot;과 같은 단어를 찾습니다. 이는 종종 강화할 수 있는 규칙을 나타냅니다. 모호한 지침을 특정 단어, 형식 또는 제한 목록으로 바꿉니다. 예를 들어 &quot;일반적인 스키 클리셰를 피하십시오&quot;를 &quot;gnar,&#39; &#39;pow,&#39; 또는 &#39;shred&#39;를 사용하지 마십시오&quot;로 바꿉니다.

* 주관성을 제거할 수 없다면 범위를 좁히세요. 광범위한 형용사를 특정한 제한으로 바꾸십시오. 예를 들어, &quot;직접적이고 행동지향적&quot;은 &quot;직접적이고 행동지향적&quot;이 됩니다; filler words를 생략하고 언어를 헤징합니다.&quot;