---
author: karuanag
ms.author: karuanag
title: 필수 구성 요소가 및 결정
ms.date: 02/10/2019
description: 결정 사항 및 사용자 지정 학습 설치 및 설정에 대 한 필수 구성 요소 정보
ms.openlocfilehash: 99ab08d8b18be00c3a29878ff462f9109cc9ed29
ms.sourcegitcommit: f93a6a691331515ba10f4d43b491928ec268f0ec
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29952637"
---
## <a name="service-decisions"></a><span data-ttu-id="c9d2a-103">서비스 결정</span><span class="sxs-lookup"><span data-stu-id="c9d2a-103">Service Decisions</span></span>

<span data-ttu-id="c9d2a-104">에 필수 구성 요소가 충족 되 면 및 설치 하기 전에 CLO365의 프로그램 구현 하는 방법에 대 한 다음과 같은 결정을 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-104">Once your pre-requisites are met and prior to installation you should make the following decisions about your implemenation of CLO365:</span></span>

1. <span data-ttu-id="c9d2a-105">**이미 있습니까 교육 포털 현대 인터페이스를 사용 하 여 회사에 있습니까?**</span><span class="sxs-lookup"><span data-stu-id="c9d2a-105">**Do you already have a training portal in your company with a modern interface?**</span></span>

- <span data-ttu-id="c9d2a-106">**예** 이러한 질문에 대 한 대답 ' 예 ' 인 경우 권장 되는 일련의 작업 이면 해당 기존 사이트 환경 내에서 [웹 파트를 설치](installwebpart.md) 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-106">**YES** If your answer to these questions are yes, then [installing the webpart](installwebpart.md) within that existing site experience is our recommended course of action.</span></span>
- <span data-ttu-id="c9d2a-p101">**아니요** 사용자가 응답 하면 하는 경우 없는 것이 좋습니다 [전체 사용자 정의 학습 사이트 설치](installsitepackage.md) 패키지를 합니다.  이 작업을 준비할 수 현대 SharePoint Online 통신 사이트와 하 여 최종 사용자에 게 중요 한 기타 정보를 포함할로 확장할 수 있습니다.  사이트 사용자 지정 웹 파트의 콘텐츠 업데이트를 가져올 수에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-p101">**NO** If you answer no we suggest [installing the full Custom Learning site](installsitepackage.md) package.  This will prepare you with a modern SharePoint Online communication site that your can expand to house other information that is important to your end users.  Customizing the site will not impact the webpart's ability to get content updates.</span></span> 

2. <span data-ttu-id="c9d2a-110">**Office 365 관리자 입니까?**</span><span class="sxs-lookup"><span data-stu-id="c9d2a-110">**Are you an Office 365 Administrator?**</span></span>

- <span data-ttu-id="c9d2a-111">**예**: 두 설치에 대 한 적절 한 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-111">**YES**:  You have the appropriate rights for either installation.</span></span>
- <span data-ttu-id="c9d2a-112">**NO**: 지원에 대 한 Office 365 관리자에 게 문의 하거나 소유 하 고 사이트 모음에 있는 웹 파트를 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-112">**NO**: Contact your Office 365 Administrator for assistance or install the webpart in a site collection you own</span></span>

3. <span data-ttu-id="c9d2a-113">**조직에서 공식 교육 부서 있습니까?**</span><span class="sxs-lookup"><span data-stu-id="c9d2a-113">**Do you have a formal training department in your organization?**</span></span>

- <span data-ttu-id="c9d2a-114">**예**: 하 게 참여할 하 고 추가, 사용자 지정 된 교육 콘텐츠를 제공 하기 위해 이러한 솔루션 사용 방법을 알려 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-114">**YES**:  Make sure to engage them and let them know how they can use these solutions to deliver additional, customized training content.</span></span>
- <span data-ttu-id="c9d2a-115">**NO**: 사용해 [셀프서비스 채택 키트 (영문)를](driveadoption.md) 사용 하 여 최종 사용자에 게는 사이트를 볼 수는 사용할 수를 인식 하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-115">**NO**:  Use our [self service adoption kit](driveadoption.md) to make your end-users aware the site is available to help them.</span></span>

4. <span data-ttu-id="c9d2a-116">**조직에서 사용자 커뮤니티에 있습니까?  이 라고도 power users 또는 서버만 자세한 내용을 보려면 관심 기술에 대 한 정보를 자세히 확인 하려면 사용자의 공식 / 비공식 그룹 중 하나 설치 해야 합니다.**</span><span class="sxs-lookup"><span data-stu-id="c9d2a-116">**Do you have a user community in your organization?  This would be either a formal or informal group of users who like to know more about technology, sometimes called power users or just those interested to learn more.**</span></span>

- <span data-ttu-id="c9d2a-117">**예**: 모든 기존 또는 새 사용자 커뮤니티 포럼에 대 한 링크를 제공 하려면 사용자 정의 학습 사이트 경험을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-117">**YES**:  You can use the Custom Learning site experience to provide links to any new or existing user community forums.</span></span>
- <span data-ttu-id="c9d2a-p102">**NO**: 사용자가 성공 공유 및를 서로 설명 수 있도록 내부 사용자 그룹을 시작 것이 좋습니다.  내부 사용자 그룹을 촉진 시키는 시간 하지 않을 경우 및 직원에 게 참여할 수 있습니다 월별 교육, 온라인 커뮤니티와 미리 액세스의 멤버 자격에 대 한 [Microosft Office 365 챔피언 커뮤니티](https://aka.ms/O365Champions) 도구와 리소스를 Office 365에 대 한.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-p102">**NO**:  Consider starting an internal user group so people can share their success and learn from each other.  If you don't have time to nurture an internal user group you and your employees can join the [Microosft Office 365 Champion community](https://aka.ms/O365Champions) for monthly training, membership in the online community and early access to tools and resources for Office 365.</span></span>

5.  <span data-ttu-id="c9d2a-120">**사이트 유지 관리 또는 지원 질문에 대 한 책임 될 수 있습니까?**</span><span class="sxs-lookup"><span data-stu-id="c9d2a-120">**Will you be accountable for site maintenance or support questions?**</span></span>

- <span data-ttu-id="c9d2a-p103">**예**: Office 365의 기능을 사용 하 여 쉽게 사이트 지원 학습 하는 사용자 정의 확인 하는 것이 좋습니다.  서비스 구독 및 조직의 크기에 따라 일부 역할을 하는:</span><span class="sxs-lookup"><span data-stu-id="c9d2a-p103">**YES**: We suggest using the capabilities of Office 365 to make Custom Learning site support easier.  Some ideas, depending on your service subscription and organization size are:</span></span>
    1. <span data-ttu-id="c9d2a-123">대규모 조직에는 공용 Yammer 커뮤니티에 참여 하는 사이트에 피드백을 받을 프로 비전 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-123">Large organizations can provision a public Yammer community to get feedback on the site</span></span>
    2. <span data-ttu-id="c9d2a-124">최대 2500 명까지 대화를 공유 하 고 질문을 Microsoft 팀에 참가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-124">Up to 2500 people can join a Microsoft Team to ask questions and share conversation</span></span>
    3. <span data-ttu-id="c9d2a-125">프로세스 티켓 공식 기술 지원에는 폼, 흐름와가 지원 될 수 있습니다 및 SharePoint Online 목록 또는 기타 타사를 통해 도구는 회사에서 IT 지원에 대 한 이미 있을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-125">A formal support ticketing process can be suppored with Forms, Flow and SharePoint Online lists or through other 3rd party tools which you may already have for IT support in your company.</span></span> 
- <span data-ttu-id="c9d2a-126">**NO**: SharePoint Online 지원을 제공 하는 IT 담당자와 사이트/웹 파트의 설치에 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-126">**NO**:  Discuss the installation of the site/webpart with your IT staff who provide SharePoint Online support.</span></span>  

## <a name="next-steps---siteinstallsitepackagemd-or-webpartinstallwebpartmd-installation"></a><span data-ttu-id="c9d2a-127">다음 단계- [사이트](installsitepackage.md) 또는 [웹 파트](installwebpart.md) 설치</span><span class="sxs-lookup"><span data-stu-id="c9d2a-127">Next Steps - [Site](installsitepackage.md) or [webpart](installwebpart.md) installation</span></span>