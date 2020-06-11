---
author: pkrebs
ms.author: pkrebs
title: 사이트 페이지 번역
ms.date: 02/10/2019
description: 사이트 페이지 번역
ms.openlocfilehash: 32dc0928d12074575c8608cef38e4b4d0e5e5cf3
ms.sourcegitcommit: 46caa9fa9d129bee107a8c9a7c5bc70a7f9af087
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2020
ms.locfileid: "44699136"
---
# <a name="translate-site-pages"></a>사이트 페이지 번역
기존 버전의 학습 경로를 버전 4.0으로 업데이트 했거나 새 사이트를 프로 비전 했는지 여부에 관계 없이 사이트 페이지 번역 프로세스는 동일 합니다. 그러나 몇 가지 사항을 알아야 합니다. 
- 다국어 4.0 버전의 새 학습 경로를 프로 비전 하는 경우 사이트 페이지는 9 개의 언어로 번역 됩니다. 
- 학습 경로 솔루션이 다국어 4.0 버전으로 업데이트 되 면 학습 경로 SharePoint 사이트 페이지는 변경 되지 않은 상태로 유지 됩니다. 번역은 수동으로 수행 해야 합니다. 

기본적으로 학습 경로 사이트에서는 다음과 같은 페이지를 제공 합니다.

- Home.aspx
- Start-with-Six-Simple-Steps .aspx
- Get-started-with-Microsoft-365 .aspx
- Get-started-with-Microsoft-Teams .aspx
- Get-started-with-SharePoint .aspx
- Get-started-with-OneDriive .aspx
- Ask-questions-and-get-help .aspx
- 교육 이벤트 일정 .aspx
- Become-a-Champion .aspx
- Recommended-Playlists .aspx
- 학습 경로 관리 성공 센터

## <a name="create-pages-for-the-languages-you-want"></a>원하는 언어에 대 한 페이지 만들기
다국어 기능에 대 한 사이트를 사용 하도록 설정 하 고 사용 가능 하도록 설정할 언어를 선택한 후에는 원하는 번역 페이지를 만들 수 있습니다. 몇 가지 중요 한 개념을 설명 하기 위해 Microsoft 365 교육 페이지를 예로 사용 합니다. 이렇게 하려면 다음을 실행합니다.

1.  학습 경로 **홈** 페이지에서 **Microsoft 365 교육**을 클릭 합니다.  
2.  위쪽 막대에서 **번역**을 선택 합니다.
![custom_update_ml_transbutton.png](media/custom_update_ml_transbutton.png)
3. 사이트에 사용할 수 있는 각 언어의 번역 페이지를 만들려면 **모든 언어에 대해 만들기**를 선택 합니다. 그렇지 않은 경우 원하는 언어에 대해서만 **만들기** 를 선택 합니다. 이 예에서는 이탈리아어를 선택 합니다.
4.  **보기**를 클릭 합니다. 이제 페이지를 번역할 준비가 되었습니다. 

### <a name="an-important-concept-to-know"></a>알아야 할 중요 한 개념
다음 예제에서는 페이지가 이탈리아어로 변환 되었습니다. 하지만 사이트 제목, 탐색 및 웹 파트는 여전히 영어로 표시 됩니다. 

![custom_update_ml_transpgconcept.png](media/custom_update_ml_transpgconcept.png)

 사이트가 영어로 설정 되 면 스페인어 (예: 기본 설정 된 개인 언어)를 사용 하는 사용자는 수동으로 제목, 탐색, 바닥글 내용을 스페인어로 편집 하 고 변환 합니다. 독일어로 표시 되는 사용자는 독일어와 동일한 방식으로 사용 됩니다. 콘텐츠를 번역 하면 해당 기본 언어의 모든 사용자에 대해 표시 됩니다. 웹 파트는 사용자의 기본 설정 언어를 선택 하 고 해당 언어로 번역 된 콘텐츠를 표시 합니다. 

> [!IMPORTANT]
> 중요: 번역 페이지를 만든 후에는 기본 영어 페이지를 게시 하거나 다시 게시 해야 다음을 확인할 수 있습니다.
- 번역 페이지는 해당 언어 사이트에 표시 됩니다.
- 뉴스 웹 파트 및 강조 표시 된 콘텐츠 웹 파트에서 번역 페이지가 올바르게 표시 됨
- 사이트 위쪽의 언어 드롭다운에서 사용 하도록 설정한 모든 언어를 포함 합니다.
- 번역자는 번역 요청에 대 한 알림을 받습니다.

## <a name="what-does-a-translator-do"></a>번역기는 어떤 역할을 하나요?
번역자는 기본 언어 페이지의 복사본을 지정 된 언어로 수동으로 번역 합니다. 페이지 복사본을 만들 때 번역자에 게 전자 메일로 알림이 전송 됩니다. 이 전자 메일에는 기본 언어 페이지와 새로 만든 번역 페이지에 대 한 링크가 포함 되어 있습니다. 변환기는 다음과 같은 작업을 수행 합니다.
1. 전자 메일에서 **번역 시작** 단추를 선택 합니다.
2. 페이지 오른쪽 위에서 **편집** 을 선택 하 고 콘텐츠를 번역 합니다.
3. 작업이 완료 되 면 **초안으로 저장** (독자에 게 공개할 준비가 되지 않은 경우)을 선택 하 고, 사이트에서 해당 언어를 사용 하는 모든 사용자가 페이지를 볼 준비가 되 면 **게시** 또는 **게시물**게시를 선택 합니다.

변환 프로세스에 대 한 자세한 내용은 [다국어 통신 사이트, 페이지 및 뉴스 만들기](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)를 참조 하세요. 

## <a name="updating-the-default-language-page"></a>기본 언어 페이지 업데이트
기본 언어 페이지가 업데이트 되 면 페이지를 다시 게시 해야 합니다. 그러면 번역 페이지의 변환기에 게 업데이트를 적용 하 여 개별 번역 페이지에 대 한 업데이트를 수행할 수 있는 전자 메일 알림이 제공 됩니다.

## <a name="next-steps"></a>다음 단계
- [사용자 지정 재생 목록 변환](custom_translate_pl_ml.md)
- [Multiligual 콘텐츠 숨기기 및 표시](custom_translate_pl_ml.md)
