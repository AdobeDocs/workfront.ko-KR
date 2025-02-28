---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets 또는 Assets Essentials로 문서 보내기
description: Workfront에서 Experience Manager Assets 또는 Assets Essentials로 문서를 전송할 수 있습니다. Workfront에서 Assets Essentials로 업로드되고 전송된 문서는 여전히 전체 문서 스토리지에 대해 계산됩니다. Assets Essentials에서 연결된 Assets은 전체 스토리지에 포함되지 않습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 0%

---

# Experience Manager Assets 또는 Assets Essentials로 문서 보내기

Workfront에서 Experience Manager Assets 또는 Assets Essentials로 문서를 전송할 수 있습니다. Workfront에서 Assets Essentials로 업로드되고 전송된 문서는 여전히 전체 문서 스토리지에 대해 계산됩니다. Assets Essentials에서 연결된 Assets은 전체 스토리지에 포함되지 않습니다.

이 통합을 통해 Experience Manager으로 전송된 Assets의 크기 제한은 **5GB**&#x200B;입니다.

미리보기 환경에서 이 통합을 통해 Experience Manager으로 전송된 Assets의 크기 제한은 **30GB**&#x200B;입니다.

메타데이터 필드는 에셋을 Workfront에서 Experience Manager Assets 또는 Assets Essentials로 전송할 때 먼저 매핑됩니다. 상위 개체에 대해 매핑하도록 구성된 메타데이터도 전송됩니다. 메타데이터 매핑 구성에 대한 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.

>[!INFO]
>
>**예** 작업에 첨부된 에셋을 처음 보낼 때 작업 메타데이터는 프로젝트, 포트폴리오 및 프로그램과 같은 상위 개체의 매핑된 메타데이터뿐만 아니라 Experience Manager Assets 또는 Assets Essentials에도 매핑됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 완료하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront 플랜</a>*</td> 
   <td> <p> 임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">기존 라이선스 개요</a>*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials가 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서에 대한 액세스 권한 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 전제 조건

시작하기 전에,

* Workfront 관리자는 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.


## Workfront에서 문서 보내기

사용자가 Workfront에서 Experience Manager Assets 또는 Assets Essentials로 문서를 전송하면 매핑된 메타데이터가 문서를 따라 전송됩니다. 문서가 전송된 후 Workfront에서 문서 메타데이터에 수행된 변경 사항은 Assets 또는 Assets Essentials에 반영되지 않습니다. Workfront의 매핑된 필드가 변경된 경우 업데이트된 메타데이터가 포함된 새 버전의 문서를 Assets 또는 Assets Essentials로 보내야 합니다. 메타데이터를 설정하거나 편집하려면 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.

문서를 전송하려면:

1. Workfront의 **문서** 영역으로 이동하여 보낼 문서를 선택하십시오.
1. **보내기**&#x200B;를 클릭한 다음 관리자가 설정한 Experience Manager 통합을 선택합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Assets 또는 Assets Essentials에 대해 구체적으로 언급하지 않을 수 있습니다.

   ![전송 대상](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 에셋을 이동할 위치를 선택한 다음 **폴더 선택**&#x200B;을 클릭합니다.
1. 원하는 대상을 찾으면 **저장**&#x200B;을 클릭하세요.

## 새 버전 보내기

이전에 Workfront에 업로드한 문서에 새 버전을 추가할 수 있습니다. 자세한 내용은 [새 문서 버전 업로드](../../documents/managing-documents/upload-new-document-version.md)를 참조하십시오. 최신 버전이 업로드되면 Assets Essentials로 전송할 수 있습니다. Workfront의 매핑된 필드가 변경된 경우 새 버전은 전송 시 Assets Essentials의 메타데이터를 업데이트합니다.

>[!IMPORTANT]
>
>새 버전을 Workfront에 업로드하기 전에 파일 이름을 바꾸는 것이 좋습니다. 이전 버전과 정확히 동일한 파일 이름의 새 버전을 업로드하는 경우 Workfront에서 가장 최근 버전만 다운로드할 수 있습니다. 파일 이름과 관계없이 Experience Manager Assets 또는 Assets Essentials에서 모든 버전을 다운로드할 수 있습니다.

최신 버전을 보내려면

1. Workfront의 **문서** 영역으로 이동하여 문서를 찾습니다.
1. **전송 대상**&#x200B;을 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택하십시오.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Assets 또는 Assets Essentials에 대해 특별히 언급하지 않을 수 있습니다.

   ![전송 대상](assets/copy-of-send-to-in-toolbar-350x149.png)

1. **저장**&#x200B;을 클릭합니다. 새 버전이 이전 버전과 동일한 위치에 저장됩니다.

## Experience Manager Assets에서 연결된 폴더로 문서 이동

>[!NOTE]
>
>이 기능은 Experience Manager Assets as a Cloud Service에서만 사용할 수 있습니다. Experience Manager Assets Essentials에서는 사용할 수 없습니다.

문서와 연결된 폴더가 모두 동일한 문서 목록(예: 프로젝트의 문서 영역)에 있는 경우 문서를 Experience Manager Assets의 연결된 폴더로 이동할 수 있습니다.

1. 이동할 문서를 찾습니다.
1. 이동할 연결된 Experience Manager Assets 폴더로 문서를 끌어다 놓습니다.

문서를 이동하는 동안에는 문서 옵션을 사용할 수 없습니다. 문서가 Experience Manager Assets으로 이동되면 은 더 이상 Workfront의 문서 목록에 표시되지 않습니다.

>[!NOTE]
>
> 문서를 이동하는 동안 문서에 대해 수행한 작업이나 편집 내용은 Experience Manager Assets의 문서에 표시되지 않으므로 손실됩니다.

