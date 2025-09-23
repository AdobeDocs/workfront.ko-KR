---
title: AI Assistant 프롬프트 우수 사례
content-type: reference
description: AI Assistant 사용 모범 사례에 대해 알아보고 프롬프트 예제 목록을 볼 수 있습니다.
author: Jenny
feature: Get Started with Workfront
exl-id: 34a60482-e060-49f9-bbaf-8aed85845e26
source-git-commit: 4bab0129d694d7134a5dae90474678226368ca78
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 4%

---

# AI Assistant 프롬프트 우수 사례

Workfront의 AI Assistant는 계정 데이터 및 특정 객체 유형에 대한 유용한 정보를 제공하여 작업을 보다 효과적으로 완수할 수 있는 강력한 도구입니다.

이 문서에서는 명확한 프롬프트를 작성하는 방법, 정보를 요청할 수 있는 개체 유형, 필요한 경우 정보를 확인하기 위해 추가 리소스에 액세스하는 방법 등 AI Assistant에 대한 현재 모범 사례에 대해 알아봅니다.

AI Assistant에 대한 자세한 내용은 [AI Assistant 개요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)를 참조하십시오.

>[!NOTE]
>
>AI Assistant의 기능이 발전함에 따라 사용자가 물어볼 수 있는 요청 및 질문 유형이 확장됩니다. 사용할 수 있는 프롬프트에 대한 자세한 내용을 보려면 새 AI Assistant 기능이 릴리스되었으므로 이 문서를 다시 참조하는 것이 좋습니다.


## AI Assistant에 사용 가능한 객체 유형

AI 어시스턴트는 다음 객체 유형에 대한 데이터를 제공할 수 있습니다.

* 포트폴리오
* 프로그램
* 프로젝트
* 작업
* 문제
* 사용자 정의 양식
* 사용자
* Workfront 계획 레코드

>[!NOTE]
>
>AI Assistant에서 해당 데이터를 요청하려면 먼저 오브젝트에 대한 액세스 수준에서 필요한 권한이 있어야 합니다.

## 모범 사례

### 지우기 프롬프트 입력

AI Assistant에서 가장 유용한 정보에 액세스하려면 원하는 응답을 제공하는 프롬프트를 생성하는 것이 중요합니다. 다음 목록에는 적절한 프롬프트를 가장 잘 작성하는 데 도움이 되는 원칙이 포함되어 있습니다.

* **명확하고 특정한 언어를 사용하십시오**: 모호한 일반적인 프롬프트를 피하면 AI Assistant에서 수신하려는 데이터를 안내하는 데 도움이 됩니다.
* **일정 포함**: 개체에 대한 AI Assistant의 특정 일정을 제공하면 처리하는 데 필요한 데이터의 범위를 좁힐 수 있으며 응답에 더 많은 타깃팅된 정보가 생성됩니다.
* **한 번에 하나만 묻기**: 관련이 없는 여러 요청이 단일 프롬프트에 포함되어 있으면 AI 지원에서 올바른 정보를 제공할 수 없습니다.

권장 프롬프트에 대한 자세한 내용은 이 문서에서 다음 섹션을 참조하십시오. [프롬프트 예](#prompt-examples).


### AI Assistant 응답 확인

AI Assistant 개발 중 이 단계에서는 Workfront 프로세스에 대한 정보를 요청할 때 AI가 제공하는 정보를 확인하는 것이 좋습니다. 이렇게 하려면 프롬프트 응답의 소스 섹션에 제공된 문서 링크를 클릭할 수 있습니다.

![소스 섹션](assets/sources-section.png)

Workfront 프로세스에 대한 프롬프트에 대한 자세한 내용은 이 문서에서 [Workfront 작업에 대한 자세한 정보를 확인하는 프롬프트](#prompts-to-learn-about-workfront-actions)를 참조하십시오.


## 프롬프트 예

아래 표에는 작업에 대한 정보를 생성하고 특정 Workfront 프로세스 또는 수행할 작업에 대해 자세히 알아보는 데 사용할 수 있는 프롬프트 예가 나와 있습니다.

### 작업에 대한 정보를 찾으라는 메시지 표시

<table>
    <tr>
        <td><b>오브젝트 유형</b></td>
        <td><b>프롬프트</b></td>
    </tr>
        <tr>
        <td>프로젝트</td>
        <td><em>[PROJECT NAME]의 기한은 언제입니까?</em>
        </td>
    </tr>
    <tr>
        <td>프로젝트</td>
        <td><em>[PROJECT NAME]의 상태는 무엇입니까?</em>
        </td>
    </tr>
    <tr>
        <td>프로젝트 </td>
        <td><em>[PROJECT NAME]의 프로젝트 소유자</em></td>
    </tr>
    <tr>
        <td>작업</td>
        <td><em>이번 주에 나에게 할당된 업무는 무엇입니까?</em></td>
    </tr>
       <tr>
        <td>문제 </td>
        <td><em>내 팀에는 어떤 진행 중 문제가 할당됩니까?</em></td>
           <tr>
        <td>사용자</td>
        <td><em>[PROJECT NAME] 크리에이티브 팀은 누구입니까?</em></td>
    </tr>
           <tr>
        <td>사용자 </td>
        <td><em>[USER]에게 몇 개의 작업이 할당됩니까?</em></td>
    </tr>
   </table>


### Workfront 작업에 대한 자세한 내용을 묻는 메시지 표시

<table>
    <tr>
        <td><b>오브젝트 유형</b></td>
        <td><b>프롬프트</b></td>
    </tr>
    <tr>
        <td>프로젝트</td>
        <td><em>템플릿에서 새 프로젝트를 만들려면 어떻게 해야 합니까?</em>
        </td>
    </tr>
    <tr>
        <td>프로젝트 </td>
        <td><em>프로젝트와 프로그램의 차이점은 무엇입니까?</em></td>
    </tr>
    <tr>
        <td>작업</td>
        <td><em>여러 사용자에게 작업을 할당하려면 어떻게 합니까?</em></td>
    </tr>
       <tr>
        <td>작업</td>
        <td><em>시작 준비 상태는 무엇을 의미합니까?</em></td>
    </tr>
       <tr>
        <td>문제 </td>
        <td><em>요청을 작업으로 전환하려면 어떻게 해야 합니까?</em></td>
    </tr>
           <tr>
        <td>문제 </td>
        <td><em>Workfront 문제의 라이프사이클은 무엇입니까?</em></td>
    </tr>
        </tr>
           <tr>
        <td>문제 </td>
        <td><em>요청을 에스컬레이션하려면 어떻게 해야 합니까?</em></td>
    </tr>
           <tr>
        <td>문서</td>
        <td><em>새 버전의 문서를 업로드하려면 어떻게 해야 합니까?</em></td>
    </tr>
           <tr>
        <td>문서 </td>
        <td><em>문서 승인 워크플로를 설정할 수 있습니까?</em></td>
    </tr>
   </table>


## 현재 AI Assistant 제한 사항

AI Assistant는 강력한 툴이지만 현재 개발 단계에서는 특정 유형의 질문과 요청이 데이터를 제공할 수 없습니다. 아래 표에는 AI Assistant가 데이터를 표시할 수 없는 프롬프트의 예가 나와 있습니다.

<table>
    <tr>
        <td><b>프롬프트 유형</b></td>
        <td><b>예</b></td>
    </tr>
    <tr>
        <td>사용자 지정된 구성에 대한 질문</td>
        <td><em>Workfront 인스턴스에서 어떤 사용자 지정 통합 논리를 실행하고 있습니까?</em>
        </td>
    </tr>
    <tr>
        <td>Workfront 외부의 데이터에 대한 질문 </td>
        <td><em>오늘 Outlook 일정을 보여 줄 수 있습니까?</em></td>
    </tr>
             <tr>
        <td>통합되지 않은 Adobe 제품에 대한 질문 </td>
        <td><em>여기에서 Acrobat의 PDF을 편집하려면 어떻게 해야 합니까?</em></td>
         <tr>
        <td>사람의 판단을 필요로 하는 질문</td>
        <td><em>이 프로젝트는 보류해야 합니까?</em></td>
    </tr>
    </tr>
       <tr>
        <td>벌크 업데이트 요청</td>
        <td><em>[USER]에 대한 모든 지연 작업을 재할당합니다.</em></td>
    </tr>
       <tr>
        <td>예측 분석에 대한 요청</td>
        <td><em>이전 데이터를 기반으로 새로운 프로젝트 계획을 제안합니다.</em></td>
    </tr>
           <tr>
        <td>액세스 수준 이상의 정보 요청</td>
        <td><em>계정의 모든 청구 요금을 나열합니다.</em></td>
    </tr>
           <tr>
        <td>모호한 정보가 포함된 요청 </td>
        <td><em>내 프로젝트를 수정합니다.</em></td>
    </tr>
   </table>
