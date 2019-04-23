---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 자산에 연결
ms.date: 02/15/2019
description: 사용자 지정 학습 자산에 연결 하는 방법
ms.openlocfilehash: cdde37f370663ca50241833a15e8411921b45a1b
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056165"
---
# <a name="link-to-custom-learning-content"></a><span data-ttu-id="c63dc-103">사용자 지정 학습 콘텐츠에 연결</span><span class="sxs-lookup"><span data-stu-id="c63dc-103">Link to Custom Learning content</span></span>

<span data-ttu-id="c63dc-104">사용자 지정 학습을 통해 콘텐츠에 연결 하는 방법에는 두 가지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-104">With Custom Learning, there are two ways to link to content:</span></span>

- <span data-ttu-id="c63dc-105">표시할 콘텐츠에 대해 필터링 된 웹 파트를 호스트 하는 페이지에 대 한 링크입니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-105">Link to the page that host the Web part filtered for the content you want to display.</span></span> 
- <span data-ttu-id="c63dc-106">웹 파트 인스턴스에 직접 연결</span><span class="sxs-lookup"><span data-stu-id="c63dc-106">Link directly to an instance of the Web part</span></span>

## <a name="link-to-a-page"></a><span data-ttu-id="c63dc-107">페이지에 연결</span><span class="sxs-lookup"><span data-stu-id="c63dc-107">Link to a page</span></span>

<span data-ttu-id="c63dc-108">사용자 지정 학습 웹 파트에서 새 페이지 및 학습 환경을 만든 경우에는 웹 파트가 구성 된 페이지에 연결 하 여 표시 하려는 콘텐츠를 표시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-108">If you've created new pages and learning experiences with the Custom Learning Web part, you can link to the page with the Web part configured to show the content you want to display.</span></span> <span data-ttu-id="c63dc-109">이전 섹션에서는 페이지에 Excel 재생 목록을 표시 하는 방법을 다루었습니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-109">In the previous section, we covered how to display Excel playlists on a page.</span></span> <span data-ttu-id="c63dc-110">이제 홈 페이지를 편집 하 여 페이지에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-110">You could now edit the Home page to link to the page.</span></span> 

1. <span data-ttu-id="c63dc-111">홈 페이지에서 **편집**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-111">From the Home page, click **Edit**.</span></span>
2. <span data-ttu-id="c63dc-112">홈 페이지 타일 중 하나에서 **세부 정보 편집** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-112">Click **Edit details** in one of the Home page tiles.</span></span> <span data-ttu-id="c63dc-113">이 예에서는 **권장 재생 목록** 타일을 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-113">In this example, we edit the **Recommended playlists** tiles.</span></span>
3. <span data-ttu-id="c63dc-114">**연결**에서 **변경을**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-114">Under **Link**, click **Change**.</span></span>

![cg-linktopage-.png](media/cg-linktopage.png)

4. <span data-ttu-id="c63dc-116">**사이트**, **사이트 페이지**를 차례로 클릭 하 고 연결할 페이지를 클릭 한 다음 **열기**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-116">Click **Site**, then **Site Pages**, click the page you want to link to, and then click **Open**.</span></span> <span data-ttu-id="c63dc-117">이 예제에서는 이전 섹션에서 설명한 **Create-your-own-experience** 페이지에 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-117">In this example, we link to the **Create-your-own-experience.aspx** page covered in the previous section.</span></span>
5. <span data-ttu-id="c63dc-118">주인공 속성 창을 닫고 **게시**를 클릭 한 다음 링크를 테스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-118">Close the Hero properties pane, click **Publish**, and then test the link.</span></span> 

## <a name="link-to-the-custom-learning-web-part"></a><span data-ttu-id="c63dc-119">사용자 지정 학습 웹 파트에 연결</span><span class="sxs-lookup"><span data-stu-id="c63dc-119">Link to the Custom Learning web part</span></span>
<span data-ttu-id="c63dc-120">사용자 지정 학습은 관리자 또는 최종 사용자에 게 웹 파트가 포함 된 페이지와는 독립적으로 웹 파트 인스턴스에 연결할 수 있는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-120">Custom Learning gives you, the administrator, or an end-user, the ability to link to an instance of the Web part independent of the page that contains the Web part.</span></span> <span data-ttu-id="c63dc-121">복사 된 링크를 공유 하거나 다른 페이지에서 링크를 공유할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-121">You can share the copied link or link to it from other pages.</span></span> <span data-ttu-id="c63dc-122">복사 된 링크를 클릭 하면 CustomLLearningViewer 페이지에 사용자 지정 학습 웹 파트 인스턴스가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-122">The copied link, when clicked, shows the Custom Learning web part instance in the CustomLLearningViewer.aspx page.</span></span> <span data-ttu-id="c63dc-123">예를 살펴보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-123">Let's look at an example.</span></span> 

1. <span data-ttu-id="c63dc-124">홈 페이지에서 **Office 365 교육**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-124">From the Home page, click **Office 365 training**.</span></span>
2. <span data-ttu-id="c63dc-125">**microsoft 팀**을 클릭 하 고 **microsoft 팀 소개를**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-125">Click **Microsoft Teams**, and then click **Intro to Microsoft Teams**.</span></span>
3. <span data-ttu-id="c63dc-126">**복사** 아이콘을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-126">Click the **Copy** icon.</span></span>

![cg-linktowebpart-.png](media/cg-linktowebpart.png)

4. <span data-ttu-id="c63dc-128">사용자 지정 학습 메뉴에서 Home을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-128">Click Home from the Custom Learning menu.</span></span>
5. <span data-ttu-id="c63dc-129">브라우저의 주소 표시줄에 복사한 URL을 붙여넣고 enter 키를 누릅니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-129">Paste the copied URL in the address bar of the browser and press ENTER.</span></span> 

<span data-ttu-id="c63dc-130">다음 그림에 표시 된 것 처럼 링크는 CustomLearningViewer 페이지로 이동 하 고 복사 된 링크의 매개 변수에 따라 콘텐츠를 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="c63dc-130">As shown in the following illustration, the link goes to the CustomLearningViewer.aspx page and displays the content based on the parameters in the copied link.</span></span> 

![cg-linktowebpartviewer-.png](media/cg-linktowebpartviewer.png)

