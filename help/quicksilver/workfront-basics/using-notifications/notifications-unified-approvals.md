---
content-type: reference
navigation-topic: notifications
title: '알림: 통합 승인'
description: 다음 알림은 통합 승인 경험에 대한 승인 활동에 대해 알려줍니다. 수신하는 알림을 구성하는 방법에 대한 자세한 내용은 이메일 알림 수정 을 참조하십시오.
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 7957c410d4a0e39b23b4f5a3d29a794e5deec72a
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%
---
# 알림: 통합 승인

{{highlighted-preview}}

다음 알림을 사용하여 통합 검토 및 승인을 위한 활동에 대한 최신 정보를 받아 보십시오. 받는 전자 메일 알림을 구성하는 방법에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

>[!NOTE]
>
>이러한 알림은 즉시 알림으로만 사용할 수 있으며 일별 요약에서는 사용할 수 없습니다.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th>포함된 필드</th> 
   <th>기본 상태</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>승인 완료됨 - 승인됨</strong> </p> <p>문서 승인이 승인됨의 최종 결정으로 종료됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>최종 결정: (문서)이 승인됨</em>입니다.</p> </td> 
   <td> <p>최종 결정<br>문서<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>승인 완료됨 - 변경 사항과 함께 승인됨</strong> </p> <p>문서 승인이 변경 사항과 함께 승인됨의 최종 결정으로 종료됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>최종 결정: (문서)이(가) 변경 사항과 함께 승인됨</em>입니다.</p> </td> 
   <td> <p>최종 결정<br>문서<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>승인 완료됨 - 작업 필요</strong> </p> <p>문서 승인이 필요한 작업의 최종 결정으로 종료됩니다.</p> <p>인스턴트 알림 전자 메일의 제목: <em>최종 결정: (문서)에 작업이 필요합니다</em></p> </td> 
   <td> <p>최종 결정<br>문서<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>기한이 다가옴</strong> </p> <p>귀하가 속한 문서 승인이 기한이 다가오고 있습니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>승인 기한이 (문서)</em>으로 다가오고 있습니다.</p> </td> 
   <td> <p>요청자<br>역할<br>팀<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>기한 지남</strong> </p> <p>귀하가 속한 문서 승인이 최종 결정 없이 기한을 경과합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>승인 기한이 지남(문서)</em>입니다.</p> </td> 
   <td> <p>고정 헤드라인<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함:</em><br>단계</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>검토 완료됨</strong> </p> <p>검토자는 문서 승인에 대한 검토를 완료합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 <em>(문서)입니다. </em></p> </td> 
   <td> <p>검토자<br>문서<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>비디오 승인 한도에 가까워짐(80%)</strong> </p> <p>비디오 승인은 플랜 비디오 승인 한도의 80%에 도달합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>Workfront의 연간 비디오 승인 요청 한도에 근접했습니다</em></p> </td> 
   <td> 헤드라인 및 본문<br>비디오 승인 요청(현재 사용량)<br>한도 합계(한도)<br>기타 수신자<br>"Workfront에서 보기" 단추<br>"FIO Enterprise로 업그레이드" 단추 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>비디오 승인 한도에 도달함</strong> </p> <p>비디오 승인이 플랜의 비디오 승인 한도에 도달합니다.</p> <p>즉시 알림 이메일의 제목: <em>Workfront에서 연간 비디오 승인 요청 한도에 도달했습니다</em></p> </td> 
   <td> 헤드라인 및 본문<br>비디오 승인 요청(현재 사용량)<br>한도 합계(한도)<br>기타 수신자<br>"Workfront에서 보기" 단추<br>"FIO Enterprise로 업그레이드" 단추 </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>결정 - 승인됨</strong> </p> <p>승인자는 문서 승인에 대해 승인됨으로 결정합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>(문서) 승인자(이름)</em></p> </td> 
   <td> <p>의사 결정자<br>의사 결정<br>문서 및 버전<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>결정 - 변경 사항과 함께 승인됨</strong> </p> <p>승인자는 문서 승인에 대한 변경 사항과 함께 승인됨으로 결정합니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>(문서)이(가) (이름)</em>의 변경 내용으로 승인되었습니다.</p> </td> 
   <td> <p>의사 결정자<br>의사 결정<br>문서 및 버전<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>결정 - 작업이 필요함</strong> </p> <p>승인자는 문서 승인 작업이 필요함을 결정합니다.</p> <p>인스턴트 알림 전자 메일의 제목: <em>(문서)은(는) (이름)</em>(으)로 작업해야 함</p> </td> 
   <td> <p>의사 결정자<br>의사 결정<br>문서 및 버전<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>그룹화된 승인에서 추가되거나 제거된 문서</strong> </p> <p>문서가 속해 있는 그룹화된 문서 승인에서 추가되거나 제거됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>귀하의 승인이 추가되었거나 제거된 문서</em></p> </td> 
   <td> <p><strong>추가됨:</strong><br>요청자<br>그룹 이름<br>썸네일 미리 보기<br>날짜<br>"검토로 이동" 단추<br>세부 정보 차단: 그룹 이름, 에셋 수, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>사용자 지정 메시지<br>프로젝트</p> <p><strong>제거됨:</strong><br>요청자<br>그룹 이름<br>썸네일 미리 보기(단추 또는 세부 정보 블록 없음)</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>모든 검토 완료됨</strong> </p> <p>모든 검토자는 문서 승인에 대한 검토를 완료합니다.</p> <p>즉시 알림 전자 메일의 제목은 다음과 같습니다. <em>모든 검토가 완료되었습니다(문서)</em></p> </td> 
   <td> <p>문서<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>미리 알림 - 24시간</strong> </p> <p>문서를 검토하고 승인할 시간이 24시간 남았습니다.</p> <p>즉시 알림 전자 메일의 제목은 다음과 같습니다. <em>미리 알림: (문서)에 승인이 필요합니다.</em></p> </td> 
   <td> <p>요청자<br>역할<br>팀<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>미리 알림 - 72시간</strong> </p> <p>문서를 검토하고 승인할 시간이 72시간 남았습니다.</p> <p>즉시 알림 전자 메일의 제목은 다음과 같습니다. <em>미리 알림: (문서)에 승인이 필요합니다.</em></p> </td> 
   <td> <p>요청자<br>역할<br>팀<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>승인자 또는 검토자로 추가됨</strong> </p> <p>문서 승인 시 승인자 또는 검토자로 추가되었습니다.</p> <p>즉시 알림 전자 메일의 제목은 다음과 같습니다. <em>승인이 필요합니다(문서)</em></p> </td> 
   <td> <p>요청자<br>역할<br>팀<br>승인 요청 날짜<br>기한<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>사용자 지정 메시지<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>승인자 또는 검토자로 제거됨</strong> </p> <p>문서 승인에서 승인자 또는 검토자로 제거되었습니다.</p> <p>즉시 알림 전자 메일의 제목은 다음과 같습니다. <em>승인이 더 이상 필요하지 않습니다(문서)</em></p> </td> 
   <td> <p>요청자<br>문서 및 버전<br>역할<br>팀(단추 또는 세부 정보 블록 없음)</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>사용자 지정 메시지</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>변경된 역할</strong> </p> <p>문서 승인에서 승인자 또는 검토자 역할이 변경됩니다.</p> <p>인스턴트 알림 전자 메일의 제목은 다음과 같습니다. <em>귀하의 역할(문서)이 변경되었습니다</em></p> </td> 
   <td> <p>요청자<br>문서 및 버전<br>역할 변경의 방향<br>"검토로 이동" 단추<br>세부 정보 차단: 문서 이름, 문서 세부 정보, 모든 수신자</p> <p><em>승인의 일부인 경우 포함됨:</em><br>문서 미리 보기<br>단계<br>프로젝트</p> </td> 
   <td><strong>즉시</strong> </td> 
  </tr> 
 </tbody> 
</table>
