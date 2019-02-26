---
author: karuanag
ms.author: karuanag
title: 설치를 위한 필수 구성 요소
ms.date: 02/11/2019
description: 사용자 지정 학습 설치 및 설정에 대 한 결정 및 필수 구성 요소 정보
ms.openlocfilehash: 1a57e8fbecfbce4608c8dcb618f4fdc007467789
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989719"
---
# <a name="getting-started"></a><span data-ttu-id="9aedb-103">시작</span><span class="sxs-lookup"><span data-stu-id="9aedb-103">Getting Started</span></span>

<span data-ttu-id="9aedb-p101">Office 365에 대 한 사용자 지정 학습을 통해 조직에 대 한 주문형 교육 솔루션을 제공할 수 있습니다.  여기에서는 배포를 성공적으로 수행 하는 데 필요한 사전 필수 구성 및 결정 사항에 대해 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aedb-p101">Custom Learning for Office 365 will allow you to provide on-demand training solutions for your organization.  Here we will discuss the pre-requisites and decisions you will need to make for a successful deployment.</span></span>

<span data-ttu-id="9aedb-p102">다음 지침에서는 테 넌 트 환경에 CLO365 커뮤니케이션 사이트 서식 파일 및 사용자 지정 학습 웹 파트의 설치를 포함 하 여 Office 365 (CLO365)에 대 한 사용자 지정 학습을 구축 하는 방법에 대해 간략하게 설명 합니다. 이 지침에서는 sharepoint online 프로 비전 서비스 https://provisioning.sharepointpnp.com 를 통해 CLO365을 설치 하는 과정을 안내 합니다. (기존 sharepoint online 통신 사이트에서 사용할 사용자 지정 학습 웹 파트만 설치 하려면 다음을 참조 하세요.) [사용자 지정 웹 파트 설치](installwebpart.md)지침</span><span class="sxs-lookup"><span data-stu-id="9aedb-p102">The following instructions outline how to provision Custom Learning for Office 365 (CLO365), including the installation of the CLO365 communication site template and the Custom Learning web part, into your tenant environment. These instructions cover the installation of CLO365 via the SharePoint Online Provisioning Service at https://provisioning.sharepointpnp.com    If you are interested in installing just the Custom Learning web part for use on an existing SharePoint Online communication site, please refer to the instructions for [installing the custom webpart](installwebpart.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="9aedb-108">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="9aedb-108">Prerequisites</span></span>
 
<span data-ttu-id="9aedb-109">[SharePoint Online 프로 비전 서비스](https://provisioning.sharepointpnp.com) 를 통해 CLO365을 설치 하려면 다음 사전 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aedb-109">To successfully install CLO365 via the [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com) you must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="9aedb-110">CLO365을 프로 비전 할 개인은 설치 대상 테 넌 트의 테 넌 트 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aedb-110">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>  
- <span data-ttu-id="9aedb-p103">SharePoint 관리 센터의 ' 앱 ' 옵션 내에서 테 넌 트 ' 앱 카탈로그 '를 사용할 수 있어야 합니다. 현재 앱 카탈로그가 없는 경우 [SharePoint Online 설명서](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) 를 참조 하 여이 기능을 프로 비전 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aedb-p103">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center. If you do not have an app catalog currently refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to provision this feature.</span></span>  
- <span data-ttu-id="9aedb-p104">CLO365을 프로 비전 할 개인은 설치를 위해 대상 테 넌 트에 있는 앱 카탈로그의 사이트 모음 소유자 여야 합니다. CLO365 설치 관리자가 앱 카탈로그의 사이트 모음 소유자가 아닌 경우에는 [이러한 지침을 완료](addappadmin.md) 하 고 계속 진행 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aedb-p104">The individual that will be provisioning CLO365 must be a site collection owner of the app catalog in the target tenant for install. If the CLO365 installer is not a site collection owner of the app catalog [complete these instructions](addappadmin.md) and continue.</span></span>  

### <a name="next-steps---service-decisionsservicedecisionsmd"></a><span data-ttu-id="9aedb-115">다음 단계- [서비스 결정](servicedecisions.md)</span><span class="sxs-lookup"><span data-stu-id="9aedb-115">Next Steps - [Service Decisions](servicedecisions.md)</span></span>
