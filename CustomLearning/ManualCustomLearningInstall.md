---
author: pkrebs
ms.author: pkrebs
title: 수동 설치 학습 경로
ms.date: 02/18/2019
manager: bpardi
description: 수동 설치 학습 경로
audience: itpro
ms.service: o365-administration
ms.topic: article
ms.openlocfilehash: 212ee8a1517cf79538d4a2d076f60f9382eeaf74
ms.sourcegitcommit: 96ad347dc08694ce2af5a5d42bf1f753d1c30a65
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51749316"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a><span data-ttu-id="0c647-103">Office 365용 사용자 지정 학습 수동 설치 및 구성</span><span class="sxs-lookup"><span data-stu-id="0c647-103">Manually installing and configuring Custom Learning for Office 365</span></span>

<span data-ttu-id="0c647-104">Microsoft 사용자 지정 학습 웹 파트는 [SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) 버전 1.7.1을 사용하여 빌드됩니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-104">The Microsoft Custom Learning Web Part is build using the [SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) version 1.7.1.</span></span>

<span data-ttu-id="0c647-105">웹 파트 및 사이트 모음을 수동으로 설치 및 구성하려면 다음 단계를 완료해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-105">To manually install and configure the web part and site collection, you will need to complete the following steps:</span></span>

1. <span data-ttu-id="0c647-106">모든 선행 요구를 충족하는지 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-106">Validate that you have met all the prerequisites.</span></span>
1. <span data-ttu-id="0c647-107">Office 365 테넌트 앱 카탈로그에 customlearning.sppkg 파일을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-107">Install the customlearning.sppkg file in your Office 365 Tenant App Catalog.</span></span>
1. <span data-ttu-id="0c647-108">Office 365 홈 사이트에 대한 사용자 지정 학습으로 사용할 최신 커뮤니케이션 사이트를 프로비전/식별합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-108">Provision/Identify a modern communication site to act as your Custom Learning for Office 365 home site.</span></span>
1. <span data-ttu-id="0c647-109">사용자 지정 학습이 사용하는 적절한 아티팩트로 테넌트를 구성하는 PowerShell 스크립트를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-109">Execute a PowerShell script that will configure your tenant with the appropriate artifacts that Custom Learning depends on.</span></span>
1. <span data-ttu-id="0c647-110">CustomLearningAdmin.aspx 사이트 페이지로 이동하여 관리 웹 파트를 로드하여 사용자 지정 콘텐츠 구성을 초기화합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-110">Navigate to the CustomLearningAdmin.aspx site page to load the admin web part to initialize the custom content configuration.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c647-111">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="0c647-111">Prerequisites</span></span>

<span data-ttu-id="0c647-112">테넌트 전체 앱 카탈로그를 설정하고 구성해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-112">You must have set up and configured the tenant-wide App Catalog.</span></span> <span data-ttu-id="0c647-113">[Office 365](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) 테넌트 설정 및 앱 카탈로그 사이트 만들기 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0c647-113">See [Set up your Office 365 tenant](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) and follow the Create app catalog site section.</span></span> <span data-ttu-id="0c647-114">테넌트 전체 앱 카탈로그가 이미 프로비전된 경우 이 설치 프로세스를 완료하기 위해 패키지를 업로드할 권한이 있는 계정에 액세스해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-114">If your tenant-wide App Catalog has already been provisioned, you will need access to an account that has rights to upload a package to it to complete this setup process.</span></span> <span data-ttu-id="0c647-115">일반적으로 이 계정에는 SharePoint 관리자 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-115">Generally this account has the SharePoint administrator role.</span></span> <span data-ttu-id="0c647-116">해당 역할의 계정이 작동하지 않는 경우 SharePoint 관리 센터로 이동하여 앱 카탈로그 사이트 모음에 대한 사이트 모음 관리자를 찾은 다음 사이트 모음 관리자 중 하나로 로그인하거나 사이트 모음 관리자에게 실패한 SharePoint 관리자 계정을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-116">If an account with that role does not work, go to the SharePoint admin center and find the Site Collection Administrators for the app catalog site collection and either log in as one of the Site Collection Administrators, or add the SharePoint administrator account that failed to the Site Collection Administrators.</span></span> <span data-ttu-id="0c647-117">또한 SharePoint 테넌트 관리자인 계정에 대한 액세스 권한이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-117">You will also need access to an account that is a SharePoint Tenant Admin.</span></span>

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a><span data-ttu-id="0c647-118">테넌트 앱 카탈로그에 웹 파트 업로드</span><span class="sxs-lookup"><span data-stu-id="0c647-118">Upload the web part to the Tenant App Catalog</span></span>

<span data-ttu-id="0c647-119">Office 365에 대한 사용자 지정 학습을 설정하려면 사용자 지정learning.sppkg 파일을 테넌트 전체 앱 카탈로그에 업로드하고 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-119">To set up Custom Learning for Office 365, you upload the customlearning.sppkg file to the tenant-wide App Catalog and deploy it.</span></span> <span data-ttu-id="0c647-120">앱 카탈로그에 앱을 추가하는 방법에 대한 자세한 내용은 앱 카탈로그를 사용하여 [SharePoint Online](/sharepoint/use-app-catalog) 환경에 사용자 지정 비즈니스 앱을 사용할 수 있도록 만들기를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0c647-120">See [Use the App Catalog to make custom business apps available for your SharePoint Online environment](/sharepoint/use-app-catalog) for detailed instructions on how to add an app to the app catalog.</span></span>

## <a name="provisionidentify-modern-communication-site"></a><span data-ttu-id="0c647-121">최신 커뮤니케이션 사이트 프로비전/식별</span><span class="sxs-lookup"><span data-stu-id="0c647-121">Provision/Identify Modern Communication Site</span></span>

<span data-ttu-id="0c647-122">기존 SharePoint 통신 사이트를 식별하거나 SharePoint Online 테넌트에서 새 사이트를 프로비전합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-122">Either identify an existing SharePoint communication site or provision a new one in your SharePoint Online tenant.</span></span> <span data-ttu-id="0c647-123">커뮤니케이션 사이트를 프로비전하는 방법에 대한 자세한 내용은 [SharePoint Online에서](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) 커뮤니케이션 사이트 만들기를 참조하고 단계에 따라 커뮤니케이션 사이트를 만드십시오.</span><span class="sxs-lookup"><span data-stu-id="0c647-123">For more information about how to provision a communication site, see [Create a communication site in SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) and follow the steps to create a communication site.</span></span>

## <a name="set-permissions-for-the-site"></a><span data-ttu-id="0c647-124">사이트에 대한 사용 권한 설정</span><span class="sxs-lookup"><span data-stu-id="0c647-124">Set permissions for the site</span></span>

<span data-ttu-id="0c647-125">방문자 그룹에 콘텐츠를 볼 수 있는 모든 사용자와 사용자 지정 재생 목록을 관리할 수 있는 모든 사람을 구성원 그룹에 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-125">You will want to add everyone who should be able to view content to the Visitors group and everyone who should be able to administer custom playlists to the Members group.</span></span> <span data-ttu-id="0c647-126">사용자가 처음 사이트 모음 관리자 또는 Owners 그룹의 일부가 되어야 하는 경우 사용자 지정 학습에 맞게 사이트를 구성하려면</span><span class="sxs-lookup"><span data-stu-id="0c647-126">To configure the site for Custom Learning the first time the user must be either a site collection administrator or part of the Owners group.</span></span>

<span data-ttu-id="0c647-127">사이트 모음에 Office 365용 사용자 지정 학습 앱을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-127">Add Custom Learning for Office 365 App to the site collection.</span></span>

## <a name="execute-powershell-configuration-script"></a><span data-ttu-id="0c647-128">PowerShell 구성 스크립트 실행</span><span class="sxs-lookup"><span data-stu-id="0c647-128">Execute PowerShell Configuration Script</span></span>

<span data-ttu-id="0c647-129">솔루션에서 사용하는 세 개의 테넌트 속성을 만들기 위해 실행해야 하는 PowerShell `CustomLearningConfiguration.ps1` 스크립트가 포함되어 [](/sharepoint/dev/spfx/tenant-properties) 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-129">A PowerShell script `CustomLearningConfiguration.ps1` is included that you will need to execute to create three [tenant properties](/sharepoint/dev/spfx/tenant-properties) that the solution uses.</span></span> <span data-ttu-id="0c647-130">또한 스크립트는 사이트 [](/sharepoint/dev/spfx/web-parts/single-part-app-pages) 페이지 라이브러리에 두 개의 단일 파트 앱 페이지를 만들어 알려진 위치에서 관리자 및 사용자 웹 파트를 호스팅합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-130">In addition, the script creates two [single part app pages](/sharepoint/dev/spfx/web-parts/single-part-app-pages) in the site pages library to host the admin and user web parts at a known location.</span></span>

### <a name="disabling-telemetry-collection"></a><span data-ttu-id="0c647-131">원격 분석 컬렉션을하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-131">Disabling Telemetry Collection</span></span>

<span data-ttu-id="0c647-132">이 솔루션의 일부에는 기본적으로 설정되어 있는, 비동기화된 원격 분석 추적 옵트인이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-132">Part of this solution includes anonymized telemetry tracking opt-in, which by default is set to on.</span></span> <span data-ttu-id="0c647-133">수동 설치를 수행하고 원격 분석 추적을 해제하려면 스크립트를 변경하여 $optInTelemetry 변수를 `CustomlearningConfiguration.ps1` $false.</span><span class="sxs-lookup"><span data-stu-id="0c647-133">If you are performing a manual install and you would like to turn telemetry tracking off, change the `CustomlearningConfiguration.ps1` script to set the $optInTelemetry variable to $false.</span></span>

<span data-ttu-id="0c647-134">수동 설치를 수행하지 않는 경우 원격 분석 추적을 해제하려면 실행 시 원격 분석 추적을 사용하지 않도록 설정하는 별도의 `TelemetryOptOut.ps1` 스크립트가 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-134">If you are not performing a manual install and would like to turn telemetry tracking off, a separate script `TelemetryOptOut.ps1` has been included that when run will disable telemetry tracking.</span></span>

## <a name="initialize-web-part-custom-configuration"></a><span data-ttu-id="0c647-135">웹 파트 사용자 지정 구성 초기화</span><span class="sxs-lookup"><span data-stu-id="0c647-135">Initialize web part custom configuration</span></span>

<span data-ttu-id="0c647-136">PowerShell 스크립트가 성공적으로 실행된 후 로 `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-136">After the PowerShell script is successfully run, navigate to `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="0c647-137">이렇게 하면 처음 사용할 사용자 지정 학습을 설정하는 CustomConfig 목록 항목이 초기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-137">This initializes the CustomConfig list item that sets up custom learning for its first use.</span></span>

<span data-ttu-id="0c647-138">이제 구성이 완료되어 Office 365용 사용자 지정 학습을 사용하여 진행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0c647-138">The configuration is now complete and you can move forward with using Custom Learning for Office 365.</span></span> <span data-ttu-id="0c647-139">자세한 내용은 사용자 설명서를 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="0c647-139">See the user documentation for more information.</span></span>
