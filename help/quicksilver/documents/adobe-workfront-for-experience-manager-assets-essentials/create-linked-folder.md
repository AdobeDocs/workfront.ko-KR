---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Experience Manager Assets 또는 Assets Essentials와 연결된 폴더 만들기
description: You can create a folder linked with Experience Manager Assets or Assets Essentials while in Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 3%

---

# Experience Manager Assets 또는 Assets Essentials와 연결된 폴더 만들기

You can create a folder linked with Experience Manager Assets or Assets Essentials while in Workfront. Because the folder is linked, any asset added to the folder will automatically show up in both Workfront and Experience Manger. You don&#39;t have to manually send the asset if it&#39;s in a linked folder.

If an asset is deleted or moved from a linked folder inside of Experience Manager Assets or Assets Essentials, Workfront retains a copy of the asset in the Project > Documents area.

>[!NOTE]
>
>이 기능은 새 문서 영역에서 사용할 수 없습니다.<br>
>조직에서 엔터프라이즈 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. From there, you can add assets from Experience Manager Assets or Assets Essentials, but you won&#39;t be able to create a linked folder.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table>
  <tr>
   <td><strong>Adobe Workfront package</strong>
   </td>
   <td>Any
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront licenses</strong>
   </td>
   <td>
   <p>표준</p>
   <p>플랜</p>
   </td>
  </tr>
  <tr>
   <td><strong>Additional products</strong>
   </td>
   <td>You must have Experience Manager Assets as a Cloud Service or Assets Essentials, and you must be added to the product as a user.
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager permissions</strong>
   </td>
   <td>You must have write access to the destination folder in the Experience Manger integration.
   </td>
  </tr>
  <tr>
   <td><strong>Access level configurations</strong>
   </td>
   <td>You must be a Workfront administrator to configure an Experience Manager integration. After it is configured, users with a Plan license can set up linked folders on individual projects.
   </td>
  </tr>
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

Before you begin,

* Workfront 관리자는 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.


## Create a linked folder

The linked folder is created in the location specified by the Workfront administrator when they set up the integration. 각 통합에는 연결된 폴더에 대해 하나의 폴더 위치만 있을 수 있습니다.

연결된 폴더의 이름은 Portfolio, 프로그램, 연결된 프로젝트를 기반으로 자동으로 생성되며 변경할 수 없습니다. 프로젝트가 Portfolio 또는 프로그램과 연결되어 있지 않으면 연결된 폴더에 프로젝트 이름과 생성 날짜가 표시됩니다.

>[!NOTE]
>
>연결된 폴더 내에 새 문서 또는 증명 버전을 만들 수 없습니다.


연결된 폴더를 만들려면 다음 작업을 수행하십시오.

1. 폴더를 원하는 프로젝트로 이동합니다.
1. **새로 추가**&#x200B;를 선택한 다음 관리자가 설정한 Experience Manager 통합으로 이동합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Experience Manager Assets 또는 Assets Essentials에 대해 특별히 언급하지 않을 수 있습니다.

1. **연결된 폴더 만들기**를 선택합니다. 시스템은 통합 설정 시 지정된 위치를 기반으로 Experience Manager에 폴더를 자동으로 생성합니다.
   ![연결된 폴더 만들기](assets/linked-folder.png)
