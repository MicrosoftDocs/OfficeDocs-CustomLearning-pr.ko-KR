---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 학습 경로 사이트 구축
ms.date: 02/10/2019
description: SharePoint 프로 비전 서비스를 통해 Microsoft 365 학습 경로 사이트 프로 비전
ms.openlocfilehash: e48052a395a8669ef684110a1c93409f5859a1d2
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334749"
---
# <a name="provision-microsoft-365-learning-pathways"></a><span data-ttu-id="a0134-103">Microsoft 365 학습 경로 프로 비전</span><span class="sxs-lookup"><span data-stu-id="a0134-103">Provision Microsoft 365 learning pathways</span></span>

<span data-ttu-id="a0134-104">SharePoint Online 프로 비전 서비스를 사용 하 여 Office 365 테 넌 트 관리자는 몇 번의 간단한 클릭으로 프로 비전 프로세스를 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-104">With the SharePoint Online Provisioning Service, an Office 365 Tenant Administrator can start the provisioning process with a few simple clicks.</span></span> <span data-ttu-id="a0134-105">구축 서비스는 학습 경로를 프로 비전 하는 데 권장 되는 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-105">The Provisioning Service is the recommended way to provision learning pathways.</span></span> <span data-ttu-id="a0134-106">프로세스를 시작 하는 데 몇 분 정도 더 빠르고 간편 하 게 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-106">It's fast, easy, and takes only a few minutes to start the process.</span></span> <span data-ttu-id="a0134-107">프로 비전 서비스를 시작 하기 전에 먼저 프로 비전을 위한 필수 구성 요소를 충족 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-107">Before getting started with the Provisioning Service, however, make sure you've met the prerequisites for provisioning.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a0134-108">5/21/2019에서 Microsoft 365 학습 경로는 이전에 Office 용 사용자 지정 학습 365 이라는 솔루션의 새 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-108">As of 5/21/2019, Microsoft 365 learning pathways is the new name for the solution formerly known as Custom Learning for Office 365.</span></span> <span data-ttu-id="a0134-109">조직에서 Office 365에 대 한 사용자 지정 학습을 이미 구축 했으며 솔루션을 업데이트 하려는 경우 [Microsoft 365 학습 경로 추가 정보의](https://github.com/pnp/custom-learning-office-365)"솔루션 업데이트" 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="a0134-109">If you have already provisioned Custom Learning for Office 365 in your organization and want to update the solution, follow the “Updating the solution” instructions in the [Microsoft 365 learning pathways ReadMe](https://github.com/pnp/custom-learning-office-365).</span></span> <span data-ttu-id="a0134-110">Microsoft 365 학습 경로를 처음으로 프로 비전 하는 경우 Microsoft 365 학습 경로 설명서에서 [microsoft 365 learning 경로 지침 프로 비전]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) 을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="a0134-110">If you are provisioning Microsoft 365 learning pathways for the first time, see [Provision Microsoft 365 learning pathways instructions]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) in the Microsoft 365 learning pathways documentation.</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="a0134-111">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="a0134-111">Prerequisites</span></span>
 
<span data-ttu-id="a0134-112">프로 비전 서비스를 사용 하 여 Microsoft 365 학습 경로를 설정 하려면 프로 비전을 수행 하는 사람이 다음 사전 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-112">To successfully set up Microsoft 365 learning pathways with the Provisioning Service, the person doing the provisioning must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="a0134-113">학습용 경로는 학습용 경로가 프로 비전 될 테 넌 트의 테 넌 트 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-113">The person provisioning learning pathways must be a Tenant Administrator of the tenant where learning pathways will be provisioned.</span></span>  
- <span data-ttu-id="a0134-114">SharePoint 관리 센터의 앱 옵션 내에서 테 넌 트 앱 카탈로그를 사용할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-114">A tenant App Catalog must be available within the Apps option of the SharePoint Admin Center.</span></span> <span data-ttu-id="a0134-115">조직에 SharePoint 테 넌 트 앱 카탈로그가 없는 경우 [Sharepoint Online 문서](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) 를 참조 하 여 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-115">If your organization does not have an SharePoint tenant App catalog, refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to create one.</span></span>  
- <span data-ttu-id="a0134-116">학습용 경로는 테 넌 트 앱 카탈로그의 사이트 모음 소유자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-116">The person provisioning learning pathways must be a Site Collection Owner of the Tenant App Catalog.</span></span> <span data-ttu-id="a0134-117">학습 경로를 프로 비전 하는 사람이 앱 카탈로그의 사이트 모음 소유자가 아닌 경우에는 [이러한 지침을 완료](addappadmin.md) 하 고 계속 진행 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-117">If the person provisioning learning pathways is not a Site Collection Owner of the App Catalog [complete these instructions](addappadmin.md) and continue.</span></span> 

### <a name="to-provision-learning-pathways"></a><span data-ttu-id="a0134-118">학습 경로를 프로 비전 하려면</span><span class="sxs-lookup"><span data-stu-id="a0134-118">To provision learning pathways</span></span>

1. <span data-ttu-id="a0134-119">http://provisioning.sharepointpnp.com 홈 페이지의 오른쪽 위 모서리에서 이동 하 여 **로그인** 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-119">Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.</span></span>  <span data-ttu-id="a0134-120">사이트 서식 파일을 설치 하려는 대상 테 넌 트에 대 한 자격 증명으로 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-120">Sign in with the  credentials for the targeted tenant where you plan to install the site template.</span></span>

![pnphome-.png](media/inst_signin.png)

2. <span data-ttu-id="a0134-122">**조직 대신 동의** 를 지우고 **수락**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-122">Clear the **Consent on behalf of your organization** and select **Accept**.</span></span>

![내](media/inst_perms.png)

<span data-ttu-id="a0134-124">이 프로 비전 서비스에는 테 넌 트 앱 카탈로그를 만들고 해당 응용 프로그램을 테 넌 트 앱 카탈로그에 설치 하 고 사이트 서식 파일을 프로 비전 하기 위해 이러한 권한이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-124">The provisioning service requires these permissions to create the tenant app catalog, install the application into the tenant app catalog and provision the site template.</span></span> <span data-ttu-id="a0134-125">테 넌 트에 전체적인 영향은 없으며 이러한 권한은 솔루션 설치의 목적으로 명시적으로 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-125">There is no overall impact on your tenant and these permissions are explicitly used for the purpose of the solution installation.</span></span> <span data-ttu-id="a0134-126">설치를 계속 하려면 이러한 사용 권한을 수락 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-126">You must accept these permissions to proceed with the installation.</span></span>

3. <span data-ttu-id="a0134-127">페이지를 아래로 스크롤하여 **솔루션** 탭을 선택한 다음 **Office 365에 대 한 학습 경로**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-127">Scroll down the page, select the **Solutions** tab, and then select **learning pathways for Office 365**.</span></span> 

![내](media/inst_select.png)

4. <span data-ttu-id="a0134-129">**테 넌 트에 추가를 선택 합니다** .</span><span class="sxs-lookup"><span data-stu-id="a0134-129">Select **Add to your tenant**</span></span>

![inst_select-.png](media/inst_add.png)

5. <span data-ttu-id="a0134-131">설치에 적합 하도록 프로 비전 정보 페이지의 필드를 완성 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-131">Complete the fields on the provisioning information page as appropriate for your installation.</span></span> <span data-ttu-id="a0134-132">적어도 프로 비전 프로세스에 대 한 알림을 받을 전자 메일 주소와 사이트를 프로 비전 할 대상 URL을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-132">At a minimum enter the email address where you wish to get notifications about the provisioning process and the destination URL for your site to be provisioned to.</span></span>  
> [!NOTE]
> <span data-ttu-id="a0134-133">"/Sites/MyTraining" 또는 "/teams/LearnMicrosoft365"과 같은 직원에 게 친숙 한 사이트의 대상 URL을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-133">Make the destination URL for your site something friendly to your employees such as "/sites/MyTraining" or "/teams/LearnMicrosoft365".</span></span>

![inst_options-.png](media/inst_options.png)

6. <span data-ttu-id="a0134-135">사용자의 테 넌 트 환경에 학습 경로를 설치할 준비가 되 면 **프로 비전** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-135">Select **Provision** when ready to install learning pathways into your tenant environment.</span></span>  <span data-ttu-id="a0134-136">구축 프로세스는 최대 15 분까지 소요 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-136">The provisioning process will take up to 15 minutes.</span></span> <span data-ttu-id="a0134-137">사이트에 액세스할 준비가 되 면 프로 비전 페이지에서 입력 한 알림 전자 메일 주소로 전자 메일을 통해 알림 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-137">You will be notified via email (to the notification email address you entered on the Provisioning page) when the site is ready for access.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="a0134-138">학습 경로 사이트를 프로 비전 하는 테 넌 트 관리자는 해당 사이트로 이동한 다음 **CustomLearningAdmin** 를 열어 학습 경로 관리 속성을 초기화 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-138">The Tenant Admin who provisions the learning pathways site must go to the site, and then open **CustomLearningAdmin.aspx** to initialize learning pathways Admin properties.</span></span> <span data-ttu-id="a0134-139">현재, 테 넌 트 관리자는 소유자를 사이트에도 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-139">At this time, the Tenant Admin should also assign Owners to the site.</span></span> 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a><span data-ttu-id="a0134-140">프로 비전 성공 유효성 검사 및 CustomConfig 목록 초기화</span><span class="sxs-lookup"><span data-stu-id="a0134-140">Validate Provisioning Success and Initialize the CustomConfig List</span></span>

<span data-ttu-id="a0134-141">프로비저닝이 완료 되 면 사이트를 프로 비전 한 테 넌 트 관리자가 PnP 프로 비전 서비스에서 전자 메일을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-141">When provisioning is complete, the Tenant Admin who provisioned the site, receives an email from the PnP Provisioning Service.</span></span> <span data-ttu-id="a0134-142">전자 메일에 사이트에 대 한 링크가 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-142">The email contains a link to the site.</span></span> <span data-ttu-id="a0134-143">이때 테 넌 트 관리자는 전자 메일에 제공 된 링크를 사용 하 여 사이트에 방문 하 고 처음 사용할 수 있도록 사이트를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-143">At this point, the Tenant Admin should go to the site using the link provided in the email and set up the site for first use:</span></span>

- <span data-ttu-id="a0134-144">`<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-144">Go to `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`.</span></span> <span data-ttu-id="a0134-145">**CustomLearningAdmin** 를 열면 처음 사용할 학습 경로를 설정 하는 **customconfig** 목록 항목이 초기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-145">Opening **CustomLearningAdmin.aspx** initializes the **CustomConfig** list item that sets up learning pathways for first use.</span></span> <span data-ttu-id="a0134-146">다음과 같은 페이지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-146">You should see a page that looks like this:</span></span>

![cg-adminapppage-.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a><span data-ttu-id="a0134-148">사이트에 소유자 추가</span><span class="sxs-lookup"><span data-stu-id="a0134-148">Add Owners to Site</span></span>
<span data-ttu-id="a0134-149">테 넌 트 관리자는 사이트를 사용자 지정 하는 사용자가 될 가능성은 없으며, 사이트에 소수의 소유자를 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-149">As the Tenant Admin, it's unlikely you'll be the person customizing the site, so you'll need to assign a few owners to the site.</span></span> <span data-ttu-id="a0134-150">소유자는 사이트 페이지를 수정 하 고 사이트를 다시 브랜딩 할 수 있도록 사이트에 대 한 관리 권한을 가집니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-150">Owners have administrative privileges on the site so they can modify site pages and rebrand the site.</span></span> <span data-ttu-id="a0134-151">또한 학습 경로 웹 파트를 통해 제공 되는 콘텐츠를 숨기 거 나 표시 하는 기능도 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-151">They also have the ability to hide and show content delivered through the learning pathways Web part.</span></span> <span data-ttu-id="a0134-152">또한 사용자 지정 재생 목록을 작성 하 고 사용자 지정 하위 범주에 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-152">In addition, they'll have the ability to build custom playlist and assign them to custom subcategories.</span></span>  

1. <span data-ttu-id="a0134-153">SharePoint **설정** 메뉴에서 **사이트 사용 권한을**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-153">From the SharePoint **Settings** menu, click **Site Permissions**.</span></span>
2. <span data-ttu-id="a0134-154">**고급 사용 권한 설정을**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-154">Click **Advanced Permission Settings**.</span></span>
3. <span data-ttu-id="a0134-155">**Microsoft 365 learning 경로 소유자**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-155">Click **Microsoft 365 learning pathways Owners**.</span></span>
4. <span data-ttu-id="a0134-156">**새로 만들기** > **사용자를이 그룹에 추가**를 클릭 한 다음 소유자가 하려는 사용자를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-156">Click **New** > **Add Users to this group**, and then add the people you want to be Owners.</span></span> 
5. <span data-ttu-id="a0134-157">링크를 추가 하 여 공유 메시지에서 [사이트를 탐색](custom_exploresite.md) 하 고 **공유**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-157">Add a link to [Explore the Site](custom_exploresite.md) in the Share message, and then click **Share**.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a0134-158">다음 단계</span><span class="sxs-lookup"><span data-stu-id="a0134-158">Next Steps</span></span>
- <span data-ttu-id="a0134-159">사이트 및 웹 파트에서 제공 되는 [기본 콘텐츠](custom_exploresite.md) 를 살펴봅니다.</span><span class="sxs-lookup"><span data-stu-id="a0134-159">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
