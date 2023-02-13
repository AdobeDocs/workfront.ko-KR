---
content-type: reference
navigation-topic: announcements
title: 이메일 스푸핑 및 POP 회신 제거
description: Adobe는 20.3 릴리스(2020년 8월 타깃팅)를 통해 Adobe Workfront이 이메일을 보내고 받는 방식을 두 가지 변경되었습니다.
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 이메일 스푸핑 및 POP 회신

Adobe는 20.3 릴리스(2020년 8월 타깃팅)를 통해 Adobe Workfront이 이메일을 보내고 받는 방식을 두 가지 변경되었습니다.

## Workfront의 아웃바운드 이메일

이메일의 성공적인 게재를 늘리기 위해 스팸으로 종종 태그가 지정되는 이메일의 스푸핑을 방지할 것입니다(이메일 스푸핑 참조). 자동화된 경고 및 사용자 대 사용자 통신을 포함하여 Workfront의 모든 이메일이 notifications@my.workfront.com에서 전송됩니다. Joan Harris의 예제 이메일은 :

![](assets/noreply.png)

*IT 팀에 문의하는 것이 좋습니다* notifications@my.workfront.com의 이메일이 시스템에 들어오는 이메일에 대해 차단되지 않도록 하려면 다음을 수행하십시오. 참조할 수도 있습니다 [방화벽 허용 목록에 추가하다 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 트래픽 및 이메일에서 가져오는 IP에 대한 자세한 정보.

## 알림에 인바운드 전자 메일 회신(POP 회신)

특정 이메일 알림을 사용하면 사용자가 이메일을 통해 회신하고 해당 응답을 Workfront 시스템의 댓글 응답으로 Workfront에 복사할 수 있습니다. Workfront의 시스템 관리자는 일반적으로 이러한 응답을 받을 수 있도록 자체 POP 이메일 서버를 제공하거나 내장된 Workfront 회신 시스템을 사용할 것인지 선택할 수 있었습니다. 사용자 지정 POP 이메일 서버 선택이 20.3 릴리스에서 제거됩니다. 사용자 지정 서버를 사용하도록 구성된 모든 계정은 자동 전환되어 기본 Workfront 이메일 회신 시스템을 사용합니다. 시스템 관리자 또는 다른 Workfront 사용자에게 필요한 작업이 없습니다.

Workfront 증명 시스템에서 직접 오는 이메일에는 변경되지 않습니다. 과거에 그랬던 것처럼 계속 해당 이메일을 받게 됩니다.

기타 문의 사항이나 우려 사항이 있는 경우 [Workfront 지원 팀](https://one.workfront.com/s/support?language=en_US).
