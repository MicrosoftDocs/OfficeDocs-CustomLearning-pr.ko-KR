---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 관리 페이지 액세스
ms.date: 02/15/2019
description: 웹 파트 또는 메뉴에서 사용자 지정 학습 관리 페이지에 액세스 하는 방법
ms.openlocfilehash: 11bb2327948aedbc2db83138dd70c3ee76d085b6
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055534"
---
# <a name="access-the-custom-learning-administration-page"></a><span data-ttu-id="2e4c3-103">사용자 지정 학습 관리 페이지 액세스</span><span class="sxs-lookup"><span data-stu-id="2e4c3-103">Access the Custom Learning Administration page</span></span>

<span data-ttu-id="2e4c3-104">사용자 지정 학습 관리 페이지는 사용자 지정 학습 웹 파트를 관리 하기 위한 중앙 제어 지점입니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-104">The Custom Learning Administration page is the central controlling point for administration of the Custom Learning web part.</span></span> <span data-ttu-id="2e4c3-105">사용자 지정 학습 관리 페이지는 SharePoint 관리자만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-105">The Custom Learning Administration page is only available to SharePoint Administrators.</span></span> <span data-ttu-id="2e4c3-106">사이트를 방문 하는 구성원 권한이 있는 사용자는 **재생 목록 관리** 옵션을 볼 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-106">Users with member privileges visiting the site will not see the **Administer Playlist** option.</span></span> <span data-ttu-id="2e4c3-107">또한 관리자만이 SharePoint **Home** menu 항목에서 사용자 지정 학습 관리 페이지를 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-107">In addition, only Administrators will have the ability to open the Custom Learning Administration page from the SharePoint **Home** menu item.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="2e4c3-108">제품 하위 범주 또는 재생 목록 숨기기와 같은 사용자 지정 학습 관리 페이지에서 변경한 내용은 해당 웹 파트의 모든 인스턴스에 반영 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-108">Changes made on the Custom Learning Administration page, such as hiding a product subcategory or playlist, will be reflected in all instances of the Web part.</span></span> <span data-ttu-id="2e4c3-109">또한 사용자 지정 학습은 여러 사용자가 동시에 사용자 지정 학습 관리를 사용 하는 경우 충돌 감지를 제공 하지 않으므로 관리자는 한 번에 한 명만 사용자 지정 학습 관리자 페이지를 변경 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-109">In addition, it’s recommended that only one administrator at time make changes on the Custom Learning Administrator page, since Custom Learning does not provide collision detection if multiple people are using the Custom Learning Administration at the same time.</span></span>  

## <a name="access-from-the-custom-learning-web-part---preferred-method"></a><span data-ttu-id="2e4c3-110">사용자 지정 학습 웹 파트의 기본 설정 방법</span><span class="sxs-lookup"><span data-stu-id="2e4c3-110">Access from the Custom Learning Web part - preferred method</span></span>
<span data-ttu-id="2e4c3-111">이 예제에서 볼 수 있듯이 웹 파트에서 사용자 지정 학습 관리 페이지를 여는 것은 새 브라우저 창에서 관리 페이지를 여는 것 보다 기본 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-111">As we'll show you in this example, opening the Custom Learning Administration page from the web part is the preferred method since it opens the Admin page in a new browser window.</span></span> <span data-ttu-id="2e4c3-112">이 방법을 사용 하 여 작업을 확인 하거나 수정 하기 위해 탭 페이지를 앞뒤로 쉽게 전환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-112">With this method, it's easy to flip back and forth between the tabbed pages to check or modify your work.</span></span>  

1. <span data-ttu-id="2e4c3-113">사용자 지정 학습 홈 페이지에서 **Office 365 트레이닝** 타일을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-113">From the Custom Learning Home page, click the **Office 365 training** tile.</span></span>
2. <span data-ttu-id="2e4c3-114">**사용자 지정 학습 시스템** 메뉴를 클릭 한 다음 **재생 목록 관리**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-114">Click the **Custom Learning System** menu, then click **Administer Playlist**.</span></span> 

![cg-adminaccbtn-.png](media/cg-adminaccbtn.png)

## <a name="access-from-the-custom-learning-menu-item"></a><span data-ttu-id="2e4c3-116">사용자 지정 학습 메뉴 항목에서 액세스</span><span class="sxs-lookup"><span data-stu-id="2e4c3-116">Access from the Custom Learning menu item</span></span>
<span data-ttu-id="2e4c3-117">관리자는 웹 파트가 있는 페이지로 이동 하는 대신 SharePoint **Home** 메뉴 항목에서 사용자 지정 학습 관리 페이지에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-117">Rather than navigate to a page with a Web part, administrators can access the Custom Learning Adminstration page from the SharePoint **Home** menu item.</span></span> 

- <span data-ttu-id="2e4c3-118">사용자 지정 학습 홈 페이지에서 **홈** 메뉴를 클릭 한 다음 **사용자 지정 학습 관리**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="2e4c3-118">From the Custom Learning Home page, click the **Home** menu, then click **Custom Learning Administration**.</span></span>

![cg-adminaccmenu-.png](media/cg-adminaccmenu.png)