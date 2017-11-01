---
title: "CSP 파트너 | 파트너 센터용 Cloudyn의 Azure 비용 관리"
description: "Cloudyn의 Azure 비용 관리를 사용하려면 파트너 센터 API에 프로비전된 액세스가 필요합니다."
author: Janet
robots: 
ms.openlocfilehash: d9f0b3f0f8bd6d76f05dacba27cf7ee2ddc5071b
ms.sourcegitcommit: d9f3e4e8115c0ad44f97041d352b703cda7ba9e5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/28/2017
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Azure CSP 파트너용 Azure 비용 관리 앱  

**적용 대상**

-  파트너 센터

[Azure 비용 관리에 대한 자세한 정보 얻기](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>시작하기 전에
Azure 비용 관리를 사용하려면 먼저 다음 요구 사항을 충족해야 합니다.
- 클라우드 솔루션 공급자 프로그램의 파트너여야 합니다.
- 파트너 센터 API 웹 앱을 만들 수 있어야 합니다.

## <a name="overview"></a>개요

Cloudyn의 Azure 비용 관리는 고객이 Azure를 사용하는 정도와 사용 비용을 추적하고 관리할 수 있는 웹 앱입니다. 파트너 센터 API를 통해 사용합니다.

## <a name="register-your-web-app-in-partner-center"></a>파트너 센터에서 웹 앱 등록
파트너 센터에서 Azure Active Directory 웹 앱을 등록하면 파트너 센터 API에 액세스할 수 있습니다. 
1.  [전역 관리자 또는 관리자 에이전트 계정](create-user-accounts-and-set-permissions.md)을 사용하여 [파트너 센터](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)에 로그인합니다.
2.  **대시보드**에서 **계정 설정** &gt; **[앱 관리](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**를 선택합니다.
3.  **Web App** 섹션에서 **Add new web app**를 클릭합니다.
<br> **참고**: 이전에 웹 앱을 만든 경우 3단계를 건너뛸 수 있습니다.
4.  웹 앱의 **Commerce ID** GUID 및 **App ID** GUID를 복사하고 저장합니다. 30일 무료 평가판 Azure 비용 관리 앱을 사용하려면 두 ID가 모두 필요합니다.

## <a name="add-a-secret-key-to-your-app"></a>앱에 비밀 키를 추가합니다.
1.  **Add key** 버튼 옆에 있는 드롭다운 목록에서 기간을 1년 또는 2년으로 선택합니다.
2.  **Add key**를 클릭합니다. 
3.  비밀 키 값을 복사하고 저장합니다. 30일 무료 평가판을 사용하려면 이 키가 필요합니다.
<br>**참고**: 응용 프로그램 비밀 키는 만료 날짜가 더 긴 암호와 같습니다. 나중에 사용할 수 있도록 키 값을 안전한 위치에 저장하십시오.

## <a name="next-steps"></a>다음 단계
[30일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작합니다.
평가판을 시작하려면 다음 세부 정보가 필요합니다.
- 파트너 센터 로그인 자격 증명
- Commerce ID GUID
- App ID GUID
- 응용 프로그램 비밀 키 값