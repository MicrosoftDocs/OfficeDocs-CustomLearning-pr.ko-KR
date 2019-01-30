# <a name="installing-the-custom-learning-solution-webpart"></a>학습 솔루션 웹 파트 사용자 지정 설치

## <a name="prerequisites-for-a-tenant-wide-installation"></a>테 넌 트 전체 설치를 위한 필수 구성 요소

- 전체 테 넌 트에 대 한 사용자 정의 학습 웹 파트를 설치 하려면 Office 365 관리 권한을 갖도록 해야 합니다.  이러한 사용 권한은 Office 365 관리자와 함께 작업 하 또는 개별 사이트 모음에 대 한 웹 파트를 설치 하지 않아도 하는 경우 됩니다.
- 또는 Office 365 관리자가 설치 되어 있어야 하 고 [앱 카탈로그](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) 테 넌 트 수준 또는 [사이트 모음 앱 카탈로그](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)웹 파트를 수신 하도록 구성 된.]
- SharePoint Online만 지원 합니다. 웹 파트의 SharePoint 온-프레미스 버전을 설치 하는 지원 되지 않습니다.

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>테 넌 트에 사용자 정의 학습 웹 파트 추가 

1. 사용자 정의 학습 웹 파트를 다운로드 하 고 로컬 드라이브에 저장 합니다.  이 파일을 "ms-사용자 정의-learning.sppkg" 라고 합니다.  이름 또는 파일의 접미사를 변경 하지 마십시오. 
2. 테 넌 트에 대 한 [Office 365 관리 포털](https://admin.microsoft.com/AdminPortal/Home#/homepage) 탐색
3. 왼쪽된 탐색 모음에서 SharePoint를 관리 센터를 선택 합니다. 새 탭, SharePoint 관리 센터에서 select 앱, 앱 카탈로그, SharePoint 용 앱의 열립니다. 
4. 웹 파트를 업로드 하 고 다운로드 한 "ms-사용자 정의-learning.sppkg" 파일을 선택 하는 선택
5. 이 테 넌 트 수준의 설치에 대 한 "만들기가이 솔루션은 조직에서 모든 배치 된 위치의를 사용할 수 있습니다." 옆에 있는 상자를 선택 합니다.  

![솔루션 배포](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a>SharePoint Online 페이지에 고객 학습 웹 파트 추가

테 넌 트에 사용자 지정 학습을 설치한 후에 SharePoint 페이지에 웹 파트를 추가할 수 있습니다. 이렇게 전환 하면가 갑자기 Office 365 교육은을 사용할 수 있습니다. 

1. 전체 너비 열 레이아웃에 사용자 정의 학습 웹 파트를 추가 합니다.

![SharePoint 페이지 레이아웃](media/clo365fullcolumnwidth.png)

2. SharePoint 페이지에 추가 섹션을 선택 하 고 전체 너비 열을 선택 합니다.  다음과 같은 메시지가 표시 됩니다.

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. Microsoft Learning를 선택 합니다.  다음은 표시 됩니다. 

![사용자 지정 웹 파트를 학습](media/clo365addwebpart.png)

 솔루션에 포함 된 기본 콘텐츠를 탐색 하려면 타일에서을 클릭할 수 있습니다.  

## <a name="next-steps"></a>다음 단계
- 웹 파트에 포함 된 [기본 콘텐츠](webpartcontent.md) 를 탐색 합니다.
- [사용자 지정](customization.md) 하면 조직에 대 한 교육 경험 합니다.
- 교육 솔루션의 [채택 드라이브](driveadoption.md) 를 합니다.

