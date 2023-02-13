---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: XD 대지를 문서로 Workfront에 업로드
description: 문서를 문서로 업로드하여 빠른 검토 및 승인을 얻거나 Adobe Workfront에 저장할 수 있습니다.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# 업로드 [!DNL XD] 문서에 대한 문서로 보드 [!DNL Workfront]

문서를 문서로 업로드하여 빠른 검토 및 승인을 얻거나 간단히 저장할 수 있습니다 [!DNL Adobe Workfront].

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">제품</td> 
   <td>다음을 수행해야 합니다. [!DNL Adobe Creative Cloud] 라이센스 [!DNL Workfront] 라이센스.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>[!UICONTROL Documents]에 대한 액세스 편집</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서를 업로드할 개체에 액세스할 수 있는 [!UICONTROL 보기] 이상입니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

* 을(를) 설치해야 합니다. [!DNL Adobe Workfront for XD] 플러그인을 사용하여 XD 아트 보드를 문서로 Workfront에 업로드할 수 있습니다.

자세한 내용은 [설치 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## 새 문서 추가

1. 을(를) 클릭합니다. **[!UICONTROL 메뉴]** 오른쪽 상단 모서리의 아이콘을 클릭한 다음 **[!UICONTROL 작업 목록]**. 메뉴를 사용하여 상위 객체를 탐색할 수도 있습니다.

   ![](assets/menu-350x440.png)

1. 문서를 업로드할 작업 항목으로 이동합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 문서]** 아이콘 ![](assets/documents.png) 을 클릭합니다.

1. 클릭 **[!UICONTROL 새 파일]** 플러그인의 하단 근처에 있습니다.
1. 업로드할 대지를 선택합니다.

   >[!TIP]
   >
   >두 개 이상의 대지를 선택하려면 원하는 대지를 클릭하여 드래그합니다.
1. (선택 사항) **[!UICONTROL 업데이트]** 영역.
1. 을(를) 선택합니다 **[!UICONTROL 자산 유형]** 드롭다운 메뉴에서:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL 내보내기 형식]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>대지는 작업 항목의 [!UICONTROL 문서] 탭에 PNG로 업로드됩니다 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>대지는 작업 항목의 [!UICONTROL 문서] 탭에 JPG으로 업로드됩니다 [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>대지는 작업 항목의 [!UICONTROL 문서] 탭에 SVG으로 업로드됩니다 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>선택한 대지를 업로드하려면 선택합니다 <strong>단일 PDF 파일</strong> 또는 <strong>여러 PDF 파일</strong>. 대지는 작업 항목의 [!UICONTROL 문서] 탭에 PDF으로 업로드됩니다 [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. 클릭 **[!UICONTROL 업로드]**.\
   문서가 [!UICONTROL 문서] 영역(플러그인 및 데스크탑 앱)을 포함합니다.

## 새 버전 추가

1. 을(를) 클릭합니다. **[!UICONTROL 메뉴]** 오른쪽 상단 모서리의 아이콘을 클릭한 다음 **[!UICONTROL 작업 목록]**. 메뉴를 사용하여 상위 객체를 탐색할 수도 있습니다.

   ![](assets/menu-350x440.png)

1. 문서를 업로드할 작업 항목으로 이동합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 문서]** 아이콘 ![](assets/documents.png)을 클릭합니다.

1. 새 버전을 추가할 문서를 클릭합니다.
1. 클릭 **[!UICONTROL 새 버전]** 플러그인의 하단 근처에 있습니다.
1. 업로드할 대지를 선택합니다.

   >[!NOTE]
   >
   >새 버전의 SVG, PNG 또는 JPG을 업로드하려면 하나의 대지 만 업로드할 수 있습니다.

1. (선택 사항) **[!UICONTROL 업데이트]** 영역.

1. 을(를) 선택합니다 **[!UICONTROL 자산 유형]** 드롭다운 메뉴에서:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">내보내기 형식</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>대지는 작업 항목의 [!UICONTROL 문서] 탭에 PNG로 업로드됩니다 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>대지는 작업 항목의 [!UICONTROL 문서] 탭에 JPG으로 업로드됩니다 [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>대지는 작업 항목의 [!UICONTROL 문서] 탭에 SVG으로 업로드됩니다 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>대지는 작업 항목의 [!UICONTROL 문서] 탭에 PDF으로 업로드됩니다 [!DNL Workfront].</p>
      <p><strong>참고</strong>: 새 문서 버전에 대해 하나의 대지만 업로드할 수 있습니다.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. 클릭 **[!UICONTROL 업로드]**.\
   문서가 [!UICONTROL 문서] 영역(플러그인 및 데스크탑 앱)을 포함합니다.
