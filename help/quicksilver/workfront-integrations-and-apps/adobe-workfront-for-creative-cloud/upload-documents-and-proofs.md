---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: ' [!DNL Adobe Workfront plugin] 에서  [!DNL Creative Cloud](으)로 문서 및 증명 업로드'
description: ' [!DNL Adobe Workfront plugin] 에서  [!DNL Creative Cloud](으)로 문서 및 증명 업로드'
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# [!DNL Adobe Workfront plugin]에서 [!DNL Creative Cloud](으)로 문서 및 증명 업로드

프로젝트를 빠른 검토 및 승인을 위한 문서로 업로드하거나 간단히 [!DNL Adobe Workfront]에 저장할 수 있습니다.

>[!NOTE]
>
>Premiere Pro 및 After Effects에서는 문서 및 증명 업로드가 현재 지원되지 않습니다.


## 문서 제한

이 섹션에서는 [!DNL Workfront for Adobe Creative Cloud plugins]의 알려진 문서 제한 사항에 대해 간략히 설명합니다.

### 새 문서 버전에서는 업로드할 파일이 하나만 허용됩니다.

[!DNL Workfront] 문서에는 여러 파일이 포함될 수 없으므로 새 문서 버전을 Workfront에 업로드하려면 특정 설정을 사용하지 않도록 설정해야 합니다.

>[!NOTE]
>
>여러 파일을 생성해야 하는 경우 대신 증명을 만들 수 있습니다. 새 증명은 원본 문서와 연결되지 않습니다.



스위치를 [!DNL InDesign]의 단일 파일로 다시 변경하려면:

1. **내보내기 파일 설정 설정** 대화 상자를 엽니다.

   ![파일 내보내기 설정](assets/file-export-settings.png)

1. 내보낼 자산 유형을 찾고 아래에 설명된 대로 설정을 조정합니다.

   <table>
    <tr>
    <td><strong>PDF 및 PDF 인쇄</strong>
    </td>
    <td><strong>별도의 PDF 파일 만들기</strong>를 선택 취소합니다.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td><strong>범위</strong>를 선택하고 단일 페이지 번호를 입력하세요. 
    <p>
    <strong>참고</strong>: 전체 문서를 업로드하려면 증명을 만들어야 합니다. 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB 및 EPUB 고정</strong>
    </td>
    <td>조정이 필요하지 않습니다.
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>조정이 필요하지 않습니다.
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td><strong>범위</strong>를 선택하고 단일 페이지 번호를 입력하세요. 
    <p>
    <strong>참고</strong>: 전체 문서를 업로드하려면 증명을 만들어야 합니다. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td><strong>범위</strong>를 선택하고 단일 페이지 번호를 입력하세요. 
    <p>
    <strong>참고</strong>: 전체 문서를 업로드하려면 증명을 만들어야 합니다. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>조정이 필요하지 않습니다. 
    </td>
    </tr>
    </table>
