---
title: API Microsoft Graph Outlook для почты, календарей и контактов
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Сведения о API Microsoft Graph, которые можно использовать для доступа к электронной почте, календарям и контактам в Office 365 или Exchange Online.
localization_priority: Priority
ms.openlocfilehash: 7ca77596afb59ffab76001abd495de7328d2dd29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463869"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a>Приложения Microsoft Graph REST API для почты, календаря и контактов

Найдите сведения о API Microsoft Graph, которые можно использовать для доступа к электронной почте, календарям и контактам в Office 365, Exchange Online или Exchange Server в гибридных развертываниях.

Office 365, Exchange Online и Exchange Server в гибридных развертываниях предоставляют новый способ работы с электронной почтой, календарями и контактами. REST API Microsoft Graph, календарь и контакт REST предоставляют мощный и простой в использовании способ доступа к данным Exchange и управления ими. Эти API основаны на открытых стандартах: OAuth версии 2,0 для проверки подлинности и OData версии 4,0 и JSON для абстракции данных. Это обеспечивает следующие преимущества:

- Так как эти API требуют OAuth для проверки подлинности, приложению не требуется обрабатывать или хранить учетные данные пользователя.

- OAuth позволяет запрашивать строго ограниченные разрешения на пользовательские данные. Например, вы можете создать приложение, запросите разрешение и прочесть только календарь пользователя.

## <a name="work-with-email-and-mail-folders"></a>Работать с почтовыми папками и почтовыми папками

С помощью [почтовых API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) можно получать, создавать, обновлять, удалять, перемещать, копировать и отправлять сообщения электронной почты. Вы также можете получать, создавать, обновлять и удалять почтовые папки. 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a>Работать с событиями, календарями и группами календарей

С помощью [API календаря](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) можно получать, создавать, обновлять и удалять события. Вы также можете получать, создавать, обновлять и удалять группы и календари календаря. 
  
## <a name="work-with-contacts-and-contact-folders"></a>Работать с контактами и папками контактов

С помощью [API контактов](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) вы можете получать, создавать, обновлять и удалять контакты в почтовом ящике пользователя. Вы также можете получать папки контактов. 
  
## <a name="next-steps"></a>Дальнейшие действия

Перейдите на страницу [Документация по Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview) , чтобы получить дополнительные сведения об интерфейсах API почты, календаря и контактов, в том числе рекомендации по настройке среды и началу работы с API. 

Кроме того, ознакомьтесь с [краткими руководствами](https://developer.microsoft.com/graph/quick-start) и [примерами кода](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) , чтобы увидеть эти API в действии. 
  
## <a name="see-also"></a>См. также

- [Документация по Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview)   
- [Локальные требования для REST API](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api)   

