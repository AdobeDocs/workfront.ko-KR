---
product-area: documents
navigation-topic: approvals
title: AI 검토자를 위한 브랜드 설정
description: AI 검토자를 위한 브랜드 설정
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cf1d4bfeedb94e8607dad47177d804169254ee85
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 5%

---

# AI 검토자를 위한 브랜드 설정

>[!IMPORTANT]
>
>이 기능은 현재 베타 버전입니다.

AI 검토자는 브랜드 가이드라인을 사용하여 검토 과정에서 콘텐츠를 평가합니다. 브랜드 지침이 포함된 PDF 파일을 업로드하거나 브랜드 요소를 수동으로 입력하여 Workfront에서 브랜드를 만들 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
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
   <td role="rowheader">Admin Console 권한</td> 
   <td> <p>GenStudio Brand Manager여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## 전제 조건

* 조직이 Adobe IMS(Identity Management System)로 마이그레이션되었어야 합니다.
* Workfront 인스턴스에는 통합 승인이 활성화되어 있어야 합니다.
  <!--* Your organization must have GenStudio Foundation.-->
* Adobe은 파일에 서명된 Adobe Gen AI 계약이 있어야 합니다.
계약 서명에 대한 자세한 내용은 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.

## PDF을 사용하여 브랜드 만들기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **검토 및 승인** > **브랜드**(으)로 이동합니다.
1. 화면 오른쪽 상단에서 **브랜드 추가**&#x200B;를 클릭합니다.
1. 브랜드 이름을 지정합니다.
1. PDF 업로드 를 클릭하여 브랜드 파일을 업로드합니다.
   ![브랜드 pdf 업로드](assets/upload-PDF.png)
1. **계속**&#x200B;을 클릭합니다.
1. 브랜드 가이드라인이 포함된 PDF 파일을 하나 이상 업로드한 다음 **브랜드 추가**&#x200B;를 클릭합니다.
1. 파일이 업로드되면 추출한 브랜드 요소를 검토하여 브랜드 지침을 준수하는지 확인하십시오.

   >[!IMPORTANT]
   >
   >지침은 파일과 생성 AI 기술을 사용하여 생성되며 정확하지 않을 수 있습니다. 이 브랜드를 게시하기 전에 누락되거나 잘못된 세부 정보에 대해 추출된 지침을 검토하고 편집하십시오.

1. 완료되면 **게시**&#x200B;를 클릭하여 AI 검토자가 브랜드를 사용할 수 있도록 합니다.

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


1. 완료되면 **게시**&#x200B;를 클릭하여 AI 검토자가 브랜드를 사용할 수 있도록 합니다.
