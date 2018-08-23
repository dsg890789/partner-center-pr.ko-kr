---
title: 고객이 파트너에게 관리 권한을 위임하는 경우 | 파트너 센터
description: 재판매인 파트너는 고객을 관리자로 위임할 수 있으며 권한을 제거할 수도 있습니다.
author: labrenne
keywords: 위임된 관리자 권한, 대신 관리, 권한 제거
ms.openlocfilehash: 7f1bd81f40892f851e1582a7a842a64c55e4ff63
ms.sourcegitcommit: 93968695897114a68d5e948d13a36127a4079b6f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2018
ms.locfileid: "1913953"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>고객이 파트너에게 관리 권한을 위임하는 경우

**적용 대상**

-  파트너 센터

고객의 신뢰할 수 있는 조언자인 CSP 파트너는 Azure AD 테넌트 및 Office 365의 관리자로 위임될 수 있습니다. 파트너 대시보드로 초대를 보내 이러한 위임 관계를 시작할 수 있습니다. 

1. **대시보드** 메뉴에서 **고객**을 선택한 다음 **고객 관계 요청**을 선택합니다.
2. URL이 포함된 양식 이메일이 나타납니다. 해당 양식을 복사하여 고객에게 보낼 이메일에 붙여 넣을 수 있습니다. 언제든 추가 정보를 추가할 수 있지만 URL을 포함해야 합니다. 고객이 요청에 응답하기 위해 해당 URL을 사용합니다.  
3. 고객이 초대를 수락하면 귀하는 해당 서비스의 관리자가 됩니다.

고객은 Office 365 서비스 포털에서 테넌트에 대해 관리자 권한을 가진 파트너를 찾을 수 있습니다. 이렇게 하려면 다음을 수행합니다.

1. 전역 관리자 권한으로 [Office 365 관리자 포털](https://portal.office.com/adminportal)에 로그인합니다.
2. **설정** → **파트너 관계**를 선택합니다.
3. **파트너 관계** 페이지에 함께 작업하는 파트너 및 테넌트에 대해 관리 권한이 위임된 파트너의 목록이 표시됩니다.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>고객이 파트너의 위임된 관리자 권한을 관리할 수 있음 

고객은 귀하의 테넌트 관리자 권한을 제거하는 경우에도 구독 및 라이선스 갱신 목적으로 귀하와의 관계를 계속 유지할 수 있습니다. 고객은 Office 365 관리 센터의 **파트너 관계** 페이지에서 Office 365 계정에 대한 권한 및 사용 권한을 관리합니다. 이 페이지에서 고객은 다음을 수행할 수 있습니다.

- 관계를 맺고 있는 파트너 및 관리자 권한이 위임된 파트너 확인

- 파트너에게 위임된 테넌트 관리 권한 제거

파트너에게 위임된 관리 권한을 제거하려면 다음을 수행합니다.

1. **파트너 관계** 페이지에서 관심 파트너를 선택합니다.
2. 세부 정보 창에서 **위임된 관리자 제거**를 선택합니다.
3. 확인 창에서 **제거**를 선택합니다.

>**중요**<br>
Azure AD 역할 할당은 암시적입니다. Azure AD Portal/PowerShell/Graph를 사용하여 Azure AD 역할의 구성원을 나열하려고 시도하는 경우 파트너가 반환되지 않습니다. 파트너가 Azure AD 역할에 할당되었는지 확인하려면 Office 365 관리자 포털의 파트너 관계 페이지를 참조하여 위임된 관리 권한이 파트너에게 부여되었는지 여부를 확인해야 합니다.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD의 위임된 관리자 권한 

위임된 관리에 대해 사용되는 파트너의 Azure AD 테넌트에는 관리자 에이전트 및 기술 지원팀 에이전트의 두 가지 보안 그룹이 있습니다. 고객이 파트너에게 위임된 관리 권한을 부여한 경우:

- 관리자 에이전트 그룹은 고객의 Azure AD 테넌트에서 전역 관리자 역할로 할당됩니다.

- 기술 지원팀 에이전트 그룹은 고객의 Azure AD 테넌트에서 기술 지원팀 관리자 역할로 할당됩니다.

할당된 디렉토리 역할에 따라 두 그룹의 구성원은 고객을 대신하여 파트너 자격 증명 및 관리자를 사용해서 고객의 Azure AD 테넌트 및 O365 서비스에 로그인할 수 있습니다.

고객이 위임된 관리자 권한을 제거하면 Azure AD 역할 할당이 제거되고 귀하는 더 이상 고객의 Azure AD 테넌트를 관리할 수 없습니다.

### <a name="azure-subscriptions-and-resource-management"></a>Azure 구독 및 리소스 관리

각 Azure 구독에는 고유한 리소스 관리 역할 세트가 있습니다. CSP 파트너가 고객의 Azure 구독을 관리하려면 해당 파트너는 Azure 구독에 대해 하나 이상의 역할에 할당되어야 합니다. 특히 다음 사항에 주의하세요.

- 고객이 재판매인 초대를 수락하고 파트너에게 위임된 관리 권한을 부여하면 파트너는 고객 테넌트의 기존 Azure 구독에 자동으로 액세스하지 않습니다.

- CSP 파트너가 고객에게 새로운 Azure 구독을 제공하면 CSP 파트너 테넌트의 관리자 에이전트 그룹에 구독에 대한 소유자 역할이 자동으로 할당됩니다. 이 역할 할당을 기반으로 그룹 구성원은 구독에 따라 리소스에 액세스하고 이를 관리할 수 있습니다.

- 고객이 Office 365 Portal을 사용하여 파트너의 위임된 관리 권한을 제거한 경우, 파트너는 여전히 구독에 대해 하나 이상의 역할에 할당되어 있는 경우에 한해 고객의 Azure 구독을 관리할 수 있습니다. 파트너의 Azure 구독 관리를 중지하려면 고객이 해당 역할 할당을 제거해야 합니다.

## <a name="windows-autopilot"></a>Windows AutoPilot 

파트너 대시보드에서 CSP 파트너는 위임된 관리자 권한 없이도 고객의 AutoPilot 구성을 관리할 수 있습니다. [Windows Autopilot으로 디바이스 설정 간소화](https://docs.microsoft.com/partner-center/autopilot)하는 방법을 알아보세요.

직접 또는 간접 재판매인 여부에 따라 수행할 수 있는 작업이 달라질 수 있습니다.

|**작업**   |**직접 재판매인 또는 간접 재판매인**   |**간접 재판매인**   |
|-----------------|-----------------------------------| -----------------------------|
|장치 추가(csv 파일 사용)  |예      |아니요|
|장치 제거   |예   |아니요|
|프로필 추가   |예   | 예   |
|프로필 업데이트   |예    |예   |
|프로필 제거   |예   |예   |
|프로필을 장치에 적용   |예   |예   |
|장치에서 프로필 제거   |예   |예   | 

- 고객이 파트너의 위임된 관리 권한을 제거한 경우에도 CSP 파트너는 재판매인 관계에 있는 기존 고객을 위해 AutoPilot 구성을 계속 관리할 수 있습니다.

- 귀하는 본인 또는 다른 CSP 파트너가 추가한 고객을 위해 기존 장치를 관리할 수 있습니다.

- 고객이 비즈니스용 Microsoft Store 또는 Microsoft Intune Portal을 통해 업로드한 장치는 관리할 수 없습니다.

>**중요** Microsoft 파트너 센터의 현재 AutoPilot 관리 환경은 최종적인 것이 아니며 향후 변경될 수 있습니다. 이 문서의 결합 시점을 기준으로 다음 변경 사항이 고려됩니다.

  - 파트너가 프로필을 추가/업데이트/제거하고 고객 테넌트의 모든 장치에서 프로필을 적용/제거하려면 파트너가 위임된 관리 권한을 고객에게 부여 받아야 합니다.

- 파트너가 고객 테넌트에서 다른 파트너 또는 고객이 업로드한 장치를 제거하려면 위임된 관리 권한을 고객에게 부여 받아야 합니다. 그렇지 않으면 파트너는 이전에 동일한 파트너가 추가한 장치만 제거할 수 있습니다.