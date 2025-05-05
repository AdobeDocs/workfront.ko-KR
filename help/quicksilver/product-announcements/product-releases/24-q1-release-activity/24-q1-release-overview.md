---
title: 2024년 1분기 릴리스 개요
description: 2024년 1분기 릴리스 개요
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 2ad9e170-9e63-472a-8476-13f81b7abff3
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 0%

---

# 2024년 1분기 릴리스 개요

이 페이지에서는 2024년 1분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 2024년 1월 18일과 19일에 24.1 릴리스를 통해 모든 고객을 위한 프로덕션 환경에서 사용할 수 있도록 계획되었습니다.

24.1 릴리스 웨비나는 2024년 1월 11일에 있었습니다. [웨비나에 등록하여 여기에서 주문형 녹화를 볼 수 있습니다](https://webinars.on24.com/adobe_workfront/whatsnewin241?partnerref=releaseoverview).

<span class="preview">주기 외 기능(2024년 1분기 릴리스 날짜 이전에 프로덕션에 릴리스된 기능)은 노란색으로 강조 표시됩니다.</span>

>[!IMPORTANT]
>
>23.3 릴리스에는 조직을 월별 릴리스로 이동하는 옵션이 포함되었습니다. 따라서 Workfront은 월별 및 분기별 릴리스 트랙을 모두 고려하여 릴리스의 번호 지정 체계를 변경했습니다.
>
>월별 및 분기별 릴리스는 달리 지정하지 않는 한 해당 월의 두 번째 전체 주 목요일에 사용할 수 있습니다.
>
>| 월별 릴리스 | 분기별 릴리스 |
>|----|----|
>| <ul><li>릴리스 없음(2024년 11월)</li><li>릴리스 없음(2024년 12월)</li><li>24.1 (2024년 1월)</li></ul> | <ul><li>24.1 (2024년 1월)</li></ul> |
>| <ul><li>24.2 (2024년 2월)</li><li>24.3 (2024년 3월)</li><li>24.4 (2024년 4월)</li></ul> | <ul><li>24.4 (2024년 4월)</li></ul> |
>
>빠른 릴리스 프로세스에 대한 자세한 내용은 [빠른 릴리스 프로세스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하십시오.


## Adobe Workfront 개선 사항

* [관리자 개선 사항](#administrator-enhancements)
* [보드 개선 사항](#boards-enhancements)
* [문서 관리 개선 사항](#document-management-enhancements)
* [홈 개선 사항](#home-enhancements)
* [통합 개선 사항](#integration-enhancements)
* [프로젝트 개선 사항](#project-enhancements)
* [스트림 및 알림 개선 사항 업데이트](#update-stream-and-notification-enhancements)

### 관리자 개선 사항

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">기능</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">릴리스 날짜</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">이전 12개월 동안 증명/문서 결정을 사용할 수 있음</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>이제 새 라이선스 유형과 기존 라이선스 유형 모두에 대한 사용자 결정 보고서에 이전 12개월뿐만 아니라 현재 월의 결정 수가 표시됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 12월 14일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### 보드 개선 사항

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">기능</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">릴리스 날짜</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">보드를 만들 때 다이내믹 보드는 완료된 카드를 보관합니다</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>동적 보드를 만들 때 보드에 완료된 작업 및 문제를 포함할 수 있는 선택 사항이 있습니다. 완료된 작업 및 문제가 많은 프로젝트의 경우 동적 보드에 성능 문제가 있을 수 있습니다. 이제 동적 보드를 만들고 완료된 작업을 포함하도록 선택하면 작업 및 문제가 보드로 보관됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 12월 21일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션: 2023년 12월 21일</span></p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### 문서 관리 개선 사항

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">기능</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">릴리스 날짜</span>
                        </p>
                    </td>
                 </tr>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">문서 승인에 대해 업데이트된 상태</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>문서 승인 상태를 보다 명확하게 하기 위해 사용 가능한 문서 상태 승인을 업데이트했습니다. 이제 승인 상태는 검토자만 있고 승인자는 없는 경우뿐만 아니라 검토 완료를 표시하는 검토자를 설명합니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 12월 7일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">이 기능은 단계별 릴리스의 일부이며 현재 특정 고객에게만 제공됩니다.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">검토를 완료로 표시</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>문서를 검토하고 다음 승인 단계를 위한 준비가 되면 보다 명확하게 하기 위해 <strong>내 검토 완료</strong> 단추를 새로 만들었습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 11월 16일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">이 기능은 단계별 릴리스의 일부이며 현재 특정 고객에게만 제공됩니다.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">문서 검토 및 승인 상태가 문서 헤더에 표시됨</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>검토 및 승인 프로세스를 보다 투명하게 하기 위해 상태를 문서 세부 정보 페이지의 헤더에 추가했습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 11월 9일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">이 기능은 단계별 릴리스의 일부이며 현재 특정 고객에게만 제공됩니다.</span></p>
                    </td>
                </tr>                
           </tbody>
</table>

### 홈 개선 사항

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">기능</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">릴리스 날짜</span>
                        </p>
                    </td>
                 </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">새로운 보류 중인 승인 위젯을 사용할 수 있음</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>소유한 프로젝트에 대한 승인 및 검토의 상태를 더 쉽게 확인할 수 있도록 새로운 승인 보류 중 위젯을 홈에 추가했습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 1월 3일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">이 기능은 단계별 릴리스의 일부이며 현재 특정 고객에게만 제공됩니다.</span></p>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">레이아웃 템플릿을 사용하는 새 홈에 대한 관리자 컨트롤</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>이제 관리자는 레이아웃 템플릿을 사용하여 사용자를 위해 새 홈을 사용자 정의할 수 있습니다. 사용자 지정 옵션에는 필수 위젯과 해당 위치 선택, 배경 선택 및 사용 가능한 필터 및 그룹 선택(및 기본값 설정)을 위한 위젯별 옵션이 포함됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 12월 21일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">내 작업 빠른 작업 단추가 마우스오버에만 표시되도록 변경됨</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>성능 향상을 위해 이제 내 작업 위젯에서 사용할 수 있는 빠른 작업 버튼이 작업 항목을 마우스로 가리킬 때만 표시됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 11월 29일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션: 2023년 11월 29일</span></p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### 통합 개선 사항

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">기능</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">릴리스 날짜</span>
                        </p>
                    </td>
                 </tr>
                <tr>
                    <td>
                        이제 <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Experience Manager Assets Essentials의 메타데이터 매핑에서 <code>dc:subject</code></a> 대신 <code>xcm:keywords</code>을(를) 사용합니다.</p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>Experience Manager Assets as a Cloud Service 통합의 경험에 맞게 Experience Manager Assets Essentials 통합을 업데이트했습니다. 이제 여러 한 줄 텍스트 필드를 Experience Manager Assets의 단일 필드에 매핑할 때 두 서비스 모두 <code>xcm:keywords</code> 필드를 사용합니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 1월 10일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 2023년 1월 10일</p>
                            </li>
                            <li>
                                <p>분기 릴리스 프로덕션: 2023년 1월 10일</p>
                            </li>
                        </ul>
                    </td>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">이제 Adobe Experience Manager 통합에서 자동 완성 필드를 사용할 수 있습니다</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>Workfront과 Adobe Experience Manager 간에 필드를 더 쉽게 연결할 수 있도록 메타데이터 매핑에서 자동 완성 필드에 대한 지원이 추가되었습니다. 이제 자동 완성 필드를 Adobe Experience Manager의 해당 필드에 매핑할 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 11월 16일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션: 2023년 11월 29일</span></p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager에서 에셋 자동 게시</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>Adobe Experience Manager 통합에 다른 워크플로우를 추가했습니다. 이제 Adobe Experience Manager으로 전송할 때 자산을 자동으로 게시하도록 설정할 수 있습니다. Adobe Experience Manager 게시 서비스 또는 Adobe Experience Manager Brand Portal에 게시하도록 통합을 구성할 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 11월 9일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션: 2023년 11월 9일</span></p>
                            </li>
                        </ul>
                    </td>
                    </tr>
           </tbody>
        </table>


### 프로젝트 개선 사항

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">기능</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">릴리스 날짜</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-project-enhancements.md" class="MCXref xref" xrefformat="{para}">더 적절한 스마트 할당</a></p>
                        [!BADGE In Production for Fast Release &#x200B;]{type=Positive}<p>Workfront이 작업에 대한 스마트 할당을 계산하고 제안하는 데 사용하는 알고리즘을 변경했습니다. 새 알고리즘은 작업을 지정하는 Workfront의 작업 목록, 작업 헤더의 지정 영역, 홈 및 요약 패널에서 적용됩니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 12월 21일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.3 릴리스 포함(2024년 3월)</p>
                            </li>
                        </ul>
                    <p><i>이 기능은 미리보기 및 빠른 릴리스 프로덕션에서 제거되었습니다.</i></p>
                    </td>
                </tr>
           </tbody>
        </table>

### 스트림 및 알림 개선 사항 업데이트

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">기능</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">릴리스 날짜</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">업데이트 섹션의 댓글에 이미지를 끌어다 놓기</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>이제 댓글의 내용을 개선하기 위해 오브젝트의 업데이트 섹션에서 댓글 또는 답글에 이미지를 빠르게 끌어서 놓을 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 12월 14일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                    </td>
                    </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">새로운 댓글 달기 환경에서 프로젝트, 작업, 문제 및 문서에 대한 모든 정보를 캡처합니다</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>Workfront 인스턴스가 시작된 이후 프로젝트, 작업, 문제 및 문서는 새 댓글 달기 경험 영역에 모든 업데이트를 표시합니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 11월 28일</p>
                            </li>
                            <li>
                                <p><span class="preview">모든 고객을 위한 프로덕션: 2023년 11월 28일</span></p>
                            </li>
                        </ul>
                    </td>
                    </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">업데이트 섹션에서 댓글 또는 사용자 검색</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>이제 오브젝트의 업데이트 섹션에서 정보를 빠르게 찾기 위해 댓글에서 키워드나 댓글과 연관된 사용자를 검색할 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 11월 16일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                    </td>
                    </tr>
                    <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">업데이트 섹션의 댓글에 이미지를 복사하여 붙여 넣기</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>이제 메시지 내용에 대한 컨텍스트를 제공하기 위해 컴퓨터에서 이미지를 복사하고 새 업데이트 또는 회신에 붙여넣어 이미지에 이미지를 주석에 빠르게 첨부할 수 있습니다.</p>
                    </td>
                    <td><p><b>다음 날짜에 사용 가능:</b></p>
                        <ul>
                            <li>
                                <p>미리보기 릴리스: 2023년 11월 16일</p>
                            </li>
                            <li>
                                <p>빠른 릴리스를 위한 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                            <li>
                                <p>분기별 릴리스 프로덕션: 24.1 릴리스 포함</p>
                            </li>
                        </ul>
                    </td>
                    </tr>
           </tbody>
</table>

## 공지

### Workfront Fusion 개선 사항

Workfront Fusion의 새로운 기능은 2023년 1분기 릴리스 일정 이외의 케이던스로 프로덕션에서 사용할 수 있습니다. 최신 기능에 대한 자세한 내용은 [Adobe Workfront Fusion 릴리스 활동](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)을 참조하십시오.

### Workfront Scenario Planner 개선 사항

릴리스의 현재 시점에는 시나리오 플래너 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### Workfront Proof 개선 사항

릴리스의 현재 시점에는 Workfront Proof 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### Workfront 목표 개선 사항

릴리스의 현재 시점에는 Workfront 목표 업데이트가 없습니다. 업데이트를 사용할 수 있으면 이 영역이 업데이트됩니다.

### API 버전 17

API 버전 17의 경우 일부 리소스 및 끝점을 수정했습니다. 일부 변경 사항은 새로운 기능을 지원하며, 다른 변경 사항을 통해 API를 통해 사용 가능한 정보를 보다 쉽게 사용할 수 있습니다.

새로운 기능 및 업데이트 내용은 [API 버전 17의 새로운 기능](/help/quicksilver/wf-api/api/new-api-version-17.md)을 참조하세요.

API 버전에 대한 자세한 내용은 [API 버전 관리 및 지원 일정](/help/quicksilver/wf-api/api/api-version-support-schedule.md)을 참조하십시오.

### Workfront 유지 관리 업데이트

2024년 1분기 릴리스 동안 이루어진 유지 관리 업데이트에 대한 자세한 내용은 [Workfront 유지 관리 업데이트](https://experienceleague.adobe.com/ko/docs/workfront-known-issues/releases/current-updates)를 참조하십시오.

### 교육 업데이트

각 Adobe Workfront 제품 릴리스의 학습 프로그램, 학습 경로, 비디오 및 안내서에 대한 최신 업데이트를 살펴보십시오. 자세한 내용은 [Workfront 자습서 페이지](https://experienceleague.adobe.com/ko/docs/workfront-learn/tutorials-workfront/home)의 &quot;새로운 기능&quot; 섹션을 참조하십시오.
