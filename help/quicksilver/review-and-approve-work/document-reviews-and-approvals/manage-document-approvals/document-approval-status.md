---
product-area: documents
navigation-topic: approvals
title: 문서 의사 결정 상태 개요
description: 문서 결정 상태가 나열되고 설명됨
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 30a10ed9-ae11-4ff1-a66c-58ea94fe9959
source-git-commit: fcdb935b148ed7f8b9c49476f099f8285e02b0b5
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 5%

---

# 문서 의사 결정 상태 개요

문서 목록에서 직접 문서 상태를 볼 수 있습니다.

문서 목록의 ![상태](assets/status-in-doc-list.png)


다음 상태를 사용할 수 있습니다.

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        검토 보류 중</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                검토자와 승인자에게 알림이 전송되었지만 아직 에셋을 열지 않았습니다.
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        검토 중</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>적어도 한 명의 검토자가 자산을 열람했습니다.</p>
                            </li>
                            <li>
                                <p>적어도 한 명의 검토자가 검토를 완료하지 않았습니다.</p>
                            </li>
                            <li>
                                <p>이 자산에 할당된 승인자가 없습니다.</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        검토됨</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>모든 검토자가 검토를 완료했습니다</p>
                            </li>
                            <li>
                                <p>이 자산에 할당된 승인자가 없습니다.</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>작업 필요</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>모든 승인 및 검토가 완료되었습니다.</p>
                            </li>
                            <li>
                                <p>최소 한 명의 승인자가 "작업 필요"에 대한 결정을 내렸습니다.</p>
                                <p>다른 승인자는 "변경 사항과 함께 승인됨" 또는 "승인됨"을 결정할 수 있습니다.
                            </li>
                        </ul>
                    </td>
                </tr>
                  <tr>
                    <td>변경 사항과 함께 승인됨</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>모든 승인 및 검토가 완료되었습니다.</p>
                            </li>
                            <li>
                                <p>최소 한 명의 승인자가 "변경 사항과 함께 승인됨"을 결정했습니다.</p>
                                <p>다른 승인자가 "승인됨"에 대한 결정을 내렸을 수 있습니다.
                            </li>
                            <p>참고: 검토 및 승인을 위해 Frame.io 통합을 사용하는 경우에는 이 옵션을 사용할 수 없습니다.</p>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>승인됨</p>
                    </td>
                    <td>
                        <ul>
                           <!--<li>
                                <p>All approvals and reviews are complete</p>
                            </li>-->
                            <li>
                                <p>모든 승인자가 "승인됨"에 대한 결정을 내렸을 수 있습니다.
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>



<!--



<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        Pending review</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                Reviewers and approvers have been notified, but have not yet opened the asset.
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        In review</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>At least one reviewer or approver has viewed the asset</p>
                            </li>
                            <li>
                                <p>At least one reviewer has not completed their review</p><p>Or</p>
                                <p>At least one approver has not made an approval decision</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        Reviewed</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                All reviews are complete
                            </li>
                            <li>
                                There are no approvers
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Needs work</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>At least one approver has made a decision of "Needs work"</p>
                                <p>Other approvers may have given decisions of "Approved with changes" or "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
                  <tr>
                    <td>Approved with changes</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>At least one approver has made a decision of "Approved with changes"</p>
                                <p>Other approvers may have given decisions of "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Approved</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>All approvers may have given decisions of "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>


-->
