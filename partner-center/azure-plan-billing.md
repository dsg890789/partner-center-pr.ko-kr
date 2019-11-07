---
title: Azure 플랜 - 청구 | 파트너 센터
ms.topic: article
ms.date: 11/03/2019
description: Azure 플랜에 대한 청구서 및 조정 파일 구조에 대해 설명합니다.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: f7b2e22fb4cc0c424ad18278df644d289944ca01
ms.sourcegitcommit: d6913109534aa1f1f1e5db8c72f8026d159ec2a4
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/05/2019
ms.locfileid: "73595935"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="d5833-103">CSP의 새로운 상거래 환경 - Azure 청구</span><span class="sxs-lookup"><span data-stu-id="d5833-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="d5833-104">**적절한 역할:**</span><span class="sxs-lookup"><span data-stu-id="d5833-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="d5833-105">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="d5833-105">Billing admin</span></span>
- <span data-ttu-id="d5833-106">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="d5833-106">Admin agent</span></span>
- <span data-ttu-id="d5833-107">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="d5833-107">Global admin</span></span>


<span data-ttu-id="d5833-108">Azure 플랜에 따른 청구는 잘 조정된 단일 청구 날짜와 월별 청구 기간을 사용하는 간소화된 청구 환경입니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="d5833-109">청구 플랫폼에 대한 자세한 내용은 [청구 개요](billing-basics.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d5833-109">For information on the billing platform, read [Billing overview](billing-basics.md).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="d5833-110">청구 기본 정보 요약</span><span class="sxs-lookup"><span data-stu-id="d5833-110">Summary of billing essentials</span></span>

- <span data-ttu-id="d5833-111">**청구서 날짜**: 청구서 및 조정 파일은 8일(UTC 자정)에 파트너 센터 대시보드/API에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="d5833-112">**청구서 청구 기간**: 청구서 청구 기간은 달력의 월을 기준으로 조정됩니다(예: 10/1-10/31, 11/1-11/30).</span><span class="sxs-lookup"><span data-stu-id="d5833-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="d5833-113">**서비스 기간 요금 청구**: 요금은 달력의 월을 기준으로 조정됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="d5833-114">예를 들어 청구 파트너가 10/15에 Azure 플랜을 통해 Azure 서비스를 추가하고 고객이 10/15에 Azure 서비스 사용을 시작하는 경우 청구 파트너는 서비스 기간 10/15 - 10/31에 고객이 사용한 요금에 대한 청구서/조정 파일을 11/8에 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="d5833-115">12/8에 생성될 다음 달 청구서에는 서비스 기간 11/1 - 11/31의 모든 요금이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-115">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="d5833-116">**청구서 결제 기간**: 순 60일.</span><span class="sxs-lookup"><span data-stu-id="d5833-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="d5833-117">**청구서 통화** : 파트너는 고객의 국가에 할당된 통화로 계속 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="d5833-118">예를 들어 청구 파트너가 아일랜드에 있고 고객은 영국, 노르웨이 및 독일에 있는 경우 청구 파트너는 GBP, NOK 및 EUR 청구서/조정 파일을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="d5833-119">**파트너 인센티브**: 청구 월이 끝나고 45일 후에 결제됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="d5833-120">청구서 및 조정 파일 액세스</span><span class="sxs-lookup"><span data-stu-id="d5833-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="d5833-121">청구서를 볼 수 있게 되면 회사의 글로벌 관리자 또는 대금 청구 관리자에게 이메일을 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="d5833-122">**청구서 및 조정 파일에 액세스하려면**</span><span class="sxs-lookup"><span data-stu-id="d5833-122">**To access the invoice and reconciliation file**</span></span>

1. <span data-ttu-id="d5833-123">파트너 센터 [대시보드](https://partner.microsoft.com/en-us/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/).</span></span>

2. <span data-ttu-id="d5833-124">파트너 센터 메뉴에서 **청구**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="d5833-125">**되풀이** 및 **일회성** 탭과 관심 있는 통화를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

![청구](images/azure/billing1.png)

4. <span data-ttu-id="d5833-127">**청구서** 또는 **조정 파일**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-127">Select **Invoice** or **Reconciliation file**.</span></span>  

<span data-ttu-id="d5833-128">과거의 청구서 및 조정 파일을 보려면 아래쪽에서 청구 기록 행을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-128">To view historical invoices and recon files expand the Billing history row below.</span></span>


## <a name="understanding-usage-data"></a><span data-ttu-id="d5833-129">사용량 데이터 이해</span><span class="sxs-lookup"><span data-stu-id="d5833-129">Understanding usage data</span></span> 

1. <span data-ttu-id="d5833-130">Azure 플랜은 사용량에 대한 루트 또는 최상위 컨테이너입니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="d5833-131">모든 사용량은 단일 Azure 플랜에 다시 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-131">All usage is tied back to a single azure plan.</span></span> 

2. <span data-ttu-id="d5833-132">플랜 내에는 하나 이상의 Azure 구독이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="d5833-133">이러한 구독은 리소스 관리 및 배포에 사용되는 컨테이너입니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="d5833-134">구독 내에서 리소스 그룹은 그룹 리소스에 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="d5833-135">모든 리소스는 하나의 리소스 그룹에 배포됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="d5833-136">리소스의 예로 가상 머신 및 스토리지 계정이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="d5833-137">리소스 내보내기 측정기: 측정기는 리소스의 사용량을 측정하며, 하나의 리소스에서 여러 측정기의 사용량을 내보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="d5833-138">측정기는 ProductId, SKUId 및 AvailabilityId로 식별됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="heirarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="d5833-139">구독 리소스 그룹 및 계량의 계층 구조</span><span class="sxs-lookup"><span data-stu-id="d5833-139">Heirarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="d5833-140">**Azure 계정(테넌트)**</span><span class="sxs-lookup"><span data-stu-id="d5833-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="d5833-141">구독 A</span><span class="sxs-lookup"><span data-stu-id="d5833-141">Subscription A</span></span>
    - <span data-ttu-id="d5833-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="d5833-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="d5833-143">가상 머신(리소스)</span><span class="sxs-lookup"><span data-stu-id="d5833-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="d5833-144">컴퓨팅 측정기</span><span class="sxs-lookup"><span data-stu-id="d5833-144">Compute meter</span></span>
        - <span data-ttu-id="d5833-145">가상 네트워크(리소스)</span><span class="sxs-lookup"><span data-stu-id="d5833-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="d5833-146">청구 측정기 없음</span><span class="sxs-lookup"><span data-stu-id="d5833-146">No billing meter</span></span>

    - <span data-ttu-id="d5833-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="d5833-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="d5833-148">가상 머신(리소스)</span><span class="sxs-lookup"><span data-stu-id="d5833-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="d5833-149">컴퓨터 측정기</span><span class="sxs-lookup"><span data-stu-id="d5833-149">Computer meter</span></span>
        - <span data-ttu-id="d5833-150">프리미엄 SSD 관리 디스크(리소스)</span><span class="sxs-lookup"><span data-stu-id="d5833-150">Premium SSD managed disk (resource)</span></span>
            - <span data-ttu-id="d5833-151">스토리지 용량 측정기</span><span class="sxs-lookup"><span data-stu-id="d5833-151">Storage capacity meter</span></span>
            - <span data-ttu-id="d5833-152">스토리지 작업 수 측정기</span><span class="sxs-lookup"><span data-stu-id="d5833-152">Storage operations meter</span></span>

- <span data-ttu-id="d5833-153">구독 B   -ResourceGroup 1       - Azure SQL(리소스)           - DTU 측정기       - VPN Gateway(리소스)           - VPN Gateway 측정기</span><span class="sxs-lookup"><span data-stu-id="d5833-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="d5833-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="d5833-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="d5833-155">Virtual Network 인터페이스(리소스)</span><span class="sxs-lookup"><span data-stu-id="d5833-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="d5833-156">청구 측정기 없음</span><span class="sxs-lookup"><span data-stu-id="d5833-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="d5833-157">청구서 읽기</span><span class="sxs-lookup"><span data-stu-id="d5833-157">Read the invoice</span></span>

1. <span data-ttu-id="d5833-158">청구서는 매월 8일 이후에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-158">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="d5833-159">파트너는 60일 내에 결제 금액을 송금해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="d5833-160">청구 기간에는 지정된 달력 월(예: 10/1-10/31)이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="d5833-161">요금은 순 조정액입니다(금액은 "관리형 서비스에 대해 파트너가 획득한 순 크레딧").</span><span class="sxs-lookup"><span data-stu-id="d5833-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="d5833-162">자세한 청구 정보는 청구서 조정 파일 및 일일 평가 사용량 파일을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="d5833-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![청구서](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="d5833-164">청구서 조정 파일 읽기</span><span class="sxs-lookup"><span data-stu-id="d5833-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="d5833-165">각 Azure 플랜과 측정기의 조합은 조정 파일에 최대 두 개의 청구 줄을 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="d5833-166">측정기가 한 달 전체에 걸쳐 모든 유형의 할인 또는 크레딧(예: 계층화된 할인 또는 관리형 서비스에 대한 파트너 획득 크레딧)에 적합한 경우 조정 파일에는 하나의 청구 줄만 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="d5833-167">**PriceAdjusmentDescription** 열은 할인 또는 획득 크레딧을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="d5833-168">할인 또는 파트너 획득 크레딧에 적합한 특정 측정기에 대한 리소스가 없으면, 조정 파일에 하나의 청구 줄만 포함되며 유효 단가는 소매 가격(단가)이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="d5833-169">측정기 또는 해당 측정기를 내보내는 리소스가 월의 일부 동안 **관리형 서비스에 대한 파트너 획득 크레딧**에 적합한 경우 조정 파일에는 두 줄의 청구가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-169">If the meter, or any resources emitting that meter,qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="d5833-170">하나는 미터가 자격을 획득한 날을 표시하고 다른 하나는 미터가 자격을 획득하지 못한 날을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="d5833-171">일일 사용량 파일 읽기</span><span class="sxs-lookup"><span data-stu-id="d5833-171">Read the daily usage file</span></span>

- <span data-ttu-id="d5833-172">Azure 플랜 하의 구독 미터는 날마다 평가하여 누적됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="d5833-173">**관리형 서비스에 대한 파트너 획득 크레딧**은 매일 확인 및 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="d5833-174">모든 구독 미터에는 서비스가 사용된 월의 모든 날에 대한 행이 하나 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="d5833-175">아래 예제를 살펴보세요.</span><span class="sxs-lookup"><span data-stu-id="d5833-175">In the example below:</span></span>

  - <span data-ttu-id="d5833-176">미터가 7/1 – 7/3에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).</span><span class="sxs-lookup"><span data-stu-id="d5833-176">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="d5833-177">미터가 7/4 – 7/7에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득하지 못했습니다(유효 단가는 소매 가격).</span><span class="sxs-lookup"><span data-stu-id="d5833-177">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="d5833-178">미터가 7/8 – 7/31에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).</span><span class="sxs-lookup"><span data-stu-id="d5833-178">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="d5833-180">고객 통화로 작성된 청구서</span><span class="sxs-lookup"><span data-stu-id="d5833-180">Invoice in customer currency</span></span> 

<span data-ttu-id="d5833-181">Azure 플랜을 통한 Azure 서비스는 USD로 가격이 책정되며 고객의 국가에 할당된 통화 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="d5833-182">청구 통화가 USD가 아닌 경우 사용되는 환율은 청구서의 마지막 페이지에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="d5833-183">환율은 매월 결정되며 다음 청구서부터 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="d5833-184">국가 통화의 전체 목록은 [최신 상거래 제품 사용 가능 국가 및 고객 통화표](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d5833-184">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="d5833-185">Microsoft는 [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company)를 사용하여 가격 책정 통화를 청구 통화로 변환하는 데 사용되는 환율을 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-185">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="d5833-186">환율은 적용되는 월의 첫 번째 날짜 이전에 새로 고쳐지고 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-186">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="d5833-187">**예**:  8월 1일 – 8월 31일의 서비스 기간에 대한 사용량 요금은 7월 31일에 게시된 환율을 사용하여 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-187">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="d5833-188">이 요금은 9월 청구서에 표시되며, 청구서의 마지막 페이지에 환율이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-188">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

 
## <a name="azure-reservations"></a><span data-ttu-id="d5833-189">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="d5833-189">Azure reservations</span></span> 

<span data-ttu-id="d5833-190">Azure 플랜을 통해 [Azure 예약](https://docs.microsoft.com/partner-center/azure-reservations)을 구매하는 경우 파트너 센터에서 일회성 청구를 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-190">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="d5833-191">월별 청구는 Azure Portal에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-191">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="d5833-192">파트너 센터에서도 향후 월별 청구를 제공할 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-192">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-spending"></a><span data-ttu-id="d5833-193">Azure 지출</span><span class="sxs-lookup"><span data-stu-id="d5833-193">Azure spending</span></span> 

<span data-ttu-id="d5833-194">기존의 Azure 지출 환경이 파트너 센터에서 새 Azure 플랜 청구서를 지원하도록 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-194">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="d5833-195">이를 통해 파트너는 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-195">This enables partners to:</span></span>

- <span data-ttu-id="d5833-196">고객 수준에서 설정된 예산에 대한 경고 보기, 관리 및 받기</span><span class="sxs-lookup"><span data-stu-id="d5833-196">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="d5833-197">Azure 플랜에 대한 총 예상 지출 보기(리소스 및 측정기 수준별로 세분화됨)</span><span class="sxs-lookup"><span data-stu-id="d5833-197">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="d5833-198">Azure 플랜을 통한 Azure 서비스의 청구 모델은 후불 사용량 요금제이므로 청구 금액이 예상 금액을 초과하지 않도록 파트너는 월별 예산을 적용하고 사용률을 추적할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-198">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="d5833-199">예산을 한 고객에게 또는 동시에 여러 고객에게 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-199">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Azure 지출](images/azure/azurespend.png)

<span data-ttu-id="d5833-201">**자세한 내용**</span><span class="sxs-lookup"><span data-stu-id="d5833-201">**For more information**</span></span>

-  <span data-ttu-id="d5833-202">PEC(파트너 획득 크레딧)를 계산하는 방법은 파트너 센터 [대시보드](https://partner.microsoft.com/en-us/dashboard/)(로그인 필요)를 통해 사용할 수 있는 가격표에서 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5833-202">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/) (sign in required).</span></span> 
   
-  [<span data-ttu-id="d5833-203">Azure 플랜 구매</span><span class="sxs-lookup"><span data-stu-id="d5833-203">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="d5833-204">CSP의 새로운 상거래 환경에 대한 가격표</span><span class="sxs-lookup"><span data-stu-id="d5833-204">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)