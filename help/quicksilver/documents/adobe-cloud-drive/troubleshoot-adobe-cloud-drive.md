---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Adobe 클라우드 드라이브 문제 해결
description: Mac 및 Windows에서 Adobe Cloud Drive와 관련된 일반적인 문제에 대한 제한 사항, 성능 고려 사항 및 솔루션을 검토합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6ad89f8d00dd3a06eb160863c3213a9f80b1a44b
workflow-type: tm+mt
source-wordcount: 928
ht-degree: 0%

---

# Adobe 클라우드 드라이브 문제 해결

이 문서에서는 Adobe Cloud Drive의 제한 사항, 염두에 두어야 할 성능 고려 사항 및 발생할 수 있는 일반적인 문제에 대한 해결 방법에 대해 설명합니다.

Adobe Cloud Drive 사용에 대한 자세한 내용은 [Adobe Cloud Drive 사용](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)을 참조하세요.

## 제한 사항

### 파일 및 폴더 작업

* 프로젝트 폴더는 최상위 수준에서 읽기 전용입니다. Adobe 클라우드 드라이브에서는 이름을 바꾸거나, 삭제하거나, 이동할 수 없습니다. 프로젝트를 만들거나, 이름을 바꾸거나, 삭제하려면 Workfront 웹 인터페이스를 사용하십시오.
* 프로젝트 폴더 내의 파일 및 폴더 작업은 완전히 지원됩니다.

### 파일 및 경로 제한

* 모든 플랫폼에서 파일 이름은 255자를 초과할 수 없습니다.
* 전체 파일 경로(모든 폴더 이름과 파일 이름)는 1,024자를 초과할 수 없습니다. 이 제한보다 긴 경로를 가진 파일은 Adobe 웹 인터페이스에 표시되더라도 Workfront Cloud Drive에 표시되지 않습니다.
* 파일에 **전체 경로가 너무 깁니다** 오류가 표시되면 폴더 이름을 줄이거나 폴더 중첩 깊이를 줄여 경로를 제한 이내로 만드십시오.

### 스토리지

* Adobe Cloud Drive에 저장된 파일은 장치의 디스크 공간을 로컬로 사용합니다.
* 클라우드 전용 파일은 로컬 저장소를 사용하지 않습니다.
* 더 이상 필요하지 않은 파일에 대한 오프라인 액세스를 제거합니다. 자세한 내용은 [Adobe 클라우드 드라이브 사용](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)에서 [오프라인 액세스 제거를 통해 사용 가능한 공간](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space)을 참조하세요.

## 성능 고려 사항

* **파일 크기:** 동기화에 필요한 시간은 파일 크기에 따라 다릅니다. 일반적으로 파일이 클수록 시간이 오래 걸립니다.
* **네트워크 속도:** 연결 속도가 빨라져 동기화 성능이 향상됩니다. 중단 후 동기화가 자동으로 다시 시작됩니다.
* **처음 액세스:** 처음 액세스할 때 필요할 때 파일이 다운로드됩니다. 파일이 로컬로 캐시되므로 이후 액세스가 더 빨라집니다.

## 일반적인 문제

### Adobe Cloud Drive가 표시되지 않습니다

**가능한 원인:**

* Adobe Cloud Drive가 설치되지 않았습니다.
* 설치가 완료되지 않았습니다.
* 조직은 Adobe 클라우드 스토리지를 지원하는 Workfront 버전을 사용하지 않습니다.

**솔루션:**

* Adobe Cloud Drive가 설치되었는지 확인합니다. **응용 프로그램**(Mac) 또는 **프로그램**(Windows)을 확인하세요.
* Adobe Cloud Drive를 수동으로 시작합니다.
* Workfront 관리자에게 문의하여 조직이 Adobe 클라우드 스토리지를 지원하는 Workfront 버전을 사용하고 있는지 확인하십시오.
* 필요한 경우 Adobe Cloud Drive를 다시 설치합니다. 자세한 내용은 [Adobe 클라우드 드라이브 설치](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)를 참조하십시오.

### Adobe Cloud Drive 아이콘이 메뉴 모음 또는 작업 표시줄에 표시되지 않습니다

**가능한 원인:**

* 메뉴 모음(Mac) 또는 시스템 트레이(Windows)에 아이콘을 표시할 공간이 부족합니다.

**솔루션:**

* **Mac:** Cmd를 누른 채 기존 메뉴 모음 아이콘을 끌어서 다시 정렬하거나 제거하고 Adobe Cloud Drive 아이콘에 대한 공간을 만듭니다.
* **Windows:** 작업 표시줄에서 위쪽 화살표(**숨겨진 아이콘 표시**)를 클릭하여 Adobe Cloud Drive 아이콘을 찾은 다음 표시 영역으로 끌어서 놓습니다.

### 프로젝트가 표시되지 않거나 일부 프로젝트가 누락되었습니다.

**가능한 원인:**

* 프로젝트에 대한 액세스 권한이 없습니다.
* 동기화가 완료되지 않았습니다.
* 네트워크 연결 문제가 있습니다.

**솔루션:**

* Workfront 웹 인터페이스에서 프로젝트 액세스를 확인합니다.
* 네트워크 연결을 확인합니다.
* Adobe Cloud Drive에서 로그아웃했다가 다시 로그인하세요.

### 파일이 동기화되지 않음

**가능한 원인:**

* 네트워크 연결 문제가 있습니다.
* 파일 또는 폴더에 동기화 오류가 있습니다.
* 디스크 공간이 부족합니다.

**솔루션:**

* 인터넷 연결을 확인합니다.
* 사용 가능한 디스크 공간이 충분한지 확인합니다.
* 파일 상태 표시기에서 동기화 오류를 확인합니다. 자세한 내용은 [Adobe 클라우드 드라이브 사용](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)에서 [파일 상태 표시기](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators)를 참조하십시오.
* Adobe 클라우드 드라이브를 다시 시작합니다.
* 시스템 트레이(Windows) 또는 메뉴 모음(Mac)에서 Adobe Cloud Drive 상태를 확인합니다.

### 파일을 열 수 없습니다.

**가능한 원인:**

* 파일이 클라우드 전용이며 다운로드하지 못했습니다.
* 파일을 여는 데 필요한 응용 프로그램이 설치되지 않았습니다.
* 파일이 손상되었습니다.

**솔루션:**

* 파일 상태 표시기를 확인합니다.
* 필요한 응용 프로그램이 설치되어 있는지 확인합니다.
* 파일을 마우스 오른쪽 단추로 클릭하고 **이 장치에서 항상 유지**&#x200B;를 선택한 다음 다시 열어 보십시오.
* Workfront 웹 인터페이스에서 파일이 손상되지 않았는지 확인합니다.

### 동기화가 느림

**가능한 원인:**

* 파일이 큽니다.
* 네트워크 연결이 느립니다.
* 많은 파일이 동시에 동기화됩니다.

**솔루션:**

* 대용량 파일에 대해 인내심을 가지십시오. 동기화가 다시 시작될 수 있으므로 중단 후 중지된 위치가 선택됩니다.
* 네트워크 속도를 확인합니다.
* 동시 파일 작업 수를 제한합니다.
* 오프라인 액세스가 필요하지 않은 경우 대용량 파일을 클라우드 전용으로 유지합니다.

### 오프라인 파일에 너무 많은 공간이 소요됩니다.

**솔루션:**

* 오프라인 파일을 마우스 오른쪽 단추로 클릭하고 **공간 사용**&#x200B;을 선택합니다.
* 정기적으로 디스크 공간을 확인하십시오.
* 거의 액세스하지 않는 큰 파일은 클라우드 전용 모드로 유지합니다.

### 파일 또는 폴더를 만들거나 편집하거나 삭제할 수 없습니다

**가능한 원인:**

* 프로젝트 폴더를 만들거나 이름을 바꾸거나 삭제하려고 합니다. 프로젝트 폴더는 최상위 수준에서 읽기 전용입니다.
* 프로젝트가 읽기 전용이므로 이 프로젝트 내에서 파일이나 폴더를 만들거나 편집하거나 삭제할 수 없습니다.

**솔루션:**

* 프로젝트를 만들거나, 이름을 바꾸거나, 삭제하려면 Workfront 웹 인터페이스를 사용하십시오.
* 프로젝트 소유자에게 편집 액세스 권한이 있는 사용자와 프로젝트를 공유하도록 요청하십시오.

## 도움말 보기

라이선스 질문, 프로젝트 액세스 문제 또는 조직별 구성은 Workfront 관리자에게 문의하십시오.

Adobe 지원 팀과 로그를 공유하려면 [Adobe 로그 수집기 도구 실행](https://helpx.adobe.com/kr/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html)의 단계를 따르십시오.

## 모범 사례

* **오프라인 작업을 계획합니다.** 여행하거나 연결이 좋지 않은 지역에서 작업하기 전에 파일을 다운로드하십시오.
* **동기화 상태를 모니터링합니다.** 응용 프로그램을 닫기 전에 파일 표시기를 확인하십시오.
* **프로젝트의 폴더 구조를 따릅니다.** 프로젝트 소유자가 의도하는 대로 프로젝트 폴더 내에 파일을 구성합니다.
* **설명 파일 이름을 사용합니다.** 팀원이 필요한 항목을 찾을 수 있도록 지원합니다.
* **중복 항목을 만들지 마십시오.** 불필요한 파일 복사본을 만들지 마십시오.
