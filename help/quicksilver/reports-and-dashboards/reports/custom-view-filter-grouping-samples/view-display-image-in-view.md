---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 열에 문자열 대신 이미지 표시'
description: 뷰에 있는 개체의 이름을 텍스트 모드를 사용하여 이미지로 바꿀 수 있습니다. 이미지를 대체하는 객체를 열 수 있는 이미지에 대한 링크를 추가할 수도 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# 보기: 열에 문자열 대신 이미지 표시

뷰에 있는 개체의 이름을 텍스트 모드를 사용하여 이미지로 바꿀 수 있습니다. 이미지를 대체하는 객체를 열 수 있는 이미지에 대한 링크를 추가할 수도 있습니다.

>[!NOTE]
>
>이미지는 실제 해상도에 표시되므로 작은 이미지를 사용해 보십시오.

![](assets/replace-project-name-with-image-and-link-350x125.png)

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 예: 프로젝트 보기의 프로젝트 이름을 이미지로 바꿉니다.

1. Adobe Workfront 외부의 웹 사이트 또는 서버에 이미지를 업로드합니다. 웹 브라우저를 사용하여 이미지에 액세스할 수 있어야 합니다.

   >[!TIP]
   >
   >* 모든 브라우저 유형은 다르지만 모든 브라우저 유형은 URL을 표시할 수 있습니다.
   >* Workfront에 업로드된 이미지를 사용하지 마십시오. Workfront에 저장된 이미지를 공개적으로 사용할 수 없고 일정 시간 후 만료되는 액세스 키를 가지고 있으므로 이러한 이미지는 시간이 지남에 따라 보기에서 표시되지 않습니다.
   >* 컴퓨터에 저장된 이미지에 고유한 URL이 없습니다. 이미지 호스팅을 제공하는 사이트를 찾고 이미지를 호스팅하십시오. 조직에 이미 이러한 사이트가 있을 수 있습니다.


1. 웹 브라우저를 사용하여 저장한 이미지로 이동합니다.
1. 다음을 수행하여 이미지의 URL을 얻습니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. 마우스 오른쪽 단추를 클릭하고 을 선택합니다 **이미지 위치 복사**, 또는 **링크 가져오기**&#x200B;브라우저에 따라 다릅니다. 이제 해당 특정 이미지에 대한 URL이 있으며 클립보드에서 붙여넣을 수 있습니다.
   1. 해당 링크가 있는 모든 사람이 링크로 이동하여 이미지를 볼 수 있는 권한이 있고, 해당 링크에 액세스하기 위해 로그인하지 않아도 되는지 확인하십시오.

1. 프로젝트로 이동하여 **자세히** 메뉴 ![](assets/more-icon-45x33.png) 프로젝트 이름 옆에 있는 를 클릭하고 **편집**.

1. 에서 **URL** 필드에서 이미지에 링크를 추가합니다.
1. 목록 또는 보고서의 프로젝트 보기로 이동하고 보기를 사용자 지정합니다.
1. 에 대한 열 헤더를 클릭합니다. **프로젝트 이름**&#x200B;를 클릭한 다음 **텍스트 모드로 전환**.

1. 기존 코드에 열에 다음 코드를 추가합니다.

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   선택한 이미지는 프로젝트 보기에서 프로젝트 이름을 대체하며 이미지는 프로젝트에 대한 링크입니다.

1. 클릭 **보기 저장**.
