---
author: pkrebs
ms.author: pkrebs
title: 파트너 통합 모델
ms.date: 3/9/2019
description: 파트너 통합 모델
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: a91cdf4ee6aa3bbc22033dd484605ea5405b3c4c
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575993"
---
# <a name="partner-integration-models"></a>파트너 통합 모델
SharePoint Online Provisioning Service에서 직접 Microsoft 365 학습 경로 콘텐츠를 보완할 수 없는 경우 파트너가 활용할 수 있는 몇 가지 통합 모델이 있습니다. 위의 파트너 통합 모델은 복잡성과 투자 수준이 증가하는 순서로 표시됩니다. 따라서 당사의 지침은 비즈니스 모델을 기반으로 전문 지식을 구축하고 고급 수준으로 발전하는 것입니다.

![Flow 차트에는 활성화자, 통합자 및 재배포자 역할이 표시됩니다.](media/cg-part-intmodel.png)

## <a name="how-should-i-get-started"></a>어떻게 시작해야 하나요? 
시작을 위해 따라야 할 몇 가지 모범 사례는 다음과 같습니다.     

### <a name="1-begin-with-building-expertise-as-an-enabler"></a>1. 먼저 사용 가능으로 전문 지식을 구축합니다. 
학습 경로 교육 포털을 사용하도록 설정하고 대상 Microsoft 콘텐츠 큐레이터를 수행하여 고객 기반의 비율을 바로 지원할 수 있습니다. 학습 경로 프로비전에 대한 지침은 새 학습 경로 솔루션 프로비전을 [참조하세요.](/office365/customlearning/custom_provision)  

### <a name="2-then-extend-your-services-as-an-integrator"></a>2. 그런 다음 통합자로 서비스를 확장합니다.
콘텐츠 및/또는 서비스 통합 요구의 양에 따라 투자 분석에 대한 자동화 수익을 수행하세요. 예를 들어 유료 콘텐츠를 대상으로 하는 대상 사용자 지정 재생 목록을 빠르게 만들거나 서비스를 참조할 수 있는 경우 콘텐츠 통합 지침과 관련한 개발 및 운영 비용을 감당하는 것이 타당하지 않을 수 있습니다.

### <a name="3-when-the-return-on-investment-makes-sense--consider-redistribution"></a>3. 투자 수익률이 의미 있는 경우 – 재배포 고려 
투자 수익률이 의미 있는 경우 재배포(또는 관련 학습 경로 파트너와 작업)를 고려하여 다시 포장된 솔루션을 빌드합니다. 사용자 지정된 사이트를 추출한 다음 고객 환경에 배포하는 솔루션을 제공하는 SharePoint 패턴 및 연습 프레임워크를 기반으로 합니다. 

## <a name="partner-provided-content-integration-guidelines"></a>파트너 제공 콘텐츠 통합 지침
Microsoft 365 경로에 대한 콘텐츠는 학습 패키지의 콘텐츠 매니페스트 역할을 하는 JSON 파일 집합을 통해 구동됩니다. 세 개의 파일이 있습니다. metadata.js, playlists.js및 assets.js있습니다. 이러한 파일은 웹 파트가 인식하는 모델과 일치하도록 구성한 다음 웹 파트가 로드될 수 있도록 콘텐츠 배달 네트워크(CDN)에서 호스팅해야 합니다. Microsoft는 사용자가 시작할 수 있는 이러한 파일의 시작 서식 파일을 제공합니다.  

**고지 사항:** JSON 파일 구조는 예정된 솔루션 작동에 따라 변경될 수 있습니다. 이 Microsoft 365 학습 경로 파트너 EAP(Early Adopter Program)는 이러한 특성의 임박한 변경에 대해 알릴 것입니다. 모든 고객 전과의 호환성 및/또는 전환 지침과 함께 

### <a name="download-the-microsoft-365-learning-pathways-solution"></a>학습 Microsoft 365 솔루션 다운로드
JSON 파일과 함께 Microsoft 365 학습 경로 솔루션을 다운로드할 수 GitHub https://github.com/pnp/custom-learning-office-365 있습니다. 현재 Microsoft는 솔루션에서 GitHub 끌어오기 요청을 처리하지 않습니다. 그러나 사용자 지정 GitHub 만들기 위한 시작점으로 파일 파일을 사용할 수 있습니다. 

### <a name="metadatajson-structure"></a>Metadata.js대한 구성
이 파일을 메뉴 및 구조의 브레인으로 생각할 수 있습니다. 다른 두 파일의 데이터에 대한 선택 목록뿐만 아니라 모든 탐색 구조가 포함되어 있습니다. 


|              이름        |                     설명                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|**기술**              |콘텐츠에 태그가 지정되어 할당된 기술에 따라 숨길 수 있습니다.                 |  
|&nbsp;&nbsp;Id                |기술을 나타내는 GUID                                                           |  
|&nbsp;&nbsp;이름              |기술의 표시 이름                                                             |
|&nbsp;&nbsp;*Subjects[ ]*     |기술의 하위 집합인 주제의 배열                                   | 
|&nbsp;&nbsp;&nbsp;&nbsp;Id    |제목을 나타내는 GUID                                                              |
|&nbsp;&nbsp;&nbsp;&nbsp;이름  |제목의 표시 이름                                                                |
|**Categories [ ]**             |범주는 웹 항목의 탐색을 알 수 있습니다. 각 범주는 탐색의 최상위 수준을 나타 내는 항목입니다.                                                                                                                 |
|&nbsp;&nbsp;Id                |범주/하위 범주를 나타내는 GUID                                                 |
|&nbsp;&nbsp;이름              |범주/하위 범주의 표시 이름                                                  |
|&nbsp;&nbsp;이미지             |UX에 표시해야 하는 이미지의 URL(UX 기준CDN 기준)            |
|&nbsp;&nbsp;TechnologyId      |이 콘텐츠와 관련된 기술의 GUID(선택 사항 - 빈 문자열)            |
|&nbsp;&nbsp;SubjectId         |제목 이 콘텐츠의 GUID(선택 사항 - 빈 문자열)와 관련이 있습니다.               |
|&nbsp;&nbsp;원본            |원본 배열에서 사용자가 추가한 사용자 지정 데이터가 아닌 UX에서 특별히 사용되지 않는 배열은 "테넌트"로 표시되어 있으며 UX 관리 영역은 "테넌트"로 표시된 모든 것을 편집할 수 없습니다.                           |
|&nbsp;&nbsp;*하위categories[ ]*|Sub-Categories 수준은 기본적으로 수준 2의 내비게이트 수준입니다. 구조는 방금 중첩된 Category와 동일합니다.          |
|**대상[ ]**             |범주/하위 범주와 연결된 재생 목록이 태그가 지정되는 다양한 대상이면 선택기에서 사용 가능한 대상을 표시하는 데 사용할 수 있습니다. |         
|&nbsp;&nbsp;Id                |대상의 GUID                                                                       |  
|&nbsp;&nbsp;이름              |대상의 표시 이름                                                               |       
|**Sources [ ]**               |사용자가 추가한 사용자 지정 데이터가 아닌 특별히 UX에서 사용되지 않는 원본으로 콘텐츠에 태그를 지정하는 문자열 배열은 "테넌트"로 표시되어 있으며 UX 관리 영역은 "테넌트"로 표시된 모든 내용을 편집할 수 없습니다.                                                   |  
|**수준 [ ]**               |범주/하위 범주와 연결된 재생 목록이 다양한 수준 태그가 지정되는 경우 선택기에서 사용 가능한 수준을 표시하는 데 사용할 수 있습니다.             |  
|&nbsp;&nbsp;Id                |수준 GUID                                                                          |  
|&nbsp;&nbsp;이름              |수준 표시 이름                                                                  | 
|**StatusTag [ ]**           |상태 태그는 UX에 노출될 다양한 상태의 콘텐츠를 식별하는 것입니다. 이러한 플래그 중 일부는 소비자에게 표시하고 일부는 관리자에게만 표시됩니다.                                                   |  
|&nbsp;&nbsp;Id                |StatugTag의 GUID                                                                      |  
|&nbsp;&nbsp;이름              |StatusTag의 표시 이름                                                              | 
|**원격 분석 [ ]**            |                                                                                           |  
|&nbsp;&nbsp;AppInsightsKey    |뷰어 웹 파트의 로드를 추적하기 위해 설정한 앱 인사이트 키의 GUID입니다. 관리자가 전체 테넌트에 대한 추적을 해제할 수 있지만, 전송된 정보는 테넌트 ID가 있는 사용자가 비동기화됩니다. 자세한 내용은 이 섹션을 참조하세요. https://github.com/pnp/custom-learning-office-365#disabling-telemetry-collection               |  
|**버전**                   |버전 정보는 솔루션에서 웹 텐트가 업데이트된 것을 관리자에게 나타내고 중요한 변경 사항이 있는 경우 웹 사이트에서 사용자 지정 콘텐츠를 최신 버전의 매니페스트로 자체 업데이트하도록 허용하는 데 사용됩니다.         | 
|&nbsp;&nbsp;매니페스트          |매니페스트의 버전                                               |
|&nbsp;&nbsp;ManifestMinWebPart|매니페스트 버전에서 작동하는 웹 버전의 최소 버전             |
|&nbsp;&nbsp;CurrentWebPart    |UX에 표시해야 하는 이미지의 URL(UX 기준CDN 기준)            |
|&nbsp;&nbsp;RepoURL           |웹 파트 업데이트 지침이 있는 리포지토리의 URL입니다.                    |
|**콘텐츠 팩**             |현재 추가 콘텐츠 CDN 팩은 지원되지 않습니다. Microsoft는 콘텐츠 팩을 통해 M365LP를 활용하여 콘텐츠를 전달하고 자체적으로 사용자 지정 CDNS에 있는 프로비저닝 서비스를 통해 프로비전할 수 있는 다른 Microsoft에서 만든 솔루션을 제안할 수 있습니다.       | 
|&nbsp;&nbsp;Id                |콘텐츠 팩/콘텐츠 팩의 CDN                                                              |
|&nbsp;&nbsp;이름              |화면 표시 CDN                                                                   |
|&nbsp;&nbsp;설명       |콘텐츠 팩을 추가하기 위해 UI에 표시할 설명                               |
|&nbsp;&nbsp;이미지             |콘텐츠 팩을 추가하기 위해 UI에 표시할 이미지                                     |
|&nbsp;&nbsp;ProvisionURL      |콘텐츠 팩의 사이트 모음을 만드는 프로비저닝 서비스 패키지의 URL입니다.  |
|&nbsp;&nbsp;CDNbase           |콘텐츠 팩에 대한 매니페스트의 기본 URL                                       |
|AssetOrigins                  |나중에 설명하는 파일에서 URL assets.js배열입니다. 원본 URL이 지원되는 경우 게시 메시지가 help_getClientHeight. "help_getClientHeight={height of content}"(예: "help_getClientHeight=5769")의 데이터 속성에 응답하면 iFrame의 적절한 높이를 프레임 콘텐츠의 적절한 높이로 조절할 수 있습니다.         |

### <a name="playlistsjson-structure"></a>Playlists.js대한 구성
playlists.js- 재생 목록 매니페스트는 재생 목록에 포함된 자산 및 재생 목록에 대한 메타데이터를 설명하는 개체의 배열입니다.

|              이름        |                     설명                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |재생 목록을 나타내는 GUID                                                             |  
|제목                         |재생 목록의 표시 이름                                                               |
|이미지                         |재생 목록을 시각화하기 위한 이미지에 대한 상대 URL(CDN)                              |                      
|LevelId                       |연결된 수준                                                                           |
|AudienceId                   |연결된 대상                                                                        |
|TechnologyId                 |관련 기술                                                                      |
|SubjectId                    |범주/하위 범주의 표시 이름                                                  |
|원본                        |원본 배열에서 사용자가 추가한 사용자 지정 데이터가 아닌 UX에서 특별히 사용되지 않는 경우 "테넌트"로 표시되어 있으며 UX 관리 영역은 "테넌트"로 표시된 모든 것을 편집할 수 없습니다.                                              |
|CatId                         |재생 목록이 표시될 컨테이너를 나타내는 Category 또는 SubCategory ID입니다. 현재 매니페스트는 SubCategory 하위 항목도 있는 경우 범주 또는 하위 범주를 컨테이너로 선택할 수 없습니다.        |
|설명                   |UX의 각 재생 목록에 대해 설명이 표시                                           |
|StatusTagId                   |연결된 상태 태그                                                                      |
|StatusNote                    |관리자에게 표시되는 콘텐츠에 대한 참고 사항                                            |
|*자산[]*                        |이 재생 목록의 일부인 자산에 대한 GUID 배열(표시 순서)입니다.        |         

### <a name="assetjson-structure"></a>Asset.js대한 구성
playlists.js- 재생 목록 매니페스트는 재생 목록에 포함된 자산 및 재생 목록에 대한 메타데이터를 설명하는 개체의 배열입니다.

|              이름        |                     설명                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |재생 목록을 나타내는 GUID                                                             |  
|제목                         |재생 목록의 표시 이름                                                               |
|설명                   |---                                                                                           |                      
|URL                           |iFrame에 적용할 자산의 원본 URL입니다.                                  |
|TechnologyId                  |관련 기술                                                                      |
|SubjectId                     |관련 주체                                                                         |
|원본                        |범주/하위 범주의 표시 이름                                                  |
|StatusTagId                   |연결된 상태 태그                                                                      |
|StatusNote                    |관리자에게 표시되는 콘텐츠에 대한 참고 사항                                           |

### <a name="caching"></a>캐싱
뷰어 웹 파트의 현재 버전은 24시간 동안 캐시된 버전의 매니페스트 파일을 활용합니다. 24시간이 지난 후 웹 팀에 처음 방문한 사용자는 원본 웹 사이트에서 매니페스트를 다운로드하여 캐시를 새로 고치고 CDN 숨겨진 기술 및 재생 목록과 병합하고 사용자 지정 하위 범주, 재생 목록 및 자산의 병합을 통해 캐시를 새로 고칠 수 있습니다. 또는 관리자 웹 파트는 항상 매니페스트에서 콘텐츠를 다운로드하여 병합하고 캐시를 업데이트합니다.  따라서 즉, 관리자는 관리 웹 파트를 로드하여 관리 페이지로 이동하여 캐시 업데이트를 강제할 수 있습니다.

## <a name="content-pack-guidelines"></a>콘텐츠 팩 지침
콘텐츠 팩 기능은 다음과 같은 시나리오의 잠금을 해제합니다.
- 파트너가 고객의 환경에 맞게 사용자 지정한 부가 가치의 사용자 지정 학습 콘텐츠를 재배포할 수 있는 능력
- 강력한 교육 팀 및 IT 지원이 있는 조직이 자체 내부 시스템 및 거버넌스를 위한 사용자 지정 학습 콘텐츠를 빌드할 수 있는 능력
- Microsoft가 고객이 옵트인할 수 있는 향후 추가 학습 경로를 제공할 수 있는 능력

이 현재 문서 집합은 기능의 복잡도로 인해 파트너를 대상으로 의도적으로 지정됩니다. 서비스 팀은 향후 시나리오를 보다 잘 지원하고 사용하도록 #2 적극적으로 작업하고 있습니다. 

### <a name="how-content-packs-work"></a>콘텐츠 팩 작동 방식
Microsoft는 매니페스트 GitHub 이미지에 대한 Content Delivery Network(CDN) 원본으로 CDN 페이지를 활용합니다. 매니페스트 파일의 각 버전에 대한 하위 폴더를 포함하는 GitHub 저장소의 루트에 문서 폴더가 있습니다. 각 폴더에는 세 개의 매니페스트 파일과 모든 범주, 하위 범주 및 재생 목록 이미지를 저장하는 이미지 폴더가 있습니다. 

자체 콘텐츠 팩을 통해 학습 경로 솔루션을 확장하기로 선택한 경우 Microsoft와 동일한 버전 관리 구조를 유지해야 합니다. 웹 파트가 CDN 버전이 지원되는 매니페스트 버전이 버전 폴더에 추가되고 해당 url에 자동으로 추가되어 CDN 없습니다. 매니페스트 파일을 개정할 때 매니페스트 파일의 새 인스턴스를 만들 시간을 줄 것입니다.

![Screenshot shows sample structure.](media/cg-part-json-folder.png) 

원본으로 GitHub 페이지를 활용하는 CDN 도움말 설명서를 [https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages) 참조하세요. .

Microsoft의 솔루션은 이러한 파일에 액세스할 수 있는 사용자에 대한 보안이 없는 자산에 대한 정보를 일반에게 공개합니다. 소비자를 위한 무료 콘텐츠 계층이 있을 것으로 생각됩니다. 즉, 콘텐츠의 일부 또는 전체에 대해 급여를 지불해야 하는 경우 솔루션의 기술적 제한 내에서 이를 다르게 구현해야 한다고 말하며 GitHub 페이지를 사용하는 것은 요구 사항이 아닙니다. 사용 CDN 버전 번호 매기기 구조를 유지 관리하는 경우 사용할 모든 사용자 공급자가 괜찮습니다. 앞서 설명한 것 처럼 웹 파트가 지원하는 매니페스트 구조의 버전이 코드에 구워지며 웹 파트 URL에 CDN 추가됩니다. 

### <a name="content-pack-integration-guidance"></a>콘텐츠 팩 통합 지침 
사용자가 테넌트에서 추가 CDN 끝점을 구성할 수 있도록 관리자 및 뷰어 웹 파트가 확장되어 뷰어 웹 파트가 표시할 데이터를 CDN 수 있습니다. 

이 기능에 유의해야 하는 주요 프레이밍: 
- 수동 재생 목록 구성이 너무 번거로우는 파트너 재배포 시나리오에 기본 적용될 수 있습니다. 
- 사용자 지정 콘텐츠 팩은 고급 기능으로, 웹 콘텐츠를 관리한 경험이 있는 파트너만 사용할 수 있습니다. 신뢰할 수 없는 콘텐츠 원본이 사이트에 안전하지 않은 콘텐츠를 도입할 수 있습니다. 신뢰할 수 있는 원본만 추가해야 합니다.

> **중요** 사용자 지정 콘텐츠 팩을 추가하기 전에 학습 경로 3.0 Microsoft 365 프로비전해야 합니다. 학습 경로 프로비전에 대한 Microsoft 365 자세한 내용은 프로비전 Microsoft 365 [참조합니다.](./custom_provision.md)

### <a name="content-whitelisting"></a>콘텐츠 화이트리스트
파트너는 소비자가 해당 환경에서 콘텐츠가 화이트리스트에 추가된 것을 지원할 책임이 있습니다. 해당 환경에서 콘텐츠가 방화벽 내부의 SharePoint 수 있는지 검사하는 테스트 시나리오를 만드는 것이 좋습니다. 사용자 지정 [SharePoint](./custom_createnewpage.md) 페이지 만들기 지침에 따라 이 경우를 확인할 수 있습니다.

### <a name="add-a-content-pack-to-learning-pathways"></a>학습 경로에 콘텐츠 팩 추가
JSON을 수정하고 사용자 정의한 CDN 학습 경로에 연락처 팩을 추가할 수 있습니다. 

1. 학습 경로 사이트 **홈 페이지에서** 홈을  클릭한 다음 학습 경로 **관리 를 클릭합니다.** 
2. 관리 **페이지에서** ... **페이지의 오른쪽 위** 모서리에 콘텐츠 팩을 추가합니다.
3. 사용자 지정 콘텐츠 팩을 클릭한 다음 콘텐츠 팩의 이름을 입력한 다음 JSON CDN 위치를 지정합니다.

   ![이름과 경로를 입력하는 화면입니다.](media/cg-part-addconpack.png)

4. **저장** 을 클릭합니다. 이제 사용자 지정 콘텐츠 팩의 콘텐츠가 관리 페이지에 표시됩니다. 예를 들면 다음과 같습니다. 

   ![관리 페이지 예제입니다.](media/cg-part-addconpackex.png)

### <a name="filter-to-the-content-pack-in-the-web-part"></a>웹 파트의 콘텐츠 팩으로 필터링
학습 경로를 사용하여 학습 경로 웹 파트를 페이지에 추가하고, 웹 파트를 필터링하여 사용자 지정 콘텐츠 팩 원본을 지정한 다음 웹 파트를 원하는 범주, 하위 범주, 재생 목록 및 자산으로 필터링할 수 있습니다. 

1. 학습 경로 사이트에서 새로 고치고 페이지를 **클릭합니다.** 
2. 비어 **있는** 를 클릭한 다음 페이지 **만들기 를 클릭합니다.**
3. 페이지에 이름을 지정합니다. 
4. + **페이지 왼쪽에** 있는 새 섹션 추가를 클릭합니다.
5. 새 섹션의 위쪽을 클릭한 다음 학습 경로 웹 Microsoft 365 **+** **추가합니다.**
6. 웹 파트를 클릭한 다음 편집 **아이콘을** 클릭합니다.
7. 학습 **원본 선택 상자에서** 사용자 지정 콘텐츠 팩을 선택한 다음 웹 파트를 원하는 콘텐츠로 필터링합니다. 다음은 사용자 지정 콘텐츠 팩의 재생 목록으로 필터링된 웹 파트의 예를 제공하는 예제입니다.

   ![사용자 지정 콘텐츠 팩의 재생 목록으로 필터링된 샘플 웹 파트의 스크린샷](media/cg-part-conpackfilter.png)