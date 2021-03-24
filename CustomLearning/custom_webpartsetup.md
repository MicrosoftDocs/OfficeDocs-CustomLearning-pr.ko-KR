---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 사이트 프로비전
ms.date: 02/10/2019
description: SharePoint 프로비전 엔진을 통해 Office 365용 사용자 지정 학습 사이트 프로비전
ms.service: sharepoint online
ms.openlocfilehash: be45ade7588f08801062710d310ca967ddd23926
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2021
ms.locfileid: "51162925"
---
# <a name="provision-custom-learning"></a><span data-ttu-id="e0354-103">사용자 지정 학습 프로비전</span><span class="sxs-lookup"><span data-stu-id="e0354-103">Provision Custom Learning</span></span>

<span data-ttu-id="e0354-104">SharePoint Online 프로비저닝 서비스를 사용하여 Office 365 테넌트 관리자는 몇 번의 클릭으로 프로비저닝 프로세스를 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="e0354-105">프로비저닝 서비스는 사용자 지정 학습을 프로비전하는 권장 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-105">The Provisioning Service is the recommended way to provision Custom Learning.</span></span> <span data-ttu-id="e0354-106">빠르고 쉬우며 프로세스를 시작하는 데 몇 분 정도 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="e0354-107">그러나 프로비저닝 서비스를 시작하기 전에 프로비전을 위한 선행 준비를 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0354-108">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="e0354-108">Prerequisites</span></span>
 
<span data-ttu-id="e0354-109">프로비저닝 서비스 [SharePoint Online 프로비전](https://provisioning.sharepointpnp.com)서비스를 사용하여 사용자 지정 학습을 성공적으로 설정하려면 프로비저닝을 수행한 사람이 다음의 선행 요구 사항을 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-109">To successfully set up Custom Learning with the Provisioning Service [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com), the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="e0354-110">사용자 지정 학습을 프로비전하는 사람은 사용자 지정 학습을 프로비전할 테넌트의 테넌트 관리자 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-110">The person provisioning Custom Learning must be a Tenant Administratorof the tenant where Custom Learning will be provisioned.</span></span>  
- <span data-ttu-id="e0354-111">테넌트 앱 카탈로그는 SharePoint 관리 센터의 앱 옵션 내에서 사용할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-111">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="e0354-112">조직에 SharePoint 테넌트 앱 카탈로그가 없는 경우 [SharePoint Online](/sharepoint/use-app-catalog) 설명서를 참조하여 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-112">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="e0354-113">사용자 지정 학습을 프로비저닝하는 사람은 테넌트 앱 카탈로그의 사이트 모음 소유자가 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-113">The person provisioning Custom Learning must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="e0354-114">사용자 지정 학습을 프로비저닝하는 사용자가 앱 카탈로그의 사이트 모음 소유자가 아닌 경우 [이러한 지침을 완료하고](addappadmin.md) 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-114">If the person provisioning Custom Learning is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-custom-learning"></a><span data-ttu-id="e0354-115">사용자 지정 학습을 프로비전하기 위해</span><span class="sxs-lookup"><span data-stu-id="e0354-115">To provision Custom Learning</span></span>

1. <span data-ttu-id="e0354-116">으로 http://provisioning.sharepointpnp.com **이동하여 홈 페이지의** 오른쪽 위 모서리에서 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-116">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="e0354-117">사이트 서식 파일을 설치할 대상 테넌트의 자격 증명으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-117">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome.png](media/inst_signin.png)

2. <span data-ttu-id="e0354-119">조직을 대신하여 동의를 **지우고** 수락 을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="e0354-119">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![in](media/inst_perms.png)

3. <span data-ttu-id="e0354-121">솔루션 **갤러리에서 Office 365용** 사용자 지정 학습을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-121">Select **Custom Learning for Office 365** from the solution gallery.</span></span>

![in](media/inst_select.png)

4. <span data-ttu-id="e0354-123">솔루션 홈 페이지에서 **테넌트에 추가를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="e0354-123">From the solution home page select **Add to your Tenant**</span></span>

![inst_select.png](media/inst_add.png)

5. <span data-ttu-id="e0354-125">설치에 적합한 프로비저닝 정보 페이지의 필드 입력을 완료합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-125">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="e0354-126">최소한 프로비저닝 프로세스에 대한 알림을 받을 전자 메일 주소와 프로비전할 사이트의 대상 URL을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-126">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="e0354-127">"/sites/MyTraining" 또는 "/teams/LearnOffice365" 등 직원에게 친숙한 사이트의 대상 URL을 만드세요.</span><span class="sxs-lookup"><span data-stu-id="e0354-127">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnOffice365".</span></span>

![inst_options.png](media/inst_options.png)

6. <span data-ttu-id="e0354-129">**테넌트** 환경에 사용자 지정 학습을 설치할 준비가 되면 프로비전을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-129">Select **Provision** when ready to install Custom Learning into your tenant environment.</span></span>  <span data-ttu-id="e0354-130">프로비저닝 프로세스는 최대 15분이 소요됩니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-130">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="e0354-131">사이트에 액세스할 준비가 되면 이메일(프로비저닝 페이지에 입력한 알림 이메일 주소로)을 통해 알립니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-131">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e0354-132">사용자 지정 학습 사이트를 프로비전하는 테넌트 관리자는 사이트로 이동한 다음 CustomLearningAdmin.aspx를 열어 사용자 지정 학습 관리 속성을 초기화해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-132">The Tenant Admin who provisions the Custom Learning site must go to the site, and then open CustomLearningAdmin.aspx to initialize Custom Learning Admin properties.</span></span> <span data-ttu-id="e0354-133">이때 테넌트 관리자는 소유자를 사이트에 할당해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-133">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success"></a><span data-ttu-id="e0354-134">프로비저닝 성공 유효성 검사</span><span class="sxs-lookup"><span data-stu-id="e0354-134">Validate Provisioning Success</span></span>

<span data-ttu-id="e0354-135">프로비전이 완료되면 테넌트 관리자가 PnP 프로비전 서비스에서 전자 메일을 수신합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-135">When provisioning is complete, the Tenant Admin receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="e0354-136">관리자는 전자 메일에 제공된 사이트에 대한 링크를 복사한 다음 지침에 따라 사이트로 이동하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-136">The admin can copy the link to the site provided in the email, and then follow the instructions to go to the site.</span></span> <span data-ttu-id="e0354-137">또는 테넌트 관리자는 YOUR-SITE-COLLECTION-URL </SitePages/CustomLearningAdmin.aspx>탐색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-137">Alternately, the tenant admin can navigate to <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx.</span></span> <span data-ttu-id="e0354-138">이렇게 하면 처음 사용할 때 사용자 지정 학습을 설정하는 CustomConfig 목록 항목이 초기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-138">This initializes the CustomConfig list item that sets up Custom Learning for its first use.</span></span> <span data-ttu-id="e0354-139">이 페이지를 처음 여는 사람은 테넌트 관리자, 사이트 모음 관리자 또는 사이트 소유자입니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-139">The person who first opens this page must be a Tenant Admin,Site Collection Admin, or Owner of the site.</span></span> <span data-ttu-id="e0354-140">다음과 같은 페이지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-140">You should see a page that looks like this:</span></span> 

## <a name="add-owners-to-site"></a><span data-ttu-id="e0354-141">사이트에 소유자 추가</span><span class="sxs-lookup"><span data-stu-id="e0354-141">Add Owners to Site</span></span>
<span data-ttu-id="e0354-142">테넌트 관리자는 사이트를 사용자 지정하는 사람이 될 가능성이 낮기 때문에 사이트에 소유자를 할당해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-142">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign Owners to the site.</span></span> <span data-ttu-id="e0354-143">소유자는 사이트에 대한 관리 권한이 있으므로 사이트 페이지를 수정하고 사이트를 다시 브랜드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-143">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="e0354-144">또한 사용자 지정 학습 웹 파트를 통해 제공된 콘텐츠를 숨기고 표시하는 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-144">They also have the ability to hide and show content delivered through the Custom Learning Web part.</span></span> <span data-ttu-id="e0354-145">또한 사용자 지정 재생 목록을 빌드하고 사용자 지정 하위 목록에 할당하는 기능을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-145">They'll also have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="e0354-146">SharePoint **설정 메뉴에서** 사이트 **사용 권한 을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="e0354-146">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="e0354-147">고급 **사용 권한 설정을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="e0354-147">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="e0354-148">**Office 365 소유자에** 대한 사용자 지정 학습을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-148">Click **Custom learning for Office 365 Owners**.</span></span>
4. <span data-ttu-id="e0354-149">이 **그룹에 새** 사용자  >  **추가를 클릭하고** 소유자가 될 사용자를 추가한 다음 공유를 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="e0354-149">Click **New** > **Add Users to this group**, add the people you want to be Owners, and then click **Share**.</span></span>

8. <span data-ttu-id="e0354-150">페이지 오른쪽 **위** 모서리에서 다음 옵션을 클릭하여 사이트를 팔로우합니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-150">Click the **Following** option in the upper right hand corner of the page to follow the site.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="e0354-151">다음 단계</span><span class="sxs-lookup"><span data-stu-id="e0354-151">Next Steps</span></span>
- <span data-ttu-id="e0354-152">[웹Part에 포함된](sitecontent.md) 기본 콘텐츠를 살펴보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="e0354-152">Explore the [default content](sitecontent.md) included in the webpart.</span></span>