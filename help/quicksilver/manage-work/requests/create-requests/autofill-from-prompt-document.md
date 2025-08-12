---
title: 프롬프트 또는 문서를 사용하여 요청 자동 채우기
content-type: reference
description: AI를 사용하여 프롬프트를 입력하거나 문서를 제공하여 요청 필드를 자동으로 채울 수 있습니다.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: fd42ac97be05df9499ea3214642099738ccc69b1
workflow-type: tm+mt
source-wordcount: '1093'
ht-degree: 2%

---

# 프롬프트 또는 문서를 사용하여 요청 자동 채우기

>[!NOTE]
>
>* 이 기능은 다음 일정에 따라 공개 베타로 사용할 수 있습니다.
>
>   * 월별 릴리스: 2025년 9월 11일
>   * 분기별 릴리스: 2025년 10월 16일
>
>* 이 기능을 사용하려면 조직이 Workfront AI Assistant를 사용하기 위한 요구 사항을 충족해야 합니다. 자세한 내용은 [AI Assistant의 필수 구성 요소](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)를 참조하십시오.

AI는 사용자가 입력하는 프롬프트에 따라 요청 필드를 자동으로 채우는 데 도움이 됩니다. 또한 업로드된 문서와 같은 텍스트를 기반으로 필드를 채울 수도 있습니다. 요청을 제출하기 전에 이러한 제안을 승인하거나 거부할 수 있습니다.

자동 채우기는 이미 입력한 필드를 덮어쓰지 않습니다.

사용자는 액세스 권한이 없는 데이터에 대한 제안을 받지 않습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 기여자 이상</p>
   또는
   <p>현재: 요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문제에 대한 액세스 편집</p>  </td> 
  </tr> 
   <td role="rowheader">개체 권한</td> 
   <td><p>요청 대기열에 요청을 추가하는 액세스 권한</p> <p>기존 요청에 대한 이상의 권한 보기</p> <p>요청 대기열 설정에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a>를 참조하십시오. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

프롬프트 또는 문서를 사용하여 요청을 자동으로 채우려면 다음 중 **모두**&#x200B;을(를) 적용해야 합니다.

* 조직이 Adobe IMS(Identity Management System)로 마이그레이션되었어야 합니다.
* Adobe 통합 경험을 활성화해야 합니다.
* 조직에 Select, Prime 또는 Ultimate Workfront 플랜이 있어야 합니다.
* Adobe은 파일에 서명된 Adobe Gen AI 계약이 있어야 합니다.

  계약 서명에 대한 자세한 내용은 AI Assistant 개요 문서의 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.
* 조직의 시스템 설정에서 AI Assistant를 활성화해야 합니다. Workfront 관리자가 관리합니다.

  시스템 설정에서 AI Assistant를 활성화하는 방법에 대한 자세한 내용은 [AI Assistant 활성화 또는 비활성화](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)를 참조하십시오.

## 텍스트 프롬프트에서 제안 받기

자동 채우기는 전자 메일과 같은 텍스트를 기반으로 필드 값을 제안할 수 있습니다. 텍스트 블록에 붙여넣으면 Workfront은 텍스트를 처리하여 텍스트를 기반으로 필드 값을 제안합니다.

예를 들어, 이메일에 &quot;6월 1일 날짜입니다&quot;가 포함되어 있고 요청 양식에 기한 필드가 있는 경우, Workfront은 해당 필드 값에 6월 1일을 제안합니다.

이 유형의 제안은 유사한 컨텍스트에 대한 이전 요청도 확인합니다. 예를 들어 프롬프트에서 특정 클라이언트에 대한 요청이라고 언급하면 Workfront에서 이전 요청을 기반으로 해당 클라이언트에 대한 청구 주소를 자동으로 찾아 입력할 수 있습니다.

전체 폼이나 폼의 한 구역에 적용할 텍스트에 붙여넣을 수 있습니다.

붙여넣은 텍스트 프롬프트에 따라 제안을 사용하려면 다음을 수행합니다.

1. 요청 만들기를 시작합니다.

   지침은 [요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)을 참조하세요.

1. 전체 양식에 텍스트 프롬프트를 적용하려면 양식 이름 아래의 AI 아이콘 ![AI 아이콘](assets/request-prompt-icon.png)을 클릭합니다.

   또는

   단일 섹션에 대한 텍스트 프롬프트를 적용하려면 섹션 이름 옆에 있는 AI 아이콘 ![AI 아이콘](assets/request-prompt-icon.png)을 클릭합니다.

1. 프롬프트 상자에 텍스트를 붙여넣습니다.
1. **양식 채우기**&#x200B;를 클릭합니다.

   Workfront은 양식에 대한 제안을 생성합니다.
1. 각 필드 제안에 대해 해당 필드에 대해 **수락** 또는 **거부**&#x200B;을 선택합니다.

   ![제안 수락 또는 거부](assets/accept-reject-suggestion.png)

   또는

   모든 제안을 수락하거나 거부하려면 페이지 맨 위에서 **모두 수락** 또는 **모두 거부**&#x200B;를 선택하십시오.

   >[!NOTE]
   >
   >검토되지 않은 제안은 요청을 제출할 때 자동으로 수락됩니다.

## 업로드한 문서에 따라 제안 받기

자동 채우기는 업로드하는 문서에 따라 필드 값을 제안할 수 있습니다.

이 유형의 제안은 유사한 컨텍스트에 대한 이전 요청도 확인합니다. 예를 들어 프롬프트에서 특정 클라이언트에 대한 요청이라고 언급하면 Workfront에서 이전 요청을 기반으로 해당 클라이언트에 대한 청구 주소를 자동으로 찾아 입력할 수 있습니다.

### 문서 업로드 보호

#### 지원되는 파일 유형

지원되는 파일 유형은 다음과 같습니다.

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### 지원되는 파일 크기

각 파일의 크기는 최대 100MB입니다

#### 파일 수

최대 50개의 파일(페이지, 슬라이드 또는 시트)을 업로드할 수 있습니다.

>[!IMPORTANT]
>
>문서는 각각 별도의 파일로 간주되는 일련의 이미지로 변환됩니다.
>
>예를 들어 50개의 슬라이드가 있는 PowerPoint 또는 10개의 페이지가 있는 Word 문서 5개를 업로드할 수 있습니다.

#### 지원되는 필드 유형

Workfront 필드 유형은 지정된 필드를 자동으로 채울 수 있는지 여부에 영향을 줍니다.

<table>
<tr>
<td><b>지원되는 </b><br> 자동 채우기는 채울 수 있습니다.</td>
<td><b>지원되지 않음</b> <br>자동 채우기가 채워지지 않음</td>
</tr>
<tr>
<td>
<ul>
<li>한 줄 텍스트</li>
<li>텍스트 영역 또는 단락</li>
<li>날짜 필드</li>
<li>확인란</li>
<li>라디오 버튼</li>
<li>단일 및 다중 선택 드롭다운</li>
</ul>
</td>
<td><li>타이프 어헤드</li>
<li>외부 조회</li>
<li>내부 조회</li>
<li>참조</li>
<li>WF Planning 포함 필드</li>
</ul>
</td>
</tr>
</table>

#### 기타 모범 사례

요청 자동 채우기에 대한 문서를 업로드할 때 다음 사항을 고려하십시오.

* 자동 채우기는 현재 라틴 알파벳에 맞게 최적화되어 있습니다.
* 8포인트 이상의 텍스트 크기를 사용하는 것이 좋습니다.
* 자동 채우기에는 회전되거나 왜곡된 이미지, 그래프 및 이미지의 개체에 대한 공간적 이유 사용 또는 카운트와 같은 문서의 이미지에 어려움이 있을 수 있습니다.
* 항상 그렇듯이 요청을 제출하기 전에 결과의 정확성을 확인하는 것이 좋습니다.

### 문서를 업로드하여 요청 자동 채우기

전체 양식이나 양식의 단일 섹션에 적용할 문서를 업로드할 수 있습니다.

1. 요청 만들기를 시작합니다.

   지침은 [요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)을 참조하세요.

1. 전체 양식에 문서를 적용하려면 양식 이름 아래의 AI 아이콘 ![AI 아이콘](assets/request-prompt-icon.png)을 클릭합니다.

   또는

   단일 섹션에 대한 문서를 적용하려면 섹션 이름 옆에 있는 AI 아이콘 ![AI 아이콘](assets/request-prompt-icon.png)을 클릭합니다.

1. **파일 업로드**&#x200B;를 클릭한 다음 파일 관리자에서 파일을 선택합니다.

   또는

   파일 관리자에서 **요청 양식을 자동으로 채우도록 파일 업로드** 상자로 문서를 드래그합니다.
1. **양식 채우기**/**섹션 채우기**&#x200B;를 클릭합니다.

   Workfront은 양식에 대한 제안을 생성합니다.
1. 각 필드 제안에 대해 해당 필드에 대해 **수락** 또는 **거부**&#x200B;을 선택합니다.

   ![제안 수락 또는 거부](assets/accept-reject-suggestion.png)

   또는

   모든 제안을 수락하거나 거부하려면 페이지 맨 위에서 **모두 수락** 또는 **모두 거부**&#x200B;를 선택하십시오.

   >[!NOTE]
   >
   >검토되지 않은 제안은 요청을 제출할 때 자동으로 수락됩니다.

## 문제 해결

예상되는 제안을 받지 못하는 경우 다음 중 하나로 인해 발생할 수 있습니다.

* 이전 요청의 필드 값을 제안하려면 시스템에 최소 1개월 이상의 요청 데이터가 있어야 합니다.
* 제안 사항을 가져오기 위해 문서를 업로드할 때 문서 업로드 가드레일을 따르지 않았을 수 있습니다. 자세한 내용은 이 문서에서 [문서 업로드 가드레일](#document-upload-guardrails)을(를) 참조하십시오.
