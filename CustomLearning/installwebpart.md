# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="3e6c0-101">학습 솔루션 웹 파트 사용자 지정 설치</span><span class="sxs-lookup"><span data-stu-id="3e6c0-101">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="3e6c0-102">테 넌 트 전체 설치를 위한 필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="3e6c0-102">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="3e6c0-p101">전체 테 넌 트에 대 한 사용자 정의 학습 웹 파트를 설치 하려면 Office 365 관리 권한을 갖도록 해야 합니다.  이러한 사용 권한은 Office 365 관리자와 함께 작업 하 또는 개별 사이트 모음에 대 한 웹 파트를 설치 하지 않아도 하는 경우 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="3e6c0-105">또는 Office 365 관리자가 설치 되어 있어야 하 고 [앱 카탈로그](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) 테 넌 트 수준 또는 [사이트 모음 앱 카탈로그](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)웹 파트를 수신 하도록 구성 된.]</span><span class="sxs-lookup"><span data-stu-id="3e6c0-105">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="3e6c0-p102">SharePoint Online만 지원 합니다. 웹 파트의 SharePoint 온-프레미스 버전을 설치 하는 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="3e6c0-108">테 넌 트에 사용자 정의 학습 웹 파트 추가</span><span class="sxs-lookup"><span data-stu-id="3e6c0-108">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="3e6c0-p103">사용자 정의 학습 웹 파트를 다운로드 하 고 로컬 드라이브에 저장 합니다.  이 파일을 "ms-사용자 정의-learning.sppkg" 라고 합니다.  이름 또는 파일의 접미사를 변경 하지 마십시오.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="3e6c0-112">테 넌 트에 대 한 [Office 365 관리 포털](https://admin.microsoft.com/AdminPortal/Home#/homepage) 탐색</span><span class="sxs-lookup"><span data-stu-id="3e6c0-112">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="3e6c0-p104">왼쪽된 탐색 모음에서 SharePoint를 관리 센터를 선택 합니다. 새 탭, SharePoint 관리 센터에서 select 앱, 앱 카탈로그, SharePoint 용 앱의 열립니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="3e6c0-115">웹 파트를 업로드 하 고 다운로드 한 "ms-사용자 정의-learning.sppkg" 파일을 선택 하는 선택</span><span class="sxs-lookup"><span data-stu-id="3e6c0-115">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="3e6c0-116">이 테 넌 트 수준의 설치에 대 한 "만들기가이 솔루션은 조직에서 모든 배치 된 위치의를 사용할 수 있습니다." 옆에 있는 상자를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-116">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  

![솔루션 배포](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="3e6c0-118">SharePoint Online 페이지에 고객 학습 웹 파트 추가</span><span class="sxs-lookup"><span data-stu-id="3e6c0-118">Add the Customer Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="3e6c0-p105">테 넌 트에 사용자 지정 학습을 설치한 후에 SharePoint 페이지에 웹 파트를 추가할 수 있습니다. 이렇게 전환 하면가 갑자기 Office 365 교육은을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-p105">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do, suddenly Office 365 training is available to you.</span></span> 

1. <span data-ttu-id="3e6c0-121">전체 너비 열 레이아웃에 사용자 정의 학습 웹 파트를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-121">Add the Custom Learning webpart in a full width column layout:</span></span>

![SharePoint 페이지 레이아웃](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="3e6c0-p106">SharePoint 페이지에 추가 섹션을 선택 하 고 전체 너비 열을 선택 합니다.  다음과 같은 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-p106">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="3e6c0-p107">Microsoft Learning를 선택 합니다.  다음은 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-p107">Select Microsoft Learning.  You should now see the following:</span></span> 

![사용자 지정 웹 파트를 학습](media/clo365addwebpart.png)

 <span data-ttu-id="3e6c0-129">솔루션에 포함 된 기본 콘텐츠를 탐색 하려면 타일에서을 클릭할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-129">You can now click on the tiles to explore the default content included in the solution.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="3e6c0-130">다음 단계</span><span class="sxs-lookup"><span data-stu-id="3e6c0-130">Next Steps</span></span>
- <span data-ttu-id="3e6c0-131">웹 파트에 포함 된 [기본 콘텐츠](webpartcontent.md) 를 탐색 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-131">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="3e6c0-132">[사용자 지정](customization.md) 하면 조직에 대 한 교육 경험 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-132">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="3e6c0-133">교육 솔루션의 [채택 드라이브](driveadoption.md) 를 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e6c0-133">[Drive adoption](driveadoption.md) of your training solution.</span></span>

