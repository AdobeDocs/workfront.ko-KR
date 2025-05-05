---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Power BI 도구는 제공된 암호로 연결할 수 없습니다.
description: Power BI 도구에서 Data Connect에 로그인하려고 하면 로그인 오류가 표시됩니다.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 40050915153af6e1f70024461e193fb536d74e35
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---


# Power BI 도구는 제공된 암호와 연결할 수 없습니다.

## 문제

Power BI 도구에서 Data Connect에 로그인하려고 하면 다음 오류가 표시됩니다.

`Cannot connect from BI tool with provided password`

## 원인

JDBC 연결을 생성할 때 Workfront은 Data Connect에 임시 암호를 제공합니다.

Power BI을 통해 Data Connect에 액세스하려면 먼저 제공된 연결 세부 정보를 사용하여 로그인하고 임시 암호를 업데이트한 다음 로그인을 진행해야 합니다.


## 솔루션

Workfront에서 연결 암호를 재설정한 다음 연결 편집 대화 상자에 제공된 링크로 새 암호를 만드십시오.

### Workfront에서 연결 암호 재설정

1. Workfront > 설정 > 시스템 > Data Connect로 이동합니다.
1. 목록에서 연결을 찾아 엽니다.
1. **연결 암호 재설정**&#x200B;에서 암호를 재설정할지 확인하는 상자를 선택합니다.
1. **연결 암호 재설정**&#x200B;을 클릭합니다.
   ![연결 암호 재설정](assets/reset-password.png)
1. 아래 섹션으로 이동합니다.

### 연결에 대한 새 암호 만들기

1. URL을 복사하여 새 브라우저 탭에 붙여넣습니다.
1. Workfront에서 연결 사용자 이름과 기본 암호를 복사하여 새 브라우저 탭에 붙여넣습니다.
   ![url 및 기본 암호 복사](assets/link-password.png)
1. **로그인**&#x200B;을 클릭합니다.
1. 새 암호를 입력한 다음 **제출**&#x200B;을 클릭합니다.
1. Power BI 도구로 이동한 다음 새 암호로 로그인합니다.

