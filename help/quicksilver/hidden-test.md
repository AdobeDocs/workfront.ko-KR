---
title: 숨겨진 테스트 파일
author: Bob
description: 검색에서 숨겨지고 왼쪽 탐색에서 숨겨짐
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: 1655726151338c47d8f81201db9ef0bb92d9ce9a
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# 숨겨진 테스트 파일 - 기능 분기 테스트

이 파일은 검색에서 숨겨집니다(`hide: yes`) 및 왼쪽 탐색(`hidefromtoc: yes`).

<span class="preview">이 파일은 **숨김** 검색(`hide: yes`) 및 왼쪽 탐색(`hidefromtoc: yes`).</span>

<p class="preview">이 파일은 **숨겨진** 검색('숨기기: yes') 및 왼쪽 탐색('hidefromtoc: 예)</p>

## 이미지 테스트

![이미지 테스트](assets/get-started.png){width="50" align="center"}

## 미리 보기 강조 표시 테스트

**구성 요소 블록에 DIV를 사용합니다.**

DIV는 아래에 시작됩니다.

<div class="preview">

DIV의 시작.

>[!NOTE]
>
>이건 메모예요
>
>메모의 배경을 강조해 달라는 요청이 있습니다.

![이미지](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

마지막으로 강조 표시된 항목.

</div>

DIV는 위에서 종료됩니다.

**단락 또는 구문에 SPAN 사용**

이것은 단락입니다. <span class="preview">저는 노란색 텍스트입니다.</span> 구문을 제대로 닫거나 페이지가 이상하게 렌더링될 수 있습니다.

DIV 및 SPAN은 HTML 테이블에서도 유용합니다.

**기타 지원되는 HTML 요소**

을 지정할 수도 있습니다 `class="preview"` 구문 `<p>`, `<td>`, `<tr>`등 미리 보기에서 테스트하는지 확인합니다.

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
   <td> <p><span class="preview">시스템 관리자 액세스</p> <p>중요 사항: 사용자에게 첨부할 수 있는 기존 시스템 관리자 계정을 사용하는 대신 Jira 및 Workfront에서 이 통합을 위해 별도의 시스템 관리자 계정을 만드는 것이 좋습니다. </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>Workfront 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 를 참조하십시오.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

품질 = 12

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

품질 = 6

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

HTML 표 내의 비디오

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">이 비디오 작동합니까?</td> 
   <td>아니오, 그렇지 않습니다 </td> 
  </tr> 
 </tbody> 
</table>

Markdown 테이블 내의 비디오

| 열 1 | 열 2 |
|---|---|
| 이게 효과가 있나요? | 아니요 |
