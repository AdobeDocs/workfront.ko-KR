---
product-area: documents;workfront-integrations;system-administration
navigation-topic: adobe-cloud-drive
title: Adobe 클라우드 드라이브 설정 및 관리
description: 관리자는 조직에 대한 Adobe Cloud Drive를 설정하고, 사용자 장치에 배포하며, Adobe Admin Console에서 진행 중인 액세스를 관리할 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps, System Setup and Administration
role: Admin
source-git-commit: 56dca343c919db3bb09a232ada2b4700c59f5147
workflow-type: tm+mt
source-wordcount: '3139'
ht-degree: 1%

---

# 조직을 위한 Adobe 클라우드 드라이브 설정 및 관리

관리자는 Adobe Cloud Drive를 설정하여 사용자가 macOS의 Finder와 Windows의 File Explorer를 통해 Adobe 클라우드 스토리지의 프로젝트 파일에 직접 데스크톱으로 액세스할 수 있도록 할 수 있습니다. 이 문서에서는 Adobe Admin Console에서 액세스를 활성화하고, 애플리케이션을 사용자 장치에 배포하고, 지속적으로 액세스를 관리하는 방법을 다룹니다.

Adobe Cloud Drive는 사용자의 Mac 및 Windows 컴퓨터에서 Workfront 클라우드 저장소의 Adobe 문서를 가상 드라이브로 마운트하는 엔터프라이즈 데스크톱 애플리케이션입니다. 설치 후 사용자는 Finder 또는 File Explorer에서 Workfront 프로젝트 폴더를 볼 수 있으며, 파일을 수동으로 다운로드하거나 브라우저를 통해 작업하지 않고도 데스크탑 애플리케이션을 사용하여 프로젝트 파일을 열고, 편집하고, 저장할 수 있습니다.

Adobe Cloud Drive를 사용하려면 귀사가 Workflow Ultimate 패키지에 있어야 하며 Adobe 클라우드 스토리지가 활성화되어 있어야 합니다.

Adobe Cloud Drive에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Cloud Drive 개요](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)
* [Adobe Cloud Drive 설치](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)
* [Adobe 클라우드 드라이브 사용](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 버전</td> 
   <td>Adobe 클라우드 스토리지가 활성화된 워크플로우 Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe 관리자 권한</td> 
   <td>Adobe Admin Console에서 Workfront 시스템 관리자여야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Adobe Admin Console에서 Adobe 클라우드 드라이브에 액세스 할당

Adobe 클라우드 스토리지가 활성화되면 Adobe 클라우드 드라이브가 워크플로우 Ultimate 패키지에 포함됩니다. 이 제품은 Admin Console의 **제품** 섹션에 독립 실행형 제품으로 표시되지 않습니다. 대신 **사용자** 아래의 **역할** 섹션을 통해 관리됩니다.

**사용자** > **역할**(으)로 이동하면 Workfront 제품과 관련된 두 개의 역할이 표시됩니다.

| 역할 | 자동 할당 대상: | Adobe 클라우드 드라이브와의 관련성 |
| --- | --- | --- |
| **구성원** | 조직의 모든 사용자 | 조직 수준의 Adobe Cloud Drive 기능 스위치를 포함합니다. 기본적으로에 있습니다. |
| **ACD 사용자** | 기본적으로 아무도 없습니다. | 조직 수준 스위치가 꺼져 있을 때 개별 액세스 권한을 부여합니다. |

Admin Console의 ![역할](assets/admin-console-roles.png)

### 액세스 제어

**컨트롤 1: 조직 수준 기능 제어(구성원 역할의)**

**구성원** 역할은 조직의 모든 사용자에게 자동으로 할당됩니다. 이 역할에는 **Adobe Cloud Drive** 기능 스위치가 있습니다. 이 스위치가 켜지면 Workflow Ultimate 라이선스가 있는 모든 사용자가 Adobe Cloud Drive에 액세스할 수 있습니다. 해제되면 라이선스와 관계없이 Adobe Cloud Drive에 액세스할 수 있는 사용자가 없습니다.

Adobe이 조직의 Adobe Cloud Drive를 활성화하면 기본적으로 스위치가 켜집니다.

**컨트롤 2: ACD 사용자 역할**

**ACD 사용자** 역할은 조직 수준 스위치가 꺼진 경우에만 관련이 있습니다. 제어된 지표를 실행하기 위해 조직 수준 스위치를 끄더라도 **ACD 사용자** 역할에 추가하여 특정 사용자에게 액세스 권한을 부여할 수 있습니다. 이 역할의 사용자는 조직 수준 스위치가 꺼져 있는 경우에도 Adobe Cloud Drive에 액세스할 수 있습니다. 조직 수준 스위치가 켜져 있으면 **ACD 사용자** 역할은 영향을 주지 않습니다.

**기본 요구 사항: 워크플로 Ultimate 라이선스**

Adobe Cloud Drive는 Workflow Ultimate 패키지에서만 사용할 수 있습니다. 다른 패키지에서는 역할 옵션을 사용할 수 없습니다.

Workflow Ultimate 패키지 내의 라이선스는 Standard, Light 또는 Contributor와 같은 모든 라이선스 유형일 수 있습니다. 라이선스에 대한 자세한 내용은 [라이선스 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)를 참조하세요.

다음 표에서는 이러한 컨트롤이 상호 작용하는 방식을 보여 줍니다.

| 조직 수준 스위치 | ACD 사용자 역할의 사용자 | Workflow Ultimate 라이선스 | 액세스 결과 |
| --- | --- | --- | --- |
| 켜기 | 불필요 | 예 | 부여됨 |
<!-- | On | Not required | No | Denied | -->
| 끔 | 예 | 예 | 부여됨 |
| 끔 | 아니요 | 예 | 거부됨 |
| 다음 중 하나 | 다음 중 하나 | 아니요 | 거부됨 |

## 전제 조건

시작하기 전에 다음을 확인하십시오.

* 프로비저닝할 사용자에게는 Workfront Workflow 라이선스가 할당되어 있습니다.
* IT 팀과 [네트워크 요구 사항](#network-requirements)을 검토했습니다.
* Adobe Cloud Drive에 표시되는 내용(Workfront 프로젝트 자산만 해당) 및 설치 방법을 설명하는 메시지를 사용자에게 보내도록 초안을 작성했습니다.

  >[!NOTE]
  >
  >액세스가 활성화되었지만 어떠한 Workfront 프로젝트에도 액세스할 수 없는 사용자에게는 로그인 후 빈 탑재 드라이브가 표시됩니다. 이는 예상되었습니다. Workfront 프로젝트 액세스는 Workfront에서 별도로 관리됩니다. 자세한 내용은 [프로젝트 공유](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-project.md)를 참조하십시오.
  >
  >또한 Creative Cloud 권한이 드라이브에 프로젝트를 표시하려면 Workfront과 동일한 IMS 조직에 있어야 합니다.

## Adobe Admin Console에서 액세스 구성

Adobe Cloud Drive 액세스 권한은 Adobe Admin Console에 구성됩니다. 롤아웃 전략과 일치하는 옵션을 선택합니다.

### 옵션 A: 전체 조직에 대한 액세스 활성화

Adobe이 조직에 대해 Adobe Cloud Drive를 활성화하면 조직 수준 기능 스위치가 기본적으로 켜지고 모든 사용자가 즉시 액세스할 수 있습니다. 이 절차를 사용하여 응용 프로그램을 배포하기 전에 스위치가 켜져 있는지 확인합니다.

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)에 로그인합니다.
1. 위쪽 탐색 모음에서 **사용자**&#x200B;를 클릭합니다.
1. 왼쪽 패널에서 **역할**&#x200B;을 클릭합니다.
1. 역할 목록에서 **구성원**&#x200B;을 클릭합니다.
1. 오른쪽에 열리는 **구성원** 패널에서 **Adobe Cloud Drive**&#x200B;이(가) **권한**&#x200B;에 표시되고 스위치가 켜져 있는지 확인합니다.

   ![Adobe 클라우드 드라이브가 켜진 구성원 역할 세부 정보 패널](assets/member-permissions.png)

   >[!NOTE]
   >
   >Adobe Cloud Drive가 **구성원** 역할의 **권한** 아래에 표시되지 않으면 조직에 대해 Adobe Cloud Drive가 아직 활성화되지 않았을 수 있습니다. 확인하려면 Adobe 지원 센터에 문의하십시오.

1. 변경 사항이 있으면 **저장**&#x200B;을 클릭합니다.

### 옵션 B: 특정 사용자 그룹에 대한 액세스 활성화

예를 들어 광범위한 롤아웃 전의 파일럿 중에 정의된 사용자 집합에 대한 액세스를 제한하려면 이 옵션을 사용합니다. 여기에는 조직 수준 스위치를 끈 다음 파일럿 사용자를 **ACD 사용자** 역할에 추가하는 작업이 포함됩니다.

>[!IMPORTANT]
>
>조직 수준 스위치를 끄면 현재 로그인한 사용자를 포함하여 조직의 모든 사용자에 대한 Adobe Cloud Drive 액세스 권한이 즉시 제거됩니다. 조직 수준 기능을 끄고 동일한 세션에 파일럿 사용자를 추가해야 합니다.

조직 수준 기능을 끄려면:

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)에 로그인합니다.
1. 위쪽 탐색 모음에서 **사용자**&#x200B;를 클릭한 다음 왼쪽 패널에서 **역할**&#x200B;을 클릭합니다.
1. 역할 목록에서 **구성원**&#x200B;을 클릭합니다.
1. **구성원** 패널에서 **권한**&#x200B;에서 **Adobe Cloud Drive**&#x200B;을(를) 찾은 다음 끕니다.
1. **저장**&#x200B;을 클릭합니다.

ACD 사용자 역할에 파일럿 사용자를 추가하려면

1. 왼쪽 패널에서 **역할**&#x200B;을 클릭하여 역할 목록으로 돌아갑니다.
1. 역할 목록에서 **ACD 사용자**&#x200B;를 클릭합니다.

   ![ACD 사용자 세부 정보 패널](assets/acd-user-panel.png)

1. **사용자 추가**&#x200B;를 클릭합니다.
1. 각 파일럿 사용자의 이메일 주소를 입력합니다.
1. **저장**&#x200B;을 클릭합니다.

   **ACD 사용자** 역할에 추가된 사용자는 즉시 액세스할 수 있습니다. 이 역할에 속하지 않는 사용자는 역할에 추가하거나 조직 수준 스위치를 다시 켤 때까지 액세스 권한이 없습니다.

   >[!TIP]
   >
   >시간이 지남에 따라 액세스를 확장하려면 **ACD 사용자** 역할로 돌아가서 필요에 따라 사용자를 추가하십시오. 전체 롤아웃이 준비되면 **구성원** 역할에서 조직 수준 스위치를 다시 켜십시오. 조직 수준 스위치가 켜지면 **ACD 사용자** 역할은 영향을 주지 않으며 유지 관리할 필요가 없습니다.

## Adobe Cloud Drive 애플리케이션 배포

Adobe Admin Console에서 액세스를 구성하면 권한이 설정됩니다. 애플리케이션을 배포하면 사용자의 장치에 설치됩니다. 이 단계는 별도로 요구되는 두 단계입니다.

Adobe Cloud Drive는 독립 실행형 애플리케이션입니다. 이 변수는 Creative Cloud 데스크탑 애플리케이션을 통해 배포되지 않으며 Creative Cloud 패키지 관리자에 표시되지 않습니다. 그러나 Adobe Cloud Drive의 사용자 프로필은 Creative Cloud 앱 권한에 연결되어 있습니다. 즉, 사용자가 드라이브의 Workfront 프로젝트에 액세스할 수 있으려면 Creative Cloud 앱은 Workfront과 동일한 IMS 조직에서 권한을 부여받아야 합니다.

조직의 장치 관리 방식과 일치하는 배포 방법을 선택합니다.

### 방법 A: Admin Console 패키지를 통한 IT 관리 배포

조직에서 Microsoft Intune, SCCM, Jamf Pro 또는 Apple 원격 데스크톱과 같은 중앙 집중식 배포 도구를 사용하는 경우 이 방법을 사용하십시오. 표준 Adobe 엔터프라이즈 배포 워크플로우이며, 다른 Adobe 애플리케이션에 사용되는 것과 동일한 패키지 생성 프로세스를 따릅니다.

Adobe Admin Console에서 패키지를 만들려면 다음을 수행하십시오.

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)에 로그인합니다.
1. 위쪽 탐색 모음에서 **패키지**&#x200B;를 클릭합니다.
1. 왼쪽 패널에서 **미리 생성된 패키지**&#x200B;를 클릭합니다.
1. **템플릿** 탭을 클릭합니다.

   Adobe Cloud Drive는 템플릿 목록에 두 번 나타납니다(macOS의 경우 한 번, Windows의 경우 한 번).

   ![미리 생성된 패키지 템플릿](assets/pre-generated-packages.png)

1. 대상 플랫폼과 일치하는 **Adobe Cloud Drive** 행을 찾은 다음 해당 행의 세부 정보 아이콘을 클릭합니다.

   사이드 패널에는 패키지 메타데이터가 표시됩니다.

   ![패키지 세부 정보 및 메타데이터](assets/template-details-and-metadata.png)

1. **사용자 지정**&#x200B;을 클릭합니다.

   패키지 사용자 지정 마법사가 열리며 **구성**, **앱 선택**, **옵션**, **완료**&#x200B;의 네 가지 단계로 구성됩니다.

1. **구성** 단계에서 대상 컴퓨터의 아키텍처를 선택한 다음 언어 설정을 확인하고 **다음**&#x200B;을 클릭합니다.

   * **macOS:** **macOS(Intel)** 또는 **macOS(Apple Silicon)**&#x200B;을(를) 선택합니다.
   * **Windows:** **Windows(64비트)** 또는 **Windows(ARM)**&#x200B;를 선택하십시오.

   ![패키지 마법사에서 단계 구성](assets/configure-step-in-wizard.png)

1. **앱 선택** 단계에서 원하는 버전으로 Adobe Cloud Drive가 선택되었는지 확인합니다.

   Adobe Cloud Drive는 사용 가능한 최신 버전과 함께 미리 선택됩니다. 이전 버전을 사용하려면 **다른 버전**&#x200B;을 클릭하고 **이전 버전**&#x200B;을 선택하십시오.

   ![패키지 마법사에서 앱 단계 선택](assets/choose-apps-step-in-wizard.png)

1. **다음**&#x200B;을 클릭합니다.
1. **옵션** 단계에서 옵션을 선택하지 않고 **다음**&#x200B;을 클릭합니다.

   이러한 설정은 Creative Cloud 데스크탑 애플리케이션에 적용되며 Adobe Cloud Drive에는 적용되지 않습니다.

   ![패키지 마법사의 옵션 단계](assets/options-step-in-wizard.png)

1. **완료** 단계에서 패키지 이름을 입력하고 **기본 패키지**&#x200B;를 선택합니다.
1. 요약을 검토하고 **패키지 만들기**&#x200B;를 클릭하세요.

   ![패키지 마법사에서 단계 완료](assets/finalize-step-in-wizard.png)

   마법사가 종료됩니다. 새 패키지가 빌드되는 동안 패키지 목록 맨 위에 **준비** 상태로 나타납니다. 준비가 완료되면 상태가 **최신**(으)로 변경되고 다운로드 링크가 나타납니다.

   ![준비 중인 패키지](assets/package-is-preparing.png)

1. **다운로드**&#x200B;를 클릭하고 패키지 파일을 선택한 위치에 저장합니다.

### 방법 B: 소프트웨어 배포에서 셀프서비스 직접 다운로드

소규모 조직, 자체 관리 장치의 경우 또는 개별 사용자에게 애플리케이션을 직접 설치하도록 지시할 때 이 방법을 사용하십시오.

시작하기 전에 다음을 확인하십시오.

* Adobe Admin Console의 사용자에 대해 액세스가 활성화됩니다.
* 소프트웨어 배포 URL 및 로그인 지침이 사용자에게 통지되었습니다.
* 필요한 끝점에 대한 네트워크 연결이 확인되었습니다. 자세한 내용은 이 문서에서 [네트워크 요구 사항](#network-requirements)을 참조하십시오.

Adobe Cloud Drive를 자동으로 설치하려면:

1. Adobe Admin Console에서 사용자에 대해 액세스 권한이 활성화되었는지 확인합니다.
1. 사용자를 [experience.adobe.com/#/downloads](https://experience.adobe.com/#/downloads)&#x200B;(으)로 보냅니다.

   >[!NOTE]
   >
   >Adobe Cloud Drive 설치 관리자를 보려면 사용자가 Adobe Admin Console에서 Adobe Cloud Drive 액세스 권한을 활성화해야 합니다. 액세스 권한이 없는 사용자에게는 나열된 설치 관리자가 표시되지 않습니다.

1. 사용자가 Enterprise ID 또는 Federated ID으로 로그인합니다. Adobe Cloud Drive 설치 관리자가 소프트웨어 배포의 **Workfront** 탭에 나타납니다.
1. 사용자는 플랫폼에 대한 설치 관리자를 다운로드하고 [Adobe Cloud Drive 설치](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)의 설치 단계를 따릅니다.

   ![Workfront용 Adobe Cloud Drive 설치 관리자](assets/wf-downloads.png)

배포 후 테스트 장치에서 다음 확인을 완료합니다.

1. **응용 프로그램** 폴더(macOS) 또는 **시작** 메뉴(Windows)에서 Adobe Cloud Drive를 시작합니다.
1. Adobe Admin Console에서 Adobe Cloud Drive 액세스 권한이 활성화된 사용자 계정으로 로그인합니다.
1. Finder 또는 파일 탐색기에서 마운트된 드라이브에 Workfront 프로젝트 폴더가 표시되는지 확인합니다.

   >[!NOTE]
   >
   >성공적으로 로그인했지만 폴더가 표시되지 않는 사용자는 Workfront 프로젝트에 액세스할 수 없습니다. Workfront의 프로젝트에 사용자를 추가하여 드라이브를 채웁니다.

1. 프로젝트 폴더로 이동하여 작은 테스트 파일을 만듭니다.
1. 브라우저에서 Workfront을 열고 테스트 파일이 해당 프로젝트에 표시되는지 확인합니다.
1. 확인 후 테스트 파일을 삭제합니다.

## Adobe Cloud Drive에 대한 진행 중인 사용자 액세스 관리

조직에서 Adobe Cloud Drive를 사용하고 나면 다음 단계에 따라 새 사용자를 추가하거나 더 이상 액세스할 필요가 없는 사용자를 제거합니다.

### 새 사용자 추가

조직 수준 스위치가 켜져 있으면 Adobe Admin Console 작업이 필요하지 않습니다. 사용자에게 Adobe Cloud Drive를 다운로드하여 설치하도록 요청합니다. 사용 허가된 사용자가 여전히 Adobe Cloud Drive에 액세스할 수 없는 경우 Adobe 지원 센터에 문의하여 계정이 올바르게 마이그레이션되었는지 확인하십시오.

조직 수준 스위치가 꺼져 있는 경우:

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)에 로그인합니다.
1. 위쪽 탐색 모음에서 **사용자**&#x200B;를 클릭한 다음 왼쪽 패널에서 **역할**&#x200B;을 클릭합니다.
1. 역할 목록에서 **ACD 사용자**&#x200B;를 클릭합니다.
1. **사용자 추가**&#x200B;를 클릭하고 사용자의 전자 메일 주소를 입력한 다음 **저장**&#x200B;을 클릭합니다.

### 사용자 제거

조직 수준 스위치가 켜져 있으면 모든 라이선스 사용자가 Adobe Cloud Drive에 액세스할 수 있습니다. Workfront 라이선스를 제거하지 않고 특정 사용자에 대한 액세스 권한을 제거하려면 조직 수준 스위치를 끄고 차단하려는 사용자를 제외한 다른 모든 사용자를 **ACD 사용자** 역할에 추가하십시오.

조직 수준 스위치가 꺼져 있고 사용자가 **ACD 사용자** 역할에 있는 경우:

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)에 로그인합니다.
1. 위쪽 탐색 모음에서 **사용자**&#x200B;를 클릭한 다음 왼쪽 패널에서 **역할**&#x200B;을 클릭합니다.
1. 역할 목록에서 **ACD 사용자**&#x200B;를 클릭합니다.
1. 사용자를 선택하고 **제거**&#x200B;를 클릭합니다.

사용자는 마운트된 드라이브에 즉시 액세스할 수 없습니다. Workfront에 저장된 파일은 삭제되지 않습니다. 사용자의 로컬 캐시는 응용 프로그램을 제거할 때까지 장치에 남아 있습니다.

>[!IMPORTANT]
>
>**ACD 사용자** 역할에서 사용자를 제거해도 Workfront 또는 Workfront 프로젝트에서는 제거되지 않습니다. Workfront 프로젝트 액세스를 별도로 관리합니다.

## Workfront 프로젝트 액세스 관리

Adobe Cloud Drive는 사용자가 액세스할 수 있는 Workfront 프로젝트를 표시합니다. 프로젝트 액세스는 Adobe Admin Console이 아닌 Workfront에서 관리됩니다. Adobe Cloud Drive 액세스 권한이 있지만 Workfront 프로젝트에 속하지 않는 사용자에게 로그인 후 빈 탑재된 드라이브가 표시됩니다. 이는 예상된 동작입니다.

프로젝트 액세스 관리에 대한 자세한 내용은 [프로젝트 관리](/help/quicksilver/manage-work/projects/manage-projects/manage-projects-overview.md) 및 [프로젝트 공유](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-project.md)를 참조하십시오.

## 네트워크 요구 사항

Adobe Cloud Drive를 사용하려면 Adobe 끝점 집합에 대한 아웃바운드 HTTPS(포트 443) 액세스가 필요합니다. 인바운드 방화벽 규칙이 필요하지 않습니다. 끝점 목록은 [Adobe 네트워크 끝점](https://helpx.adobe.com/in/enterprise/kb/network-endpoints.html)을 참조하십시오.

Adobe Cloud Drive는 macOS 및 Windows 모두에서 시스템 수준 프록시 구성을 읽습니다. 인증된 프록시가 지원됩니다.

## 보안 고려 사항

### 인증

Adobe Cloud Drive는 Adobe IMS(Identity Management 시스템)를 통해 사용자를 인증합니다. 사용자가 Enterprise ID 또는 Federated ID으로 로그인합니다. 조직에서 Adobe Admin Console에 구성된 SSO를 사용하는 경우 사용자는 ID 공급자를 통해 인증하므로 별도의 Adobe 자격 증명이 필요하지 않습니다.

>[!NOTE]
>
>Adobe Cloud Drive는 엔터프라이즈 배포에서 개인 Adobe ID(개별적으로 만들어지거나 관리되지 않는 계정)를 지원하지 않습니다. 사용자는 조직의 디렉터리에서 Enterprise ID 또는 Federated ID으로 로그인해야 합니다.

### 전송 중 및 유휴 상태 데이터

* Adobe Cloud Drive와 Adobe 서비스 간의 모든 통신은 TLS 1.2 이상을 사용합니다.
* Adobe 클라우드 저장소에 저장된 파일은 사용하지 않을 때 암호화됩니다.
* 로컬로 캐시된 파일은 FileVault(macOS) 또는 BitLocker(Windows)가 장치에서 활성화된 경우 OS 수준 디스크 암호화를 사용합니다.

### 파일 액세스 제어

파일 액세스는 Workfront 프로젝트 권한을 따릅니다. 사용자는 Workfront 액세스 수준에서 허용하는 대로 권한이 있는 프로젝트만 보고 상호 작용합니다.

각 Workfront 프로젝트의 루트 폴더는 데스크탑 보기에서 읽기 전용입니다. 사용자는 Finder 또는 파일 탐색기에서 프로젝트 루트 폴더의 이름을 바꾸거나, 이동하거나, 삭제할 수 없습니다. Workfront 권한에 따라 프로젝트 폴더 내의 어떤 깊이에서든 폴더, 하위 폴더 및 파일을 만들 수 있습니다.

## 일반적인 문제 해결

최종 사용자 문제 해결 단계는 [Adobe Cloud 드라이브 문제 해결](/help/quicksilver/documents/adobe-cloud-drive/troubleshoot-adobe-cloud-drive.md)을 참조하십시오. 아래 나열된 문제는 관리자에게만 해당됩니다.

### 소프트웨어 배포에서 Adobe Cloud Drive 설치 관리자를 찾을 수 없음

**원인:** Adobe Admin Console의 사용자는 Adobe Cloud Drive 액세스 권한을 사용할 수 없습니다.

**해상도:**

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)에 로그인하고 **사용자**&#x200B;를 클릭합니다.
1. 사용자를 검색하고 해당 이름을 클릭합니다.
1. **역할** 탭을 클릭하고 Adobe Cloud Drive가 활성화되어 있는지 확인합니다.

**원인:** Creative Cloud 모든 앱은 Workfront의 다른 IMS 조직에서 프로비저닝되었습니다.

**해결 방법:** 현재 사용할 수 있는 해결 방법이 없습니다.

### 사용자가 응용 프로그램을 설치하고 로그인했지만 드라이브에 폴더가 없습니다.

**원인:** 사용자에게 Workfront 프로젝트에 대한 권한이 없습니다.

**해상도:**

1. Workfront에서 사용자에게 하나 이상의 프로젝트에 대한 권한이 있는지 확인합니다.
1. 그렇지 않은 경우 사용자와 프로젝트를 공유합니다.
1. 사용자에게 프로젝트 폴더가 나타날 때까지 최대 5분 동안 기다리도록 요청합니다.
1. 5분 후에도 폴더가 표시되지 않으면 사용자에게 Adobe Cloud Drive를 종료하고 다시 시작하도록 요청하십시오.

### 사용자가 Adobe Cloud Drive에 로그인할 수 없음

**원인:** 사용자의 Adobe Admin Console 계정이 비활성 상태이거나 ID가 올바르게 구성되지 않았습니다.

**해상도:**

1. Adobe Admin Console에서 **사용자**&#x200B;를 클릭하고 사용자를 검색합니다.
1. 사용자의 계정 상태가 **활성**&#x200B;인지 확인하십시오.
1. 사용자의 이메일 도메인이 Admin Console 디렉터리에서 요구하는 도메인인지 확인합니다.
1. 조직에서 SSO를 사용하는 경우 ID 공급자에서 사용자의 계정이 활성화되어 있는지 확인하십시오.
1. 사용자에게 로그인을 다시 시도하도록 요청하십시오.

### 사용자가 저장한 후 파일이 동기화되지 않음

**원인:** 파일이 명시적으로 저장되지 않았거나 네트워크 연결 문제가 있습니다.

**해상도:**

1. 응용 프로그램에서 **파일** > **저장**&#x200B;을 사용하여 파일을 저장했는지 사용자에게 확인합니다. 응용 프로그램을 닫거나 자동 저장에 의존해도 동기화가 트리거되지 않습니다.
1. 사용자가 인터넷에 액세스할 수 있고 `*.adobe.com` 및 `*.workfront.com`에 연결할 수 있는지 확인하십시오.
1. 사용자에게 메뉴 모음(macOS) 또는 시스템 트레이(Windows)의 Adobe Cloud Drive 아이콘을 확인하도록 요청하여 오류 표시기가 있는지 확인합니다.
1. 오류가 발생하면 사용자에게 Adobe Cloud Drive를 종료하고 다시 시작한 다음 파일을 다시 저장하라고 요청합니다.
1. 문제가 지속되면 애플리케이션 로그를 수집합니다.

   * **macOS:** `~/Library/Logs/Adobe/AdobeCloudDrive/`
   * **창:** `C:\Users\<username>\AppData\Local\Temp\Adobe\AdobeCloudDrive\`

### 프로젝트 폴더에 파일의 충돌하는 복사본이 표시됨

**원인:** 두 사용자가 한 버전이 클라우드에 동기화되기 전에 동일한 파일에 변경 내용을 저장했습니다. Adobe Cloud Drive는 두 버전을 모두 자동으로 보존했습니다.

충돌하는 복사본은 다음과 같은 이름 지정 형식을 사용합니다. `filename (Conflicted copy from device_name on date_time).extension`
예: `project_brief (Conflicted copy from jsmith's MacBook Pro on 2026-06-15-10-45-19).docx`

**해상도:**

1. 두 사용자에게 어느 버전이 신뢰할 수 있는지 물어봅니다.
1. 충돌하는 복사본에서 필요한 모든 콘텐츠를 기본 파일로 복사합니다.
1. 두 버전을 조정한 후 충돌하는 복사본을 삭제합니다.

   >[!NOTE]
   >
   >Adobe Cloud Drive에서는 파일 잠금을 사용하지 않습니다. 여러 사용자가 동일한 파일을 편집할 때 충돌이 발생하지 않도록 하려면 여러 사용자가 데스크탑에서 동일한 파일에 액세스하기 전에 Workfront 작업 할당 또는 승인 워크플로우를 통해 편집을 조정합니다.

### 사용자가 프로젝트에 폴더 또는 파일을 만들 수 없음

**원인 A:** 사용자가 프로젝트 루트 수준에서 폴더 또는 파일을 만들려고 합니다. 프로젝트 루트 폴더는 현재 Adobe Cloud Drive에서 읽기 전용입니다. 루트 수준 폴더는 Workfront에서 만들고 관리하는 Workfront 프로젝트를 나타냅니다.

**해상도:**

1. 사용자에게 프로젝트 내의 기존 하위 폴더로 이동하여 파일이나 폴더를 만들도록 요청합니다.
1. 사용자에게 프로젝트 내에 새 최상위 폴더가 필요한 경우 먼저 Workfront에서 만들도록 요청하십시오. 그런 다음 Adobe Cloud Drive에 표시됩니다.

**원인 B:** 사용자에게 Workfront 프로젝트에 대한 편집 권한이 없습니다.

**해상도:**

1. Workfront에서 프로젝트에 대한 사용자의 권한을 확인합니다(**보기**, **기여** 또는 **관리**).
1. 파일을 만들거나 편집해야 하는 경우 사용자의 권한을 **Contribute** 또는 **Manage**(으)로 업데이트하십시오.
