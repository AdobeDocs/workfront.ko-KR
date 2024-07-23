---
title: 2024년 4분기 릴리스 개요
description: 이 페이지에서는 2024년 4분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 분기 내내 프로덕션 환경에서 사용할 수 있도록 계획되어 있습니다.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 76b44f3d5ff7d7747da801a051a457157e08ea4a
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# 2024년 4분기 릴리스 개요

이 페이지에서는 2024년 4분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 분기 내내 프로덕션 환경에서 사용할 수 있도록 계획되어 있습니다.

<span class="preview">주기 외 기능(2024년 4분기 릴리스 날짜 이전에 프로덕션에 릴리스된 기능)은 노란색으로 강조 표시됩니다.</span>

>[!IMPORTANT]
>
>23.3 릴리스에는 조직을 월별 릴리스로 이동하는 옵션이 포함되었습니다. 따라서 Workfront은 월별 및 분기별 릴리스 트랙을 모두 고려하여 릴리스의 번호 지정 체계를 변경했습니다. 첫 번째 숫자는 연도를 지정하고 두 번째 숫자는 릴리스된 월을 나타냅니다. 예: 2024년 4월 릴리스는 24.4로 표시됩니다.
>
>월별 및 분기별 릴리스는 달리 지정하지 않는 한 해당 월의 두 번째 전체 주 목요일에 사용할 수 있습니다.
>
>| 월별 릴리스 | 분기별 릴리스 |
>|----|----|
>| <ul><li>24.8 (2024년 8월)</li><li>24.9 (2024년 9월)</li><li>24.10 (2024년 10월)</li></ul> | <ul><li>24.10 (2024년 10월)</li></ul> |
>
>각 분기의 최종 릴리스(이번 분기 24.10)의 경우 빠른 릴리스 일정을 사용하는 사용자는 하루 일찍 릴리스를 받게 됩니다.
>
>빠른 릴리스 프로세스에 대한 자세한 내용은 [빠른 릴리스 프로세스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하십시오.

## Adobe Workfront 개선 사항

<!--* [Project enhancements](#project-enhancements)-->
* [기타 개선 사항](#other-enhancements)

<!--
### Project enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Edit the task and issue Commit Date and Condition from the header or Details section</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>To make it easier for you to update tasks and issues, we have now added the Commit Date and Condition fields as options to add to task and issue headers and Details section in a layout template. Users are now able to update these fields from the header or Details section of a page, when they are assigned to the modified layout template.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: May 30, 2024</p>
                            </li>
                            <li>
                                <p>Production for fast release: With the 24.6 release (June 13, 2024)</p>
                            </li>
                            <li>
                                <p>Production release for all customers: With the 24.7 release (July 18, 2024)</p>
                            </li>
                        </ul>
                        <p><span class="preview">This feature has been temporarily removed from Production for customers that are not on the fast release schedule.</span></p>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">More relevant assignments added to the New Task workflow</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>We have added the same functionality for more relevant smart assignments to the Assignments field in the New Task box when adding a task to a project and in a project task list.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: February 13, 2024</p>
                            </li>
                            <li>
                                <p>Production for fast release: With the 24.5 release (May 16, 2024)</p>
                            </li>
                            <li>
                                <p>Production release for all customers: With the 24.7 release (July 18, 2024)</p>
                            </li>
                        </ul>
                        <p><span class="preview">This feature has been temporarily removed from Production for customers that are not on the fast release schedule.</span></
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">More relevant smart assignments</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>We have changed the algorithm that Workfront uses to calculate and suggest smart assignments for tasks. The new algorithm applies in the following areas in Workfront where you assign a task: task lists, the Assignments area in the task header, Home, and the Summary panel.</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: December 21, 2023</p>
                            </li>
                            <li>
                                <p>Production for fast release: With the 24.5 release (May 16, 2024)</p>
                            </li>
                            <li>
                                <p>Production release for all customers: With the 24.7 release (July 18, 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>
-->

### 기타 개선 사항

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2024년 4분기 동안의 룩앤필 업데이트</a></p>
                        <p>2024년 4분기 내에 Adobe Workfront 애플리케이션의 다양한 영역의 모양과 느낌에 대한 작은 업데이트가 이루어지고 있습니다. 특정 릴리스 날짜는 개별 릴리스 정보를 검토하십시오.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2024년 4분기 릴리스 일정 전체</p>
                            </li>
                            <li>
                                <p><span class="preview">프로덕션 릴리스: 특정 날짜에 대한 릴리스 정보 검토</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## 공지

### Workfront Fusion 개선 사항

Workfront Fusion의 새로운 기능은 2024년 4분기 릴리스 일정 이외의 케이던스로 프로덕션에서 사용할 수 있습니다. 최신 기능에 대한 자세한 내용은 [Adobe Workfront Fusion 릴리스 활동](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)을 참조하십시오.

### Workfront Scenario Planner 개선 사항

릴리스의 현재 시점에는 시나리오 플래너 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### Workfront Proof 개선 사항

릴리스의 현재 시점에는 Workfront Proof 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### Workfront 목표 개선 사항

릴리스의 현재 시점에는 Workfront 목표 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### API 버전 18

API 버전 18의 경우 일부 리소스 및 끝점을 수정했습니다. 일부 변경 사항은 새로운 기능을 지원하며, 다른 변경 사항을 통해 API를 통해 사용 가능한 정보를 보다 쉽게 사용할 수 있습니다.

새로운 기능 및 업데이트 내용은 [API 버전 18의 새로운 기능](/help/quicksilver/wf-api/api/new-api-version-18.md)을 참조하세요.

API 버전에 대한 자세한 내용은 [API 버전 관리 및 지원 일정](/help/quicksilver/wf-api/api/api-version-support-schedule.md)을 참조하십시오.

### Workfront 유지 보수 업데이트

2024년 4분기 릴리스 중 유지 관리 업데이트에 대한 자세한 내용은 [Workfront 유지 관리 업데이트](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)를 참조하십시오.

### 교육 업데이트

각 Adobe Workfront 제품 릴리스의 학습 프로그램, 학습 경로, 비디오 및 안내서에 대한 최신 업데이트를 살펴보십시오. 자세한 내용은 [Workfront Tutorials 페이지](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)의 &quot;새로운 기능&quot; 섹션을 참조하십시오.
