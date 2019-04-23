---
author: karuanag
ms.author: karuanag
title: 필수 구성 요소 및 결정 사항
ms.date: 02/10/2019
description: 사용자 지정 학습 설치 및 설정에 대 한 결정 및 필수 구성 요소 정보
ms.openlocfilehash: b7864d13e6ccd9c3b41e445ea491aed3b3471aff
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055268"
---
## <a name="service-decisions"></a>서비스 결정 사항

사용자 지정 학습에 대 한 필수 구성 요소가 충족 되었는지 확인 한 후에는 사용자 지정 학습의 implemenation에 대해 다음과 같은 사항을 결정 해야 합니다.

1. **최신 인터페이스가 있는 회사의 교육 포털이 이미 있습니까?**

- **예** 이러한 질문에 대 한 답이 예 이면 해당 기존 사이트 환경 내에서 [웹 파트를 설치](installwebpart.md) 하는 것이 좋습니다.
- **아니요** 응답 하지 않으면 [전체 사용자 지정 학습 사이트 패키지를 설치 하는](installsitepackage.md) 것이 좋습니다.  이렇게 하면 최종 사용자에 게 중요 한 정보를 포함 하기 위해 확장할 수 있는 최신 SharePoint Online 통신 사이트가 준비 됩니다.  사이트를 사용자 지정 해도 웹 파트는 콘텐츠 업데이트를 가져오는 기능에 영향을 주지 않습니다. 

2. **Office 365 관리자 인가요?**

- **예**: 설치에 대 한 적절 한 권한이 있습니다.
- **NO**: 사용자가 소유한 사이트 모음에 Office 365 관리자에 게 문의 하거나 웹 파트를 설치 합니다.

3. **조직에 공식적인 교육 부서가 있습니까?**

- **예**: 이러한 솔루션을 사용 하 여 사용자 지정 된 추가 교육 콘텐츠를 제공 하는 방법을 알려 주십시오.
- **NO**: [셀프 서비스 채택 키트](driveadoption.md) 를 사용 하 여 최종 사용자가 사이트를 도울 수 있도록 합니다.

4. **조직에 사용자 커뮤니티가 있습니까?  이는 기술에 대 한 자세한 정보 (예를 들어, power users 또는 자세히 알고자 하는 사용자)에 대해 자세히 알아볼 수 있는 공식적인 사용자나 비공식적인 그룹 중 하나입니다.**

- **예**: 사용자 지정 학습 사이트 환경을 사용 하 여 새 또는 기존 사용자 커뮤니티 포럼에 대 한 링크를 제공할 수 있습니다.
- **NO**: 사용자가 자신의 성공을 공유 하 고 서로 정보를 공유할 수 있도록 내부 사용자 그룹을 시작 하는 것이 좋습니다.  내부 사용자 그룹을 nurture 할 시간이 없는 경우 직원은 월별 교육을 위해 [마이크로 osft Office 365 챔피언 커뮤니티](https://aka.ms/O365Champions) 에 참가 하 고, 온라인 커뮤니티의 멤버 자격과 Office 365 용 도구 및 리소스에 대 한 초기 액세스 권한을 부여할 수 있습니다.

5.  **사이트 유지 관리 또는 지원 관련 질문에 대 한 책임을 야 하나요?**

- **예**: 사용자 지정 학습 사이트 지원을 보다 쉽게 만들기 위해 Office 365의 기능을 사용 하는 것이 좋습니다.  서비스 구독 및 조직 크기에 따라 다음과 같은 몇 가지 아이디어가 있습니다.
    1. 대규모 조직에서는 공개 Yammer 커뮤니티를 프로 비전 하 여 사이트에 대 한 의견을 받을 수 있습니다.
    2. Microsoft 팀에 참가 하 여 질문을 하 고 대화를 공유할 수 있는 최대 2500 명의 사용자
    3. 공식적인 지원 티켓 프로세스는 양식, 흐름, SharePoint Online 목록 또는 회사에서 이미 IT 지원을 받을 수 있는 다른 타사 도구를 사용 하 여 suppored 수 있습니다. 
- **NO**: SharePoint Online 지원을 제공 하는 IT 직원과 사이트/웹 파트의 설치에 대해 설명 합니다.  

### <a name="next-steps---site-provisioninginstallsitepackagemd-or-webpartinstallwebpartmd-installation-steps"></a>다음 단계- [사이트 프로 비전](installsitepackage.md) 또는 [웹 파트](installwebpart.md) 설치 단계