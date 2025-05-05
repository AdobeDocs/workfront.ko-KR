---
content-type: reference
navigation-topic: announcements
title: 이메일 스푸핑 및 POP 회신 제거
description: Adobe Workfront이 20.3 릴리스(2020년 8월 목표)를 사용하여 이메일을 보내고 받는 방식을 두 가지 변경하고 있습니다.
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 이메일 스푸핑 및 POP 회신

Adobe Workfront이 20.3 릴리스(2020년 8월 목표)를 사용하여 이메일을 보내고 받는 방식을 두 가지 변경하고 있습니다.

## Workfront의 아웃바운드 이메일

이메일의 성공적인 전달을 높이기 위해 스팸으로 태그가 지정된 이메일의 스푸핑을 제거합니다(이메일 스푸핑 참조). 자동 알림 및 사용자와 사용자 간 통신을 포함하여 Workfront의 모든 전자 메일이 `notifications@my.workfront.com`에서 전송됩니다. Joan Harris의 예제 이메일은 이메일의 출처 영역에서 다음과 같이 표시됩니다.

![전자 메일 예제](assets/noreply.png)

*IT 팀에 문의*&#x200B;하여 `notifications@my.workfront.com`의 전자 메일이 시스템에 들어오는 전자 메일에 대해 차단되지 않도록 하는 것이 좋습니다. 트래픽 및 전자 메일의 IP 주소에 대한 자세한 내용은 [방화벽 허용 목록 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조할 수도 있습니다.

## 알림에 대한 인바운드 이메일 회신(POP 회신)

특정 이메일 알림을 사용하면 이메일을 통해 답장을 보낼 수 있으며, Workfront 시스템에서 답장을 댓글 답장으로 Workfront에 복사할 수 있습니다. Workfront의 시스템 관리자는 일반적으로 이러한 응답을 수신하기 위해 자체 POP 이메일 서버를 제공하거나 내장된 Workfront 회신 시스템을 사용할 수 있습니다. 사용자 지정 POP 이메일 서버 선택 항목은 20.3 릴리스에서 제거됩니다. 사용자 지정 서버를 사용하도록 구성된 모든 계정은 자동으로 기본 Workfront 이메일 회신 시스템을 사용하도록 전환됩니다. 시스템 관리자나 다른 Workfront 사용자에게는 필요한 작업이 없습니다.

Workfront Proof 시스템에서 직접 전송되는 이메일은 변경되지 않습니다. 이전과 마찬가지로 해당 이메일을 계속 수신하게 됩니다.

다른 질문이 있거나 문제가 있는 경우 [Workfront 지원 팀](https://experienceleague.adobe.com/ko?support-tab=home#support)에 문의하십시오.
