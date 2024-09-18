---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 여러 브라우저 탭으로 인해 Workfront이 로그아웃됨
description: 사용자가 여러 개의 브라우저 탭을 열어 놓은 경우 Workfront에서 자동으로 로그아웃될 수 있습니다.
feature: Get Started with Workfront
source-git-commit: ef85b267b3417dddd0c9cc4a2b916b83dc416e14
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 7%

---

# 여러 브라우저 탭으로 인해 Workfront이 로그아웃됨

>[!IMPORTANT]
>
>이 문제는 Adobe IMS에 온보딩된 조직에만 적용됩니다.

## 문제

사용자가 여러 브라우저 탭을 열고 일정 시간 동안 비활성 상태인 탭을 클릭하면 탭 세션이 만료됩니다. 사용자가 연 페이지를 볼 수 없고 대신 다음 메시지가 표시됩니다.

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## 이유

이 동작은 조직에서 구성한 보안 조치인 PBA(정책 기반 인증) 때문입니다. 조직의 PBA 구성에 설정된 시간 이상 탭이 비활성 상태이면 탭 세션이 만료됩니다.

## 솔루션

해결 방법은 Workfront에 로그인한 다른 탭에서 활성화했는지 여부에 따라 다릅니다.

* 활성 Workfront 탭이 열려 있는 경우 만료된 탭을 다시 로드합니다. 만료되기 전에 열었던 페이지로 돌아갑니다.

* 활성 Workfront 탭이 열려 있지 않으면 Workfront에 다시 로그인하십시오.