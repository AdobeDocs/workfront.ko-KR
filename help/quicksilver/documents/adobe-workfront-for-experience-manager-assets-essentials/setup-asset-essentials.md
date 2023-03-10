---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets Essentials 통합 구성
description: Experience Manager Assets Essentials - EDIT ME에서 작업을 컨텐츠와 연결합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 059cfa79c57f071b3c7efd690b583099f46c99fb
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 6%

---

# Experience Manager Assets Essentials 통합 구성

Experience Manager Assets Essentials에서 작업을 콘텐츠와 &#x200B; 연결합니다.

* Adobe Workfront에서 Experience Manager Assets Essentials로 자산 및 메타데이터&#x200B; 푸시
* Experience Manager Assets Essentials의 자산을 Workfront의 프로젝트 및 작업에 &#x200B; 연결합니다
* Experience Manager Assets Essentials로 푸시된 자산에 대한 버전 관리 워크플로우를 용이하게 합니다


## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>Adobe Workfront 플랜*</strong>
   </td>
   <td>모든
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront 라이선스*</strong>
   </td>
   <td>플랜
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager 라이선스</strong>
   </td>
   <td>표준
   </td>
  </tr>
  <tr>
   <td><strong>제품</strong>
   </td>
   <td>Experience Manager Assets Essentials가 있어야 하며 Admin Console에서 사용자로 제품에 추가해야 합니다.
   </td>
  </tr>
  <tr>
   <td><strong>액세스 수준 구성</strong>
   </td>
   <td>Workfront 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 <strong>사용자에게 전체 관리자 액세스 권한 부여</strong>.
   </td>
  </tr>
</table>


*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.


## 통합 설정

1. 을(를) 클릭합니다. **기본 메뉴** Adobe Workfront의 오른쪽 위 모서리에 있는 아이콘을 클릭한 다음 **설정**.
1. 선택  **문서** ![문서 아이콘](assets/document-icon.png) 왼쪽 패널에서 를 선택하고 **Experience Manager 통합**.
1. 선택 **Experience Manager 통합 추가**.
1. 다음을 지정합니다.

   <table>
   <tr>
      <td><strong>이름</strong>
      </td>
      <td>[문서] 영역의 [새로 추가] 단추에서 사용자가 볼 이름을 입력합니다.
      </td>
   </tr>
   <tr>
      <td><strong>탐색 URL</strong>
      </td>
      <td>시스템이 탐색 URL을 자동으로 채웁니다. 이 URL은 빠른 액세스를 위해 기본 메뉴에서 조직의 Assets Essentials 인스턴스에 연결하는 데 사용됩니다.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets 저장소</strong>
      </td>
      <td>
      시스템은 조직 ID와 연결된 Experience Manager 저장소를 자동으로 채웁니다.
      </td>
   </tr>
   </table>

1. 클릭 **저장** 또는 다음 위치로 이동 [메타데이터 설정(선택 사항)](#set-up-metadata-optional) 섹션에 자세히 설명되어 있습니다.


## 메타데이터 설정(선택 사항)

Workfront 오브젝트 데이터를 Experience Manager Assets의 에셋 미디어 필드에 매핑합니다. 메타데이터는 에셋이 Workfront에서 처음으로 전달될 때 매핑됩니다.


### 전제 조건

시작하기 전에

* 에 설명된 대로 Experience Manager Assets Essentials에서 메타데이터 스키마를 구성합니다. [Adobe Workfront과 Experience Manager Assets 간 자산 메타데이터 매핑 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (선택 사항) Workfront에서 사용자 지정 양식 필드를 구성합니다. Workfront에는 사용할 수 있는 다양한 기본 제공 사용자 지정 필드가 있습니다. 그러나 고유한 사용자 지정 필드를 만들 수도 있습니다. 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### 자산

자산이 Workfront에서 처음 푸시되면 메타데이터가 매핑됩니다. Experience Manager Assets Essentials로 자산을 처음 보낼 때 기본 제공 또는 사용자 지정 필드가 있는 문서가 지정된 필드에 자동으로 매핑됩니다.

1. 에서 **Workfront 필드** 열에서 내장 또는 사용자 지정 Workfront 필드를 선택합니다.
   >[!NOTE]
   >
   >단일 Workfront 필드를 여러 Experience Manager Assets 필드에 매핑할 수 있습니다. 여러 Workfront 필드를 단일 Experience Manager Assets 필드에 매핑할 수 없습니다.
1. 에서 **Experience Manager** 필드에서 Experience Manager Assets 필드를 선택합니다.
1. 필요에 따라 1단계와 2단계를 반복합니다.
   ![메타데이터 활성화](assets/metadata-assets-essentials.png)
1. 클릭 **저장** 또는 다음 위치로 이동 [연결된 폴더 설정(선택 사항)](#set-up-linked-folders-optional) 섹션에 자세히 설명되어 있습니다.


## 연결된 폴더 설정(선택 사항)

{{setup-linked-folder}}
