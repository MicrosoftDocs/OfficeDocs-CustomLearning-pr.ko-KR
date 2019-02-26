---
author: karuanag
ms.author: karuanag
title: 필수 구성 요소 및 결정 사항
ms.date: 02/10/2019
description: 사용자 지정 학습 설치 및 설정에 대 한 결정 및 필수 구성 요소 정보
ms.openlocfilehash: b498ba308a87cad7000a041676feeac44326d327
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989709"
---
## <a name="service-decisions"></a><span data-ttu-id="fe44b-103">서비스 결정 사항</span><span class="sxs-lookup"><span data-stu-id="fe44b-103">Service Decisions</span></span>

<span data-ttu-id="fe44b-104">필수 구성 요소를 충족 하 고 설치 하기 전에 implemenation에 대 한 다음과 같은 결정을 내려야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-104">Once your pre-requisites are met and prior to installation you should make the following decisions about your implemenation of CLO365:</span></span>

1. <span data-ttu-id="fe44b-105">**최신 인터페이스가 있는 회사의 교육 포털이 이미 있습니까?**</span><span class="sxs-lookup"><span data-stu-id="fe44b-105">**Do you already have a training portal in your company with a modern interface?**</span></span>

- <span data-ttu-id="fe44b-106">**예** 이러한 질문에 대 한 답이 예 이면 해당 기존 사이트 환경 내에서 [웹 파트를 설치](installwebpart.md) 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-106">**YES** If your answer to these questions are yes, then [installing the webpart](installwebpart.md) within that existing site experience is our recommended course of action.</span></span>
- <span data-ttu-id="fe44b-p101">**아니요** 응답 하지 않으면 [전체 사용자 지정 학습 사이트 패키지를 설치 하는](installsitepackage.md) 것이 좋습니다.  이렇게 하면 최종 사용자에 게 중요 한 정보를 포함 하기 위해 확장할 수 있는 최신 SharePoint Online 통신 사이트가 준비 됩니다.  사이트를 사용자 지정 해도 웹 파트는 콘텐츠 업데이트를 가져오는 기능에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-p101">**NO** If you answer no we suggest [installing the full Custom Learning site](installsitepackage.md) package.  This will prepare you with a modern SharePoint Online communication site that your can expand to house other information that is important to your end users.  Customizing the site will not impact the webpart's ability to get content updates.</span></span> 

2. <span data-ttu-id="fe44b-110">**Office 365 관리자 인가요?**</span><span class="sxs-lookup"><span data-stu-id="fe44b-110">**Are you an Office 365 Administrator?**</span></span>

- <span data-ttu-id="fe44b-111">**예**: 설치에 대 한 적절 한 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-111">**YES**:  You have the appropriate rights for either installation.</span></span>
- <span data-ttu-id="fe44b-112">**NO**: 사용자가 소유한 사이트 모음에 Office 365 관리자에 게 문의 하거나 웹 파트를 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-112">**NO**: Contact your Office 365 Administrator for assistance or install the webpart in a site collection you own</span></span>

3. <span data-ttu-id="fe44b-113">**조직에 공식적인 교육 부서가 있습니까?**</span><span class="sxs-lookup"><span data-stu-id="fe44b-113">**Do you have a formal training department in your organization?**</span></span>

- <span data-ttu-id="fe44b-114">**예**: 이러한 솔루션을 사용 하 여 사용자 지정 된 추가 교육 콘텐츠를 제공 하는 방법을 알려 주십시오.</span><span class="sxs-lookup"><span data-stu-id="fe44b-114">**YES**:  Make sure to engage them and let them know how they can use these solutions to deliver additional, customized training content.</span></span>
- <span data-ttu-id="fe44b-115">**NO**: [셀프 서비스 채택 키트](driveadoption.md) 를 사용 하 여 최종 사용자가 사이트를 도울 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-115">**NO**:  Use our [self service adoption kit](driveadoption.md) to make your end-users aware the site is available to help them.</span></span>

4. <span data-ttu-id="fe44b-116">**조직에 사용자 커뮤니티가 있습니까?  이는 기술에 대 한 자세한 정보 (예를 들어, power users 또는 자세히 알고자 하는 사용자)에 대해 자세히 알아볼 수 있는 공식적인 사용자나 비공식적인 그룹 중 하나입니다.**</span><span class="sxs-lookup"><span data-stu-id="fe44b-116">**Do you have a user community in your organization?  This would be either a formal or informal group of users who like to know more about technology, sometimes called power users or just those interested to learn more.**</span></span>

- <span data-ttu-id="fe44b-117">**예**: 사용자 지정 학습 사이트 환경을 사용 하 여 새 또는 기존 사용자 커뮤니티 포럼에 대 한 링크를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-117">**YES**:  You can use the Custom Learning site experience to provide links to any new or existing user community forums.</span></span>
- <span data-ttu-id="fe44b-p102">**NO**: 사용자가 자신의 성공을 공유 하 고 서로 정보를 공유할 수 있도록 내부 사용자 그룹을 시작 하는 것이 좋습니다.  내부 사용자 그룹을 nurture 할 시간이 없는 경우 직원은 월별 교육을 위해 [마이크로 osft Office 365 챔피언 커뮤니티](https://aka.ms/O365Champions) 에 참가 하 고, 온라인 커뮤니티의 멤버 자격과 Office 365 용 도구 및 리소스에 대 한 초기 액세스 권한을 부여할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-p102">**NO**:  Consider starting an internal user group so people can share their success and learn from each other.  If you don't have time to nurture an internal user group you and your employees can join the [Microosft Office 365 Champion community](https://aka.ms/O365Champions) for monthly training, membership in the online community and early access to tools and resources for Office 365.</span></span>

5.  <span data-ttu-id="fe44b-120">**사이트 유지 관리 또는 지원 관련 질문에 대 한 책임을 야 하나요?**</span><span class="sxs-lookup"><span data-stu-id="fe44b-120">**Will you be accountable for site maintenance or support questions?**</span></span>

- <span data-ttu-id="fe44b-p103">**예**: 사용자 지정 학습 사이트 지원을 보다 쉽게 만들기 위해 Office 365의 기능을 사용 하는 것이 좋습니다.  서비스 구독 및 조직 크기에 따라 다음과 같은 몇 가지 아이디어가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-p103">**YES**: We suggest using the capabilities of Office 365 to make Custom Learning site support easier.  Some ideas, depending on your service subscription and organization size are:</span></span>
    1. <span data-ttu-id="fe44b-123">대규모 조직에서는 공개 Yammer 커뮤니티를 프로 비전 하 여 사이트에 대 한 의견을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-123">Large organizations can provision a public Yammer community to get feedback on the site</span></span>
    2. <span data-ttu-id="fe44b-124">Microsoft 팀에 참가 하 여 질문을 하 고 대화를 공유할 수 있는 최대 2500 명의 사용자</span><span class="sxs-lookup"><span data-stu-id="fe44b-124">Up to 2500 people can join a Microsoft Team to ask questions and share conversation</span></span>
    3. <span data-ttu-id="fe44b-125">공식적인 지원 티켓 프로세스는 양식, 흐름, SharePoint Online 목록 또는 회사에서 이미 IT 지원을 받을 수 있는 다른 타사 도구를 사용 하 여 suppored 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-125">A formal support ticketing process can be suppored with Forms, Flow and SharePoint Online lists or through other 3rd party tools which you may already have for IT support in your company.</span></span> 
- <span data-ttu-id="fe44b-126">**NO**: SharePoint Online 지원을 제공 하는 IT 직원과 사이트/웹 파트의 설치에 대해 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe44b-126">**NO**:  Discuss the installation of the site/webpart with your IT staff who provide SharePoint Online support.</span></span>  

### <a name="next-steps---site-provisioninginstallsitepackagemd-or-webpartinstallwebpartmd-installation-steps"></a><span data-ttu-id="fe44b-127">다음 단계- [사이트 프로 비전](installsitepackage.md) 또는 [웹 파트](installwebpart.md) 설치 단계</span><span class="sxs-lookup"><span data-stu-id="fe44b-127">Next Steps - [Site Provisioning](installsitepackage.md) or [webpart](installwebpart.md) installation steps</span></span>