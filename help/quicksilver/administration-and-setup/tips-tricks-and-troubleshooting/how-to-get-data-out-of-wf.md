---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Adobe Workfront에서 이전 데이터 내보내기: 장단점'
description: 이 문서에서는 Workfront에서 내역 데이터를 내보내는 데 사용할 수 있는 4가지 옵션의 장단점에 대해 설명합니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 내역 데이터 내보내기 [!DNL Adobe Workfron]t: 장단점

이 문서에서는 내역 데이터를 내보내는 데 사용할 수 있는 4가지 옵션의 장단점을 설명합니다 [!DNL Workfront].

## 파트너 중 한 명 사용

[!DNL AtAppStore], a [!DNL Workfront] certified partner 에는 데이터를 다운로드할 수 있는 사용하기 쉬운 앱이 있습니다. 이 앱에는 데이터를 쉽게 볼 수 있는 뷰어도 포함되어 있습니다.

* **장점:** 내 모든 항목 [!DNL Workfront] 사용자 정의 필드를 포함하여 객체를 내보냅니다. Viewer의 인터페이스는 쉽게 사용하고 읽을 수 있으며 [!DNL MS Access] 데이터베이스.

* **단점:** 문서는 내보내지 않습니다. 따로 다운로드하셔야 합니다 자세한 내용을 보려면 [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx입니다.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## 요청 a [!DNL Postgres] 데이터베이스 팀의 데이터 덤프 파일

계정 관리자는 데이터베이스 팀에 데이터베이스 덤프 파일(.dmp)을 내보내도록 요청을 제출할 수 있습니다. [!DNL Postgres] 파일)을 클릭하여 제품에서 사용할 수 있습니다. 저장된 모든 문서를 검색하기 위해 추가 요청이 AOS 팀으로 이동합니다.

* **장점**: 시스템에 저장된 문서는 물론 사용자 정의 필드를 포함하여 전체 데이터를 로드합니다.

* **단점**: 데이터베이스 파일을 읽기가 어려움: 이 파일을 다음에 업로드하지 않으면 읽을 수 있는 방법이 없습니다. [!DNL Postgres] 데이터베이스 및 테이블 간의 관계를 재설정합니다. 문서는 별도의 파일 서버에 저장되며 AOS 팀에서 별도의 프로세스를 사용하여 별도로 추출해야 합니다. 이렇게 하면 문서에 대한 조직이 없으며 해당 문서가 모두 GUID에 의해 참조됩니다.
* **비용**: 팀이 파일을 만드는 데 걸리는 시간에 따라 이 다운로드와 관련된 비용이 있습니다. 자세한 내용을 확인하거나 이 프로세스를 시작하려면 AE/CAE에 문의하십시오.

## 를 통해 내보내기 [!UICONTROL 킥스타트]

원격 컨설팅 시간이 있든 없든 당사의 컨설턴트 중 한 명을 사용하여 보고서나 [!UICONTROL 킥스타트]또는 다음 보고서를 직접 실행할 수 있습니다.

* **장점**: 보고서는 읽기 쉽고 다양한 애플리케이션으로 가져올 수 있으며, 원하는 그룹화 및 보기를 포함하도록 사용자 지정할 수 있습니다.

* **단점**: 문서는 별도로 다운로드해야 합니다.

* **비용**: 보고서를 직접 실행할 수 있는 경우(시스템 관리자 로그인만 필요한 경우) 또는 나머지 원격 컨설팅 시간을 사용할 수 있는 경우 무료입니다. 원격 컨설팅을 구입하는 데 관심이 있다면 AE/CAE에 문의하십시오.

  킥스타트를 사용하여 데이터를 내보내는 방법에 대한 자세한 내용은 [데이터 내보내기 [!DNL Adobe Workfront] 경유 [!UICONTROL 킥스타트]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## 개방형 API 사용

조직에 적절한 리소스가 있는 경우, Workfront에서 모든 데이터를 검색하기 위한 사용자 지정 API를 빌드할 수 있습니다.

* **장점**: 시스템에서 내보내는 내용을 제어합니다.

* **단점**: 시간이 사용자 쪽에서 소요되며 API를 코딩하고 내보내기를 수행할 리소스를 찾아야 합니다.

* **비용**: 조직 내부
