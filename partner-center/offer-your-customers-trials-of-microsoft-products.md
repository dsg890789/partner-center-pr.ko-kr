---
title: 고객에게 Microsoft 제품 평가판 제공 | 파트너 센터
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객은 30일 동안 Microsoft 구독 제품을 시험 사용할 수 있습니다. 다른 많은 온라인 서비스 마찬가지로 카탈로그에서 이러한 평가판에 등록 합니다.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: a0f511ad2275866552e9646cf433351ae4fc3be3
ms.sourcegitcommit: a80838c0e79f66c28b958165e910871dd37d39f0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/18/2019
ms.locfileid: "75185543"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>고객에게 Microsoft 제품의 평가판 제공

**적용 대상**

- 파트너 센터

**적절한 역할**
-   전역 관리자 
-   사용자 관리자
-   영업 에이전트

고객에게 Microsoft 신제품을 소개하는 좋은 방법은 30일 무료 평가판을 제공하는 것입니다. 여러 다른 온라인 서비스와 마찬가지로 카탈로그에서 평가판을 등록할 수 있습니다. 모든 파트너가 참여할 수 있습니다.

## <a name="available-trial-offers"></a>사용 가능한 평가판 제안

**고객** 페이지에서 모든 미해결 평가판 제안을 찾을 수 있습니다. 이 페이지에는 무료 평가판 및 유료 구독을 비롯 한 모든 구독이 나열 됩니다. (이 기능은 현재 중국에서 사용할 수 없습니다.)

각 고객은 사용 가능한 각 제품에 대해 하나의 무료 평가판을 받을 수 있습니다. 예를 들어 고객은 Office 365 Business Premium 및 Office 365 E3의 평가판을 각각 한 번씩 받을 수 있습니다. 그러나 고객이 제품을 이미 소유 하 고 있는 경우 해당 제품에 대 한 무료 평가판을 사용할 수 없습니다.

### <a name="available-products"></a>사용 가능한 제품

평가판은 다음 제품에 제공됩니다.

- Office 365 Business Premium
- Office 365 E3
- PSTN과 Office 365 E5
- PSTN이 없는 Office 365 E5
- Enterprise Mobility 및 Security E5
- Dynamics 365 고객 참여 계획 1
- Dynamics 365 Business Central
- Microsoft 365 Business

Microsoft는 가장 광범위하게 인기를 끌고 있는 비즈니스 제품의 평가판을 제공합니다. 앞으로 평가판 제품이 더 추가될 가능성이 있습니다.

현재 정부 제품, 교육 제품 또는 추가 기능 제품에 대 한 **무료 평가판은 없습니다** .

## <a name="licenses-for-free-trial-offers"></a>무료 평가판 제품에 대 한 라이선스

모든 무료 평가판은 25 개의 라이선스를 제공 합니다. 이 번호는 평가판을 통해 변경할 수 없습니다. 무료 평가판에서 사용자를 추가 하거나 제거할 수 없습니다. 평가판을 유료 구독으로 변환한 후 구독에 라이선스를 더 추가할 수 있습니다.

파트너 센터에서 유료 서비스를 사용할 때와 같은 방법으로 평가판 라이선스 및 사용자 수를 할당 해야 합니다.

## <a name="sign-customers-up-for-trials"></a>평가판을 위해 고객에 게 서명

파트너 센터를 통해 고객에 게 평가판을 등록 하려면 다음을 수행 합니다.

1. 파트너 센터의 **판매** 에서 **카탈로그로**이동 합니다. 
2. 카탈로그에서 **청구 주기**에 있는 **평가판 제품**을 클릭합니다. 이렇게 하면 무료 평가판만 표시되고 무료가 아닌 제품은 표시되지 않습니다. 평가판은 카탈로그의 **평가판** 탭에 표시됩니다.
3. 제공할 무료 평가판을 선택한 다음 **제출**을 선택합니다. 모든 평가판은 30일 동안 요금이 청구되지 않습니다. 또한 평가판 기간 중 언제든지 유료 구독으로 변환할 수 있습니다.

## <a name="converting-trials-to-paid-subscriptions"></a>평가판을 유료 구독으로 변환

무료 평가판은 자동으로 유료 구독으로 변환 되지 않습니다. 30 일 후에는 무료 평가판을 유료 구독으로 변환 해야 합니다. 그렇지 않으면 [만료](#expiring-offers)됩니다. 무료 평가판은 확장할 수 없습니다.

평가판을 유료 구독으로 변환 해야 합니다. [파트너 센터를 사용](#convert-trials-using-partner-center) 하거나 [파트너 센터 api를 통해](#convert-trials-using-apis)이 작업을 수행할 수 있습니다.

> [!NOTE]
> CSP (클라우드 솔루션 공급자) 프로그램에 대 한 고객 무료 평가판을 다른 프로그램 테 넌 트 (예: EA, Open 또는 MOSP)로 변환할 수 없습니다.

### <a name="convert-trials-using-partner-center"></a>파트너 센터를 사용 하 여 평가판 변환

다음과 같이 파트너 센터 대시보드를 사용 하 여 평가판을 유료 구독으로 변환할 수 있습니다.

1. 고객의 구독 페이지로 이동하여 무료 평가판을 선택합니다.
2. **무료 평가판을 유료 구독으로 전환**을 선택합니다.
3. 원하는 라이선스 수량 및 청구 주기를 입력하고 **적용**을 선택합니다.
4. 유료 구독에 대한 청구는 전환 날짜부터 시작되고, 구독은 전환 날짜로부터 12개월 후 자동 갱신됩니다. 

### <a name="convert-trials-using-apis"></a>Api를 사용 하 여 평가판 변환

무료 평가판을 유료 구독으로 변환 하기 위해 Api를 변경 해야 할 수 있습니다. 자세한 내용은 다음 개발자 설명서를 참조 하세요.

- [평가판 구독을 유료로 전환](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [평가판 전환 제품 목록 가져오기](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>제공 만료

만료 된 제품에 대 한 알림이 표시 되지 않습니다. 파트너 센터의 고객 보기를 사용 하거나 API를 쿼리하면 예정 된 만료 날짜를 추적할 수 있습니다. 고객의 결정 시점이 다가오면 적절한 후속 조치를 취할 수 있도록 이러한 날짜를 자주 모니터링하는 것이 좋습니다.

평가판이 만료 된 후 해당 평가판에 로그인을 시도 하는 고객에 게는 만료 메시지가 표시 됩니다. 그러나 데이터는 데이터 보존 표준에 맞게 저장 됩니다. 동일한 서비스 계획을 사용 하 여 새 구독을 구매한 후 새로 활성화 된 구독에서 다시 고객의 정보에 액세스할 수 있습니다.

## <a name="billing"></a>청구

연간 청구 및 무료 평가판은 소 버린 클라우드 및 공용 클라우드에서 동일 합니다. 유일한 차이점은 시작할 때 사용할 수 있는 평가판 Sku입니다.

## <a name="billing-for-free-trials"></a>무료 평가판에 대 한 청구

무료 평가판은 매월 및 매년 청구 되는 구독에 모두 사용할 수 있습니다. 평가판을 유료 구독으로 변환할 때 청구 주기를 선택할 수 있습니다.

구독 시작 날짜는 변환 날짜를 기준으로 합니다. 평가판이 연간 청구를 통한 유료 제품으로 전환되는 경우 구독 갱신 날짜는 전환 날짜로부터 12개월 이후입니다. 평가판이 월별 청구를 통한 유료 제품으로 전환되는 경우 구독 갱신 날짜는 전환 날짜 이후 청구 날짜로부터 12개월 이후입니다.

### <a name="invoices"></a>송장

청구서 또는 라이선스 기반 조정 파일에는 무료 평가판이 표시 되지 않습니다. 무료 평가판을 유료 구독으로 변환한 후에만 무료 평가판이 청구서 및 라이선스 기반 조정 파일에 표시 됩니다. 변환 된 구독은 새 구독과 동일한 방법으로 표시 됩니다.

### <a name="incentives"></a>인센티브

무료 평가판은 성과급에 영향을 주지 않습니다.

## <a name="support"></a>지원

무료 평가판에 대 한 지원은 파트너 센터를 통해 서비스 요청을 제출 합니다.
