---
title: API-интерфейсы REST Office 365 для почты, календарям и контактам
manager: sethgros
ms.date: 4/29/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Сведения об Office 365 API-интерфейсы, которые можно использовать, чтобы получать доступ к почте, календарям и контактам в Office 365 и Exchange Online.
ms.openlocfilehash: d42d3ff0b68dfbf23d5a4eebb826a6d39a4ac116
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761233"
---
# <a name="office-365-rest-apis-for-mail-calendars-and-contacts"></a>API-интерфейсы REST Office 365 для почты, календарям и контактам

Сведения об Office 365 API-интерфейсы, которые можно использовать, чтобы получать доступ к почте, календарям и контактам в Office 365 и Exchange Online.
  
Office 365 и Exchange Online предоставляют новый способ работы с электронной почты, календарям и контактам. Почта, календарь и API-интерфейсы REST контактов позволяют мощные и простые в использовании для доступа и работы с данными Exchange. Эти интерфейсы API на основе открытых стандартов: OAuth версии 2.0 для проверки подлинности и OData версии 4.0 и JSON для абстракции данных. Это обеспечивает следующие преимущества:
  
- Так как эти интерфейсы API использующих OAuth для проверки подлинности, приложения не нужно обрабатывать или хранение учетных данных пользователя.
    
- OAuth позволяет запрашивать тесно заданной областью разрешения для пользовательских данных. Например можно создать приложение для запроса разрешений и читать только календарь пользователя.
    
## <a name="work-with-email-and-mail-folders"></a>Работа с электронной почты и почтовых папок

[API почты](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) можно использовать для получения, создание, обновление, удаление, перемещение, копирование и адрес электронной почты. Также можно получить, создание, обновление и удаление почтовых папок. 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a>Работа с событиями, календари и группы календаря

Использование [API календаря](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) для получения, создание, обновление и удаление событий. Также можно получить, создание, обновление и удаление групп календаря и календарей. 
  
## <a name="work-with-contacts-and-contact-folders"></a>Работа с контактами и папки контактов

Использование [API контакты](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) для получения, создание, обновление и удаление контактов в почтовом ящике пользователя. Можно также получить папок контактов. 
  
## <a name="work-with-file-providers"></a>Работа с поставщиками файла

Использование [Интерфейса API REST поставщиков файла](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) для получения, создание, обновление и удаление сведения о поставщиках файлов, поддерживаемые, такие как почтовый ящик, общего банка данных и т. д. 
  
## <a name="next-steps"></a>Дальнейшие действия

Не забывайте через также посещать страницы [Разработка на платформе Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) , чтобы получить дополнительные сведения о почту, календарь и интерфейсов API, контакты, включая информацию о настройке среды и начало работы с API-интерфейсы. Также не забудьте проверить [начальные проекты и примеры кода,](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) чтобы увидеть эти интерфейсы API в действии. 
  
## <a name="see-also"></a>См. также


- [Разработка на платформе Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)
    
- [Создание приложения Office 365 ASP.NET MVC](http://msdn.microsoft.com/office/office365/howto/Build-your-first-ASPNET-MVC-app%28Office.15%29.aspx)
    
- [Операции REST с почтой](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx)
    
- [Операции REST с календарем](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx)
    
- [Операции REST с контактами](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx)
    
- [Проекты API Office 365 и примеры кода для начинающих](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)
    

