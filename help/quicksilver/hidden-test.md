---
title: 숨겨진 테스트 파일
author: Bob
description: 검색 및 왼쪽 탐색 메뉴에서 숨김
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: 5c47b09550c54b7ea4f8319bb42e93572e06324b
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# 숨겨진 테스트 파일 - 기능 분기 테스트

이 파일은 검색에서 숨겨집니다(`hide: yes`) 및 왼쪽 탐색(`hidefromtoc: yes`).

<span class="preview">이 파일은 **숨김** 출처: 검색(`hide: yes`) 및 왼쪽 탐색(`hidefromtoc: yes`).</span>

<p class="preview">이 파일은 검색(`hide: yes`) 및 왼쪽 탐색(`hidefromtoc: yes`)에서 **hidden**입니다.</p>

## 이미지 테스트

![이미지 테스트](assets/get-started.png){width="50" align="center"}

## 미리보기 강조 표시 테스트

**구성 요소 블록에는 DIV를 사용하십시오.**

DIV는 아래에서 시작됩니다.

<div class="preview">

DIV 시작

>[!NOTE]
>
>이것은 노트입니다.
>
>노트 배경에 대한 하이라이트 요청이 있습니다.

![이미지](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

마지막으로 강조 표시된 항목.

</div>

DIV는 위에서 끝납니다.

**단락 또는 구에 SPAN 사용**

단락입니다. <span class="preview">저는 노란색 문자입니다.</span> 구문을 제대로 닫지 않도록 하십시오. 그렇지 않으면 페이지가 이상하게 렌더링될 수 있습니다.

DIV 및 SPAN은 HTML 테이블에서도 유용합니다.

**기타 지원되는 HTML 요소**

다음을 지정할 수도 있습니다 `class="preview"` 구문 `<p>`, `<td>`, `<tr>`등. 미리 보기에서 테스트해야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr class="preview"> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront 플랜</a>*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"></td> 
   <td> <p class="preview">플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira 액세스</td> 
   <td> <p><span class="preview">시스템 관리자 액세스</p> <p>중요: 사용자에게 첨부할 수 있는 기존 계정을 사용하는 대신 Jira 및 Workfront에서 별도의 시스템 관리자 계정을 만들어 이 통합 전용을 하는 것이 좋습니다. </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>Workfront 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 를 참조하십시오.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

화질이 높은 비디오 = 12

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

품질을 가진 비디오 = 6

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

HTML 테이블 내 비디오

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">이 비디오가 작동합니까?</td> 
   <td>아니오 그렇지 않습니다 </td> 
  </tr> 
 </tbody> 
</table>

Markdown 표 내부의 비디오

| 열 1 | 열 2 |
|---|---|
| 작동합니까? | 또한 아니요 |


