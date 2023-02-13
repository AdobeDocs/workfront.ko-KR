---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Adobe Workfront에서 이전 데이터 내보내기: 장단점'
description: 이 문서에서는 Workfront에서 이전 데이터를 내보내는 데 사용할 수 있는 4가지 옵션의 장단점에 대해 설명합니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 다음에서 이전 데이터 내보내기 [!DNL Adobe Workfron]t: 장단점

이 문서에서는 [!DNL Workfront].

## 파트너 중 하나를 사용합니다.

[!DNL AtAppStore], [!DNL Workfront] 인증된 파트너에게는 데이터를 다운로드할 수 있는 사용하기 쉬운 앱이 있습니다. 또한 이 앱에는 데이터를 쉽게 볼 수 있는 뷰어가 포함되어 있습니다.

* **장점:** 모든 사용자 [!DNL Workfront] 사용자 정의 필드를 포함한 개체를 내보냅니다. 뷰어의 인터페이스는 사용 및 읽기가 쉽고, [!DNL MS Access] 데이터베이스.

* **단점:** 문서를 내보내지 않습니다. 따로 다운로드하셔야 합니다 자세한 내용을 보려면 [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## 요청 [!DNL Postgres] 데이터베이스 팀의 데이터 덤프 파일

계정 관리자가 데이터베이스 덤프 파일(.dmp)을 내보내도록 요청을 데이터베이스 팀에 제출할 수 있습니다 [!DNL Postgres] 파일)을 만들 수 있습니다. 저장된 모든 문서를 검색하기 위해 AOS 팀에 추가 요청이 전송됩니다.

* **장점**: 사용자 정의 필드를 비롯하여 시스템에 저장된 전체 데이터 로드를 가져옵니다.

* **단점**: 데이터베이스 파일을 읽기 어렵습니다. 이 파일을 [!DNL Postgres] 데이터베이스 및 테이블 간의 관계를 다시 설정합니다. 문서는 별도의 파일 서버에 저장되며 AOS 팀이 별도의 프로세스를 사용하여 별도로 추출해야 합니다. 이렇게 하면 문서에 대한 조직이 없으며 모두 해당 GUID에서 참조됩니다.
* **비용**: 팀이 파일을 만드는 데 걸리는 시간에 따라 이 다운로드와 관련된 비용이 있습니다. 자세한 내용을 확인하거나 이 프로세스를 시작하려면 AEM/CAE에 문의하십시오.

## 를 통해 내보내기 [!UICONTROL 킥스타트]

원격 컨설팅 시간이 있는지 여부에 관계없이 Adobe 컨설턴트 중 하나를 사용하여 데이터를 보고서 형식으로 내보내거나 [!UICONTROL kick-starts]또는 다음 보고서를 직접 실행할 수 있습니다.

* **장점**: 보고서는 읽기 쉽고 다양한 애플리케이션에서 가져올 수 있습니다. 원하는 그룹화 및 보기를 포함하도록 사용자 지정할 수 있습니다.

* **단점**: 서류를 따로 다운로드해야 할 것이다.

* **비용**: 보고서를 직접 실행하거나(시스템 관리자 로그인이 필요한 경우) 원격 컨설팅 시간을 사용할 수 있는 경우에는 무료입니다. 원격 컨설팅 구매에 관심이 있는 경우 AEM/CAE와 상의하십시오.

   Kick-Starts를 사용하여 데이터를 내보내는 방법에 대한 자세한 내용은 [데이터 내보내기 위치 [!DNL Adobe Workfront] via [!UICONTROL 킥스타트]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## 열린 API 사용

조직에 올바른 리소스가 있는 경우 Workfront에서 모든 데이터를 검색하는 사용자 지정 API를 만들 수 있습니다.

* **장점**: 당신은 시스템에서 수출되는 것을 통제하고 있다.

* **단점**: 시간이 소비되며 API를 코딩할 리소스를 찾아 내보내야 합니다.

* **비용**: 조직 내부.
