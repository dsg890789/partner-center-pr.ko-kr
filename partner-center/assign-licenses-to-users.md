---
title: 고객 계정에 대한 사용자 관리 작업 | 파트너 센터
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객에 대 한 사용자 계정을 만들고, 사용자 라이선스를 추가 또는 제거 하 고, 사용자 암호를 다시 설정 하거나, 사용자 계정을 삭제 하거나, 복원 하는 방법에 대해 알아봅니다.
ms.assetid: 41B06576-8DDD-435D-BABB-697D4AD30213
author: MaggiePucciEvans
ms.author: evansma
Keywords: 고객 관리, 계정, 계정 만들기, 라이선스, 라이선스 할당, 사용자 관리, 암호, 암호 재설정, 암호 변경
ms.localizationpriority: medium
ms.openlocfilehash: cd1b32a0ceb133f9513263f56a7d1e2e98dde3c5
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721362"
---
# <a name="user-management-tasks-for-customer-accounts"></a>고객 계정에 대한 사용자 관리 작업

**적용 대상**

- 파트너 센터

**적절한 역할**

- 전역 관리자
- 사용자 관리 관리자
- 관리자 에이전트
- 영업 에이전트
- 기술 지원팀 에이전트

고객의 계정에서 새 사용자를 만들고 삭제할 수 있습니다. 삭제 후 30 일 이내에 이전에 삭제 한 사용자 계정을 하나 이상 복원할 수도 있습니다. 사용자의 이전 구독 할당도 복원됩니다(이전 할당을 사용할 수 있다고 가정).

고객에 대 한 새 구독을 구입 하는 경우 고객은 계정, 해당 사용자 권한 및 각 사용자가 요구 하는 서비스를 필요로 하는 모든 사용자의 목록을 제공 해야 합니다.  

[Excel 호환 .csv 스프레드시트 파일](adding-multiple-users-to-a-customer-account.md)을 사용하여 한 번에 [여러 사용자에게 구독을 할당](bulk-license-provisioning-for-multiple-users.md)할 수 있습니다.

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>고객용 사용자 계정 생성

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. 고객 메뉴에서 **사용자 및 라이선스**를 선택합니다.

4. 각 사용자에 대해 **사용자 추가**를 선택한 다음 권한과 라이선스 등의 정보를 작성합니다. 변경 사항을 **저장**합니다.

5. 사용자 이름 및 사용자에게 보낼 임시 암호를 기록해야 합니다.

6. 한 번에 하나씩 여러 사용자를 추가하는 경우 **다른 사용자 추가**를 사용합니다.

7. [Excel 호환 .csv 스프레드시트 파일을 가져와서](adding-multiple-users-to-a-customer-account.md) 한 번에 여러 사용자를 추가할 수도 있습니다. 다른 사용자 추가를 사용하거나 Excel과 호환되는 .csv 스프레드시트 파일로 가져와 한 번에 다수의 사용자를 추가하는 경우 전체 집합을 완료할 때까지 기다려야 확인 화면에서 이러한 이름과 암호를 메일로 보내거나 인쇄할 수 있습니다.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>고객용 사용자 라이선스 추가 또는 제거

다음 단계는 Microsoft 제품에 대 한 사용자 라이선스를 추가 하거나 제거 하는 경우에 적용 됩니다. 상업적 marketplace에서 라이선스 기반 SaaS 구독의 사용자 라이선스를 추가 하거나 제거 하려면 [SaaS 구독에 대 한 라이선스 추가 또는 제거](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)를 참조 하세요.

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. 고객 메뉴에서 **사용자 및 라이선스**를 선택합니다.

4. 목록에서 한 명 이상의 사용자를 선택합니다. 예를 들어 고객이 새 라이선스를 방금 구매한 후 아직 라이선스가 없는 사람에게 할당하려고 하는 경우 **사용자 필터링 기준...** 옵션을 사용하여 알맞은 그룹을 찾을 수 있습니다.

5. **라이선스 관리**를 선택합니다. 필요한 사항을 변경한 다음 **저장**을 선택합니다.

> [!NOTE]
> 제품을 게시 한 ISV (독립 소프트웨어 공급 업체)를 통해 라이선스 할당 및 활성화를 관리 하는 [Azure Marketplace 제품](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)입니다.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>고객용 사용자 암호 재설정

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3.  고객 메뉴에서 **사용자 및 라이선스**를 선택합니다. 목록에서 사용자를 선택합니다.

4.  화면 맨 아래에서 **암호 재설정**을 선택합니다. 

5.  사용자에게 새 임시 암호를 보냅니다.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>고객용 사용자 계정 삭제

1.  **파트너 센터** 메뉴에서 **고객**을 선택 합니다. 목록에서 고객을 선택합니다.

2.  고객 메뉴에서 **사용자 및 라이선스**를 선택합니다. 목록에서 사용자를 선택합니다.

3.  화면 맨 아래에서 **사용자 계정 삭제**를 선택합니다.

이 계정을 30일 이내에 복원해야 할 경우 고객 **사용자 및 라이선스** 목록의 **삭제된 사용자** 탭에서 이 계정을 찾을 수 있습니다. 삭제된 사용자는 30일 이내에 복원할 수 있습니다.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>삭제된 사용자 계정 복원

1.  **파트너 센터** 메뉴에서 **고객**을 선택한 다음 목록에서 고객을 선택 합니다.

2.  **사용자 및 라이선스**를 선택합니다.

3.  **삭제된 사용자( )** 탭을 선택합니다. 복원할 수 있는 삭제된 사용자가 있는 경우 **(1)** 이상이 표시됩니다.

4.  하나 이상의 삭제된 사용자의 확인란을 선택한 다음 **복원**을 선택합니다.

    선택한 모든 사용자 계정이 **사용자 및 라이선스** 페이지에 다시 나타납니다.

## <a name="related-topics"></a>관련 항목


[여러 사용자에게 라이선스 할당 또는 해지](bulk-license-provisioning-for-multiple-users.md)

[고객 계정에 대 한 여러 사용자 만들기](adding-multiple-users-to-a-customer-account.md)