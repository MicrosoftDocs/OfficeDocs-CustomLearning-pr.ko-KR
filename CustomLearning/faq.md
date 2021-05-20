---
title: Microsoft 365 경로 FAQ
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: 학습 경로에 대한 Microsoft 365 질문과 대답 정보
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: f24f16455ba41724d300d038a01dc04c2170dc4a
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575923"
---
# <a name="frequently-asked-questions"></a>질문과 대답

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>최근에 사용자 지정 학습용 사용자 지정 학습이 Office 365 경로로 Microsoft 365 블로그 게시물을 보했습니다. 이름 변경의 일환으로 솔루션에 추가되는 다른 변경 사항이 있나요? 조직에서 솔루션을 업데이트해야 하나요?

이 Microsoft 365 학습 경로 릴리스는 솔루션의 이름을 변경하여 사용자 브랜드에 맞게 변경하는 데 전념하는 Microsoft 365 있습니다. 조직에서 현재 Office 365 사용자 지정 학습이 있는 경우 현재 솔루션을 업데이트할 필요가 없습니다.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>테넌트 환경에 학습 Microsoft 365 설치하기 위한 요구 사항은 무엇입니까?

- SharePoint Online 및 커뮤니케이션 사이트를 사용할 수 있습니다.
- CLO365를 프로비전할 개인은 설치할 대상 테넌트의 테넌트 관리자 되어야 합니다.
- 테넌트 '앱 카탈로그'는 관리 센터의 '앱' 옵션 내에서 사용할 SharePoint 있어야 합니다.
- 새 앱 카탈로그를 만들 경우 앱 카탈로그를 완전히 프로비전하려면 30분 이상의 대기 시간이 필요합니다. 테넌트 Microsoft 365 바로 학습 경로를 프로비전하려고 하면 학습 경로 솔루션의 프로비전 오류가 발생합니다. 
- CLO365를 프로비전할 개인은 설치할 대상 테넌트에서 앱 카탈로그의 사이트 모음 관리자 되어야 합니다.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Microsoft에서 학습 경로를 설치할 때 테넌트 권한을 Microsoft 365 이유 

- SharePoint Online Provisioning Service는 사용 권한을 사용하여 학습 경로 SharePoint 사이트를 프로비전하고, 사이트의 페이지를 만들고, 테넌트 내에 Microsoft 365 학습 경로 응용 프로그램을 설치합니다. 그 이유는 사용 권한을 요청하는 유일한 이유입니다. 요청된 권한이 없는 경우 SharePoint 프로비전 서비스는 학습 경로 사이트 서식 파일 및 웹 파트를 자동으로 설치하는 명령을 실행할 수 없습니다. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>베타 미리 보기를 Microsoft 365 학습 경로의 의미는 무엇입니까? 

Microsoft 365 학습 경로는 현재 Beta Preview에 있습니다. 학습 경로를 평가, 계획 및 구현할 때 Microsoft 365 고려합니다.

- 모든 베타 솔루션과 함께 서비스 관리 팀은 서비스 및 해당 구성 요소를 변경할 수 있는 권리가 있습니다. 버그 및 UX 문제를 적극적으로 해결하고 있는 경우 WebPart를 업데이트해야 할 수 있습니다.
- 웹 파트를 업데이트하려면 웹 파트를 당사의 리포지토리에서 다운로드하여 테넌트 GitHub 업로드해야 합니다. 학습 경로 추가 정보 Microsoft 365 "솔루션 업데이트" [섹션을 참조하세요.](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>어떤 언어가 Microsoft 365 학습 경로를 사용할 수 있나요?

Microsoft 365 경로는 현재 영어로만 제공됩니다. 자동 종단-종단 프로비전은 영어 테넌트에서만 작동합니다. 2020년 2분기에는 다음 언어에 대한 다국어 지원을 롤아웃할 계획입니다. 

- 중국어(간체) 
- 프랑스어  
- 독일어 
- 이탈리아어(이탈리아) 
- 일본어(일본)  
- 포르투갈어(브라질) 
- 러시아어(러시아어)  
- 스페인어 

> 다가오는 학습 경로에 대한 다국어 지원 릴리스에는 네덜란드어 지원이 포함되지 않습니다. 향후에도 새로운 언어 옵션을 평가할 예정입니다.

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>테넌트 환경에 사이트를 설치하는 데 시간이 얼마나 걸릴까요?

설치 테스트에 따라 15분 미만이 걸립니다. 여기에는 요구 사항에 맞게 사이트를 사용자 지정하는 데 필요한 시간은 포함되지 않습니다.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Microsoft 365 학습 경로가 오픈 소스 솔루션인가요? 그 의미는 무엇입니까?

Microsoft 365 학습 경로는 OSS(오픈 소스 소프트웨어) 솔루션으로, OSS에 다양한 이점과 고려 사항을 제공합니다.

#### <a name="benefits"></a>이점 
- **Microsoft 365 경로는 무료 솔루션입니다.** 고객은 테넌트에 솔루션을 설치하고, 솔루션을 사용자 지정하고, 최종 사용자가 사용할 수 있도록 할 수 있습니다.
- **OSS를 사용하면 신속한 개발 및 공동 작업을 가능하게 합니다.**  모든 오픈 소스 솔루션은 광범위한 참가자 커뮤니티에서 사용할 수 있습니다.  Microsoft는 이러한 혁신을 추진하기 위해 최선을 다하고 있습니다.  핵심 서비스 관리 팀은 가장 광범위한 고객에게 혜택을 제공하는 환경을 제공하도록 보장하기 위해 공식 빌드에 병합되는 기여를 결정할 수 있는 권리가 있습니다.  
- **OSS를 사용하면 파트너와 공동 작업을 할 수 있습니다.** Microsoft는 여러 학습 파트너와 협력하여 향후 확장 및 학습 경로에 기여하기 위한 노력을 Microsoft 365 있습니다. 이러한 계획이 마무리될 때 추가 정보를 제공할 것입니다. 
    
#### <a name="implications"></a>의미
- **OSS는 상업용 제품이 아니며,** 상업용 제품에는 업데이트 및 패치가 포함되고 유료 지원 계약에 포함됩니다. Microsoft는 현재 문서, 업데이트 및 패치를 Microsoft 365 학습 경로에 대한 패치는 이러한 특정 비즈니스 시나리오를 개선하기 위한 노력의 기반이 됩니다. 당사의 계획은 학습 경로에 계속 투자할 계획입니다. 서비스 관리 팀은 향후 전략을 변경할 수 있습니다. 학습 경로에 Microsoft 365 변경 내용은 적용하기에 앞서 전달됩니다. 
- **OSS에서** Microsoft 365 학습 경로는 GitHub : Microsoft 365 Microsoft 지원 계약의 온라인 문제 목록을 통해 지원됩니다. 제출된 문제는 서비스 Microsoft 365 커뮤니티의 학습 경로에 따라 검토됩니다. 문제 해결 서비스 수준은 유료 Microsoft 지원 계약과 수준이 동일하지 않습니다.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>학습 경로를 Microsoft 365 사이트 모음의 하위 사이트로 만들 SharePoint 있습니까?

아니요. 이 사이트는 항상 루트 사이트 모음인 커뮤니케이션 사이트 서식 파일을 기반으로 합니다.

> [!NOTE]
> 최종 사용자가 사이트에 액세스하는 데 필요한 사용 권한을 고려해야 합니다. 대부분의 조직에서는 보안 또는 사용자 그룹을 정의했습니다. 직원 커뮤니티에 시작할 준비가 된 후 새 교육 포털에 적절한 보안 그룹을 추가해야 합니다.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>사이트를 다시 설치해야 합니다. 제가 뭘 해야 하나요?

여기에 게시된 설치 지침을 [따릅니다.](custom_provision.md)

> [!NOTE]
> 이전 설치에서 원격 분석 기능을 사용하지 않도록 설정한 경우 원격 분석 사용 안 을 계속하려면 여기에서 원격 분석 비활성화 지침을 따라야 합니다.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>학습 경로의 구현을 Microsoft 365 업데이트했습니다. 사이트를 다시 설치하면 이러한 업데이트(사이트 서식 파일, 재생 목록에 적용)가 손실될 수 있나요?

현재 설치를 통해 사이트를 다시 설치하면 개별 페이지 및 사용자 지정 재생 목록의 사용자 지정이 손실됩니다.  
