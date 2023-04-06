---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets 또는 Assets Essentials으로 문서 보내기
description: Workfront에서 Experience Manager Assets 또는 Assets Essentials으로 문서를 보낼 수 있습니다. Workfront에서 Assets Essentials으로 업로드되고 전송된 문서는 전체 문서 저장소에 대해 계속 계산됩니다. Assets Essentials에서 연결된 자산은 전체 스토리지에 포함되지 않습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Experience Manager Assets 또는 Assets Essentials으로 문서 보내기


Workfront에서 Experience Manager Assets 또는 Assets Essentials으로 문서를 보낼 수 있습니다. Workfront에서 Assets Essentials으로 업로드되고 전송된 문서는 전체 문서 저장소에 대해 계속 계산됩니다. Assets Essentials에서 연결된 자산은 전체 스토리지에 포함되지 않습니다.

메타데이터 필드는 자산을 Workfront에서 Experience Manager Assets 또는 Assets Essentials으로 보낼 때 먼저 매핑됩니다. 상위 개체에 대해 매핑하도록 구성된 모든 메타데이터도 전송됩니다. 메타데이터 매핑 구성에 대한 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**예** 작업에 첨부된 자산을 처음 보낼 때 작업 메타데이터는 프로젝트, 포트폴리오 및 프로그램과 같은 상위 개체의 매핑된 메타데이터와 Experience Manager Assets 또는 Assets Essentials에 매핑됩니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront 플랜</a>*</td> 
   <td> <p> 모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">이전 라이센스 개요</a>*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials이 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서에서 액세스 수준 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에

* Workfront 관리자가 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Workfront에서 문서 보내기

사용자가 Workfront에서 Experience Manager Assets 또는 Assets Essentials으로 문서를 보내면 매핑된 메타데이터가 문서에 따라 전송됩니다. 문서가 전송되면 Workfront에서 문서의 메타데이터를 변경한 내용이 자산 또는 Assets Essentials에 반영되지 않습니다. Workfront의 매핑된 필드가 변경되면 업데이트된 메타데이터가 있는 문서의 새 버전을 자산 또는 Assets Essentials으로 보내야 합니다. 메타데이터를 설정하거나 편집하려면 다음을 참조하십시오 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

문서를 보내려면

1. 로 이동합니다. **문서** Workfront에서 영역을 선택하고 전송할 문서를 선택합니다.
1. 클릭 **보내기**&#x200B;그런 다음 관리자가 설정한 Experience Manager 통합을 선택합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합의 이름을 선택할 수 있으므로 자산 또는 Assets Essentials에 대해 특별히 언급하지 않을 수 있습니다.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 자산을 이동할 위치를 선택하고 을 클릭합니다 **폴더 선택**.
1. 원하는 대상을 찾으면 을 클릭합니다 **저장**.

## 새 버전 보내기

이전에 Workfront에 업로드한 문서에 새 버전을 추가할 수 있습니다. 자세한 내용은 [문서의 새 버전 업로드](../../documents/managing-documents/upload-new-document-version.md). 최신 버전이 업로드되면 Assets Essentials에게 보낼 수 있습니다. Workfront의 매핑된 필드가 변경되면 새 버전이 Assets Essentials을 전송할 때 메타데이터를 업데이트합니다.

>[!IMPORTANT]
>
>새 버전을 Workfront에 업로드하기 전에 파일 이름을 바꾸는 것이 좋습니다. 이전 버전과 정확히 동일한 파일 이름을 사용하는 새 버전을 업로드하는 경우, Workfront에서 최신 버전만 다운로드할 수 있습니다. 파일 이름과 관계없이 Experience Manager Assets 또는 Assets Essentials에서 모든 버전을 다운로드할 수 있습니다.

최신 버전을 보내려면

1. 로 이동합니다. **문서** Workfront에서 영역을 설정하고 문서를 찾습니다.
1. 선택 **보내기**&#x200B;그런 다음 관리자가 설정한 Experience Manager 통합을 선택합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합의 이름을 선택할 수 있으므로 자산이나 Assets Essentials에 대해 특별히 언급하지는 않을 수 있습니다.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. **저장**&#x200B;을 클릭합니다. 새 버전이 이전 버전과 동일한 위치에 저장됩니다.
