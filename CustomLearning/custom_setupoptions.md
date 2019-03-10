---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 설치 옵션
ms.date: 02/11/2019
description: 사용자 지정 학습을 설정 하기 위한 옵션
ms.openlocfilehash: d9415469c60aa15153ea550aec715b523d1d365a
ms.sourcegitcommit: c358dcc2d69cc3db8fd24a1011550edebe0721fe
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2019
ms.locfileid: "30518183"
---
# <a name="custom-learning-setup-options"></a><span data-ttu-id="b1d29-103">사용자 지정 학습 설치 옵션</span><span class="sxs-lookup"><span data-stu-id="b1d29-103">Custom Learning Setup Options</span></span>
<span data-ttu-id="b1d29-104">Office 365에 대 한 사용자 지정 학습은 솔루션을 몇 가지 다른 방식으로 설정할 수 있는 유연성을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-104">Custom Learning for Office 365 provides the flexibility to set up the solution in a couple different ways.</span></span> <span data-ttu-id="b1d29-105">다음 섹션에서는 사용할 수 있는 옵션에 대해 간략하게 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-105">The following sections outline the options available.</span></span>

## <a name="recommended---setup-using-the-sharepoint-online-provisioning-service--"></a><span data-ttu-id="b1d29-106">권장-SharePoint Online 프로 비전 서비스를 사용 하 여 설정-</span><span class="sxs-lookup"><span data-stu-id="b1d29-106">Recommended - Setup using the SharePoint Online Provisioning Service -</span></span> 
<span data-ttu-id="b1d29-107">SharePoint Online 프로 비전 서비스는 사용자 지정 학습을 설정 하는 데 가장 빠르고 편리 하며 권장 되는 방법을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-107">The SharePoint Online Provisioning Service provides the fastest, easiest, and recommended method for setting up Custom Learning.</span></span> <span data-ttu-id="b1d29-108">SharePoint Online 프로 비전 서비스를 사용 하 여 Office 365 테 넌 트 관리자가 서비스에 로그인 하 고, 몇 가지 옵션을 선택한 다음, **테 넌 트에 추가** 를 클릭 하 여 사용자 지정 학습 사이트 및 사용자 지정 학습 웹 파트를 구축 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-108">With the SharePoint Online Provisioning Service, an Office 365 tenant admin signs into the service, makes a few choices, and clicks **Add to Tenant** to provision the Custom Learning Site and the Custom Learning Web part.</span></span> <span data-ttu-id="b1d29-109">프로비저닝이 완료 되 면 테 넌 트 관리자에 게 사이트를 보낼 수 있는 전자 메일을 수신 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-109">When provisioning is done, the Tenant Admin receives an email that the site is ready to go.</span></span> 

- <span data-ttu-id="b1d29-110">SharePoint 프로 비전 서비스를 시작 하려면 [PnP 프로 비전 서비스를 사용 하 여 프로 비전](custom_provision.md) 으로 이동 하세요.</span><span class="sxs-lookup"><span data-stu-id="b1d29-110">To get started with the SharePoint Provisioning Service, go to [Provision with the PnP Provisioning Service](custom_provision.md)</span></span>   

## <a name="stand-alone-setup-of-the-custom-learning-web-part"></a><span data-ttu-id="b1d29-111">사용자 지정 학습 웹 파트의 독립 실행형 설정</span><span class="sxs-lookup"><span data-stu-id="b1d29-111">Stand alone setup of the Custom Learning web part</span></span>
<span data-ttu-id="b1d29-112">이미 설정 된 sharepoint online 최신 통신 교육 포털이 있는 조직의 경우 사용자 지정 학습은 기존 SharePoint online 사이트에 사용자 지정 학습 웹 파트를 수동으로 설치 하는 옵션을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-112">For organizations that already have an established SharePoint Online modern communication training portal, Custom Learning provides the option to manually install the Custom Learning Web part into an existing SharePoint Online site.</span></span> <span data-ttu-id="b1d29-113">이 사이트는 최신 SharePoint Online 사이트 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-113">Note that the site must be a modern SharePoint Online site.</span></span> <span data-ttu-id="b1d29-114">이 방법을 사용 하려면 Windows PowerShell 또는 SharePoint Online 관리 셸에서 테 넌 트 관리자 권한 및 환경이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-114">This method requires Tenant Admin permissions and experience with Windows PowerShell or the SharePoint Online Management Shell.</span></span> 

- <span data-ttu-id="b1d29-115">수동 웹 파트 설치 지침에 대 한 자세한 내용은 [웹 파트 수동 설치](custom_manualsetup.md)를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="b1d29-115">For Manual web part installation instructions, see see [Manually install the web part](custom_manualsetup.md).</span></span> 

## <a name="upgrade-custom-learning"></a><span data-ttu-id="b1d29-116">사용자 지정 학습 업그레이드</span><span class="sxs-lookup"><span data-stu-id="b1d29-116">Upgrade Custom Learning</span></span>
<span data-ttu-id="b1d29-117">사용자 지정 학습 파일럿 프로그램에 참여 하거나 이미 사용자 지정 학습을 프로 비전 했을 수 있는 조직은 [사용자 지정 학습을 위해 수동 업그레이드](custom_upgrade.md) 를 제공 하는 지침을 따를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d29-117">Organizations that may have participated in a Custom Learning Pilot Program, or already have Custom Learning provisioned, can follow the instruction provided the [Manual Upgrade for Custom Learning](custom_upgrade.md)</span></span>    

### <a name="next-steps---provision-custom-learningcustomprovisionmd"></a><span data-ttu-id="b1d29-118">다음 단계- [사용자 지정 학습 프로 비전](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="b1d29-118">Next Steps - [Provision Custom Learning](custom_provision.md)</span></span>
