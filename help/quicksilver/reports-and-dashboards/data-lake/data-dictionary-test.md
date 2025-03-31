---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Snowflake용 Reader 계정 만들기
description: Data Connect 데이터에 액세스하려면 먼저 Snowflake 리더 계정을 만들어야 합니다.
author: Courtney
feature: Reports and Dashboards
hide: true
hidefromtoc: true
source-git-commit: a42c13804b0463af27bac6f9166bc6e3c41d3fda
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 8%

---


# 테스트

## 액세스 수준

<table>
  <thead>
    <tr>
        <th>Workfront 엔티티 이름</th>
        <th>인터페이스 참조</th>
        <th>API 참조 | 레이블</th>
        <th>데이터 레이크 보기</th>
    </tr>
  </thead>
 <tr>
        <td>액세스 수준</td>
         <td>액세스 수준</td>
        <td>ACSLVL | 액세스 수준</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong>관계 필드</strong> <br>
         ACCESSLEVELID(자체): 자체<br>
         APPGLOBALID: 관계가 아닙니다. 내부 응용 프로그램 용도로 사용됨<br>
         LASTUPDATEDBYID: USER_CURRENT | 사용자 ID<br>
         LEGACYACCESSLEVELID: 관계가 아닙니다. 내부 응용 프로그램 용도로 사용됨<br>
         OBJID: OBJCODE 필드 <br>에서 식별된 개체의 ID입니다.
         SYSID: 관계가 아님, 내부 응용 프로그램 용도로 사용됨</td>
    </tr>
</table>

## 액세스 수준

<table>
  <thead>
    <tr>
        <th>Workfront 엔티티 이름</th>
        <th>인터페이스 참조</th>
        <th>API 참조 | 레이블</th>
        <th>데이터 레이크 보기</th>
    </tr>
  </thead>
 <tr>
        <td>액세스 수준</td>
         <td>액세스 수준</td>
        <td>ACSLVL | 액세스 수준</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong>관계 필드</strong> <br>
         <ul>
            <li>ACCESSLEVELID(자체): 자체</li>
            <li>APPGLOBALID: 관계가 아님, 내부 애플리케이션 목적으로 사용됨</li>
            <li>LASTUPDATEDBYID: USER_CURRENT | 사용자 ID</li>
            <li>LEGACYACCESSLEVELID: 관계가 아닙니다. 내부 응용 프로그램 용도로 사용됩니다.</li>
            <li>OBJID: OBJCODE 필드에서 식별된 개체의 ID입니다</li>
            <li>SYSID: 관계가 아님, 내부 응용 프로그램 용도로 사용됨</li>
        </ul>
    </tr>
</table>