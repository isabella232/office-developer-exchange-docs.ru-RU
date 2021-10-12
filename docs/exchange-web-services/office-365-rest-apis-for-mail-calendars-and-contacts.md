---
title: API Microsoft Graph Outlook для почты, календаря и контактов
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Узнайте сведения об API Microsoft Graph, который можно использовать для доступа к почте, календарям и контактам в Office 365 или Exchange Online.
localization_priority: Priority
ms.openlocfilehash: 221b461443e8520d7631b8e2400e662025c8a268
ms.sourcegitcommit: f13a3a4a61fa23ca6414b7c96ddf087adbe3dc9e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/11/2021
ms.locfileid: "60262192"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a>Приложения Microsoft Graph REST API для почты, календаря и контактов

Узнайте сведения об API Microsoft Graph, которые можно использовать для доступа к почте, календарям и контактам в Office 365, Exchange Online или Exchange Server в гибридных развертываниях.

Office 365, Exchange Online и Exchange Server в гибридных развертываниях предоставляют новый способ работы с почтой, календарями и контактами. API REST почты, календаря и контактов Microsoft Graph обеспечивает мощный и простой способ доступа к данным Exchange и их использования. Эти API основаны на открытых стандартах: OAuth версии 2.0 для проверки подлинности и OData версии 4.0 и JSON для абстракции данных. Это обеспечивает следующие преимущества:

- Поскольку этим API требуется OAuth для проверки подлинности, то вашему приложению не нужно обрабатывать или хранить учетные данные пользователей.

- OAuth также позволяет запрашивать очень ограниченные права на данные пользователя. Например, можно создать приложение для запроса разрешений и только чтения календаря пользователя.

## <a name="work-with-email-and-mail-folders"></a>Работа с электронной почтой и папками электронной почты

Можно использовать [API электронной почты](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) для получения, создания, обновления, удаления, перемещения, копирования и отправки электронной почты. Вы также можете получать, создавать, обновлять и удалять почтовые папки. 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a>Работа с событиями, календарями и группами календарей

Можно использовать [API календаря](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) для получения, создания, обновления и удаления событий. Вы также можете получать, создавать, обновлять и удалять группы календарей и календари. 
  
## <a name="work-with-contacts-and-contact-folders"></a>Работа с контактами и папками контактов

Можно использовать [API контактов](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) для получения, создания, обновления и удаления контактов в почтовом ящике пользователя. Вы также можете получать папки контактов. 
  
## <a name="next-steps"></a>Дальнейшие действия

Перейдите на страницу документации [Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview) для получения дополнительных сведений об API почты, календаря и контактов, включая рекомендации по настройке среды и началу работы с API. 

Кроме того, ознакомьтесь с примерами [кратких руководств по началу работы](https://developer.microsoft.com/graph/quick-start) и [примерами кода](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph), чтобы увидеть эти API в действии. 
  
## <a name="see-also"></a>См. также

- [Документация по Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview)   
- [Требования к локальной среде API REST](https://techcommunity.microsoft.com/t5/exchange-team-blog/on-premises-architectural-requirements-for-the-rest-api/ba-p/605609)   

