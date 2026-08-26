---
title: 클라우드 코드 스킬로 App Builder 앱 구축
description: 설정 및 배포 단계를 직접 실행하는 대신 클라우드 코드 스킬 세트를 사용하여 원하는 내용을 설명함으로써 사용자 정의 Adobe Workfront App Builder 앱을 빌드할 수 있습니다.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: 366cc4ffea48295b00389b5ee36f2df42b2c8a07
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 4%

---


# 클라우드 코드 스킬로 App Builder 앱 구축

스킬 패키지를 통해 [!DNL Claude]&#x200B;(또는 클라우드 형식 스킬을 지원하는 모든 AI 코딩 활용(예: [!DNL Claude Code] 또는 [!DNL OpenAI Codex])이 [!DNL Workfront]에 대한 사용자 지정 [!DNL Adobe App Builder] 앱을 빌드할 수 있습니다. 이러한 도구 중 하나에 액세스할 수 있는 경우 개발자 경험이나 수동 설정 단계 없이 원하는 내용을 일반 영어로 설명하여 UI 확장을 구축할 수 있습니다.

Adobe App Builder 기반의 Workfront UI 확장 기능을 사용하면 고객과 파트너가 맞춤화된 사용자 경험을 만들 수 있습니다. UI 확장을 사용하면 조직의 요구 사항을 더 잘 충족하도록 조직의 Workfront 경험을 수정할 수 있으므로 효율성을 높이고 원활한 연결 경험을 제공하며 사용자 만족도를 크게 향상시킬 수 있으며 조직이 고유한 비전을 실현하는 데 도움이 됩니다.

Workfront UI 확장에 대한 자세한 내용은 [Adobe App Builder을 사용하여 Workfront용 사용자 지정 응용 프로그램 만들기](/help/quicksilver/app-builder/app-builder.md)를 참조하십시오.

## UI 확장성 기술

UI 확장성 기술을 사용하면 AI 코딩 하네스가 Workfront에서 UI 확장 생성을 관리할 수 있습니다. 원하는 기능에 대해 설명하고 도구 설정, [!DNL Adobe App Builder]에서 프로젝트 만들기, 앱 빌드, Adobe 클라우드에 배포, Workfront 내에서 실행 등의 실습 작업을 수행합니다. 사용자의 작업이 필요한 결정 또는 로그인이 있는 경우에만 프로세스에 참여합니다. 이 문서에서는 [!DNL Claude]을(를) 예로 사용하지만, 지침은 클라우드 스킬을 지원하는 모든 AI 코딩 하네스에 적용됩니다.

## 전제 조건

시작하기 전에 다음을 확인하십시오.

* **클라우드 기술을 지원하는 AI 코딩 도구**(예: [!DNL Claude Code]).

  클라우드 스킬에 대한 자세한 내용은 [스킬이란?](https://support.claude.com/en/articles/12512176-what-are-skills)을(를) 참조하십시오. Claude 설명서에서 참조할 수 있습니다.

* **스킬에 액세스**.

  * [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md)에서 기술을 찾을 수 있습니다.

    이 링크가 열리지 않으면 관리자에게 액세스 권한을 요청하십시오.
  * 스킬은 Adobe의 공개 스킬 마켓플레이스([adobe/스킬](https://github.com/adobe/skills))에 게시됩니다. [!DNL Claude Code]에서 다음을 실행합니다.

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* **[!DNL Adobe App Builder]액세스, 개발자 역할**. Adobe 조직에는 App Builder 라이선스가 필요하며 이 라이선스에 개발자로 추가되어 있어야 합니다. 이를 통해 [!DNL Claude]에서 Adobe Developer Console을 열고 프로젝트를 만들 수 있습니다.

  이 전제 조건이 충족되는지 확인하려면 다음을 수행하십시오.

  1. [Adobe Developer Console](https://developer.adobe.com/console)을 엽니다.
  1. 오른쪽 상단 모서리에 표시된 조직이 올바른지 확인합니다.
  1. **새 프로젝트 만들기** > **템플릿에서 프로젝트 만들기**&#x200B;를 클릭합니다.
  1. **App Builder**&#x200B;이(가) 목록에 있는지 확인하십시오.

     * 목록에 **App Builder**&#x200B;이(가) 표시되면 액세스 권한이 있는 것입니다.
     * **템플릿에서 프로젝트 만들기** 옵션이 없거나 **App Builder** 옵션이 없으면 아직 액세스 권한이 없습니다. Workfront 또는 Adobe 관리자에게 사용자를 개발자로 추가하도록 요청하고( Adobe Admin Console > 사용자 > 개발자에서) 조직에 App Builder 라이센스가 있는지 확인합니다.
* **Workfront MCP 서버가 연결되었습니다**. 따라서 [!DNL Claude]은(는) 데이터 형식, 필드 및 명령에서 추측하는 대신 실제 Workfront API를 사용합니다.

  Workfront MCP 서버가 이미 연결되어 있는지 확인하려면 [!DNL Claude]에게 문의하십시오. *&quot;Workfront MCP 리소스를 볼 수 있습니까?&quot;*

  자세한 내용 및 지침은 Adobe Workfront MCP 서버 구성 문서에서 [Workfront과 클라우드 연결](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)을 참조하십시오.
