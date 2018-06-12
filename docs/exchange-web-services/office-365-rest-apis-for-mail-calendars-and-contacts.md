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
# <a name="office-365-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="f13dc-103">API-интерфейсы REST Office 365 для почты, календарям и контактам</span><span class="sxs-lookup"><span data-stu-id="f13dc-103">Office 365 REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="f13dc-104">Сведения об Office 365 API-интерфейсы, которые можно использовать, чтобы получать доступ к почте, календарям и контактам в Office 365 и Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f13dc-104">Find information about the Office 365 APIs that you can use to access mail, calendars, and contacts in Office 365 or Exchange Online.</span></span>
  
<span data-ttu-id="f13dc-105">Office 365 и Exchange Online предоставляют новый способ работы с электронной почты, календарям и контактам.</span><span class="sxs-lookup"><span data-stu-id="f13dc-105">Office 365 and Exchange Online provide a new way to work with email, calendars, and contacts.</span></span> <span data-ttu-id="f13dc-106">Почта, календарь и API-интерфейсы REST контактов позволяют мощные и простые в использовании для доступа и работы с данными Exchange.</span><span class="sxs-lookup"><span data-stu-id="f13dc-106">The Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data.</span></span> <span data-ttu-id="f13dc-107">Эти интерфейсы API на основе открытых стандартов: OAuth версии 2.0 для проверки подлинности и OData версии 4.0 и JSON для абстракции данных.</span><span class="sxs-lookup"><span data-stu-id="f13dc-107">These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction.</span></span> <span data-ttu-id="f13dc-108">Это обеспечивает следующие преимущества:</span><span class="sxs-lookup"><span data-stu-id="f13dc-108">This provides the following advantages:</span></span>
  
- <span data-ttu-id="f13dc-109">Так как эти интерфейсы API использующих OAuth для проверки подлинности, приложения не нужно обрабатывать или хранение учетных данных пользователя.</span><span class="sxs-lookup"><span data-stu-id="f13dc-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>
    
- <span data-ttu-id="f13dc-110">OAuth позволяет запрашивать тесно заданной областью разрешения для пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="f13dc-110">OAuth makes it possible to request tightly scoped permissions to user data.</span></span> <span data-ttu-id="f13dc-111">Например можно создать приложение для запроса разрешений и читать только календарь пользователя.</span><span class="sxs-lookup"><span data-stu-id="f13dc-111">For example, you might design your application to request permission and read only a user's calendar.</span></span>
    
## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="f13dc-112">Работа с электронной почты и почтовых папок</span><span class="sxs-lookup"><span data-stu-id="f13dc-112">Work with email and mail folders</span></span>

<span data-ttu-id="f13dc-113">[API почты](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) можно использовать для получения, создание, обновление, удаление, перемещение, копирование и адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f13dc-113">You can use the [Mail API](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) to get, create, update, delete, move, copy, and send email.</span></span> <span data-ttu-id="f13dc-114">Также можно получить, создание, обновление и удаление почтовых папок.</span><span class="sxs-lookup"><span data-stu-id="f13dc-114">You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="f13dc-115">Работа с событиями, календари и группы календаря</span><span class="sxs-lookup"><span data-stu-id="f13dc-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="f13dc-116">Использование [API календаря](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) для получения, создание, обновление и удаление событий.</span><span class="sxs-lookup"><span data-stu-id="f13dc-116">You can use the [Calendar API](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) to get, create, update, and delete events.</span></span> <span data-ttu-id="f13dc-117">Также можно получить, создание, обновление и удаление групп календаря и календарей.</span><span class="sxs-lookup"><span data-stu-id="f13dc-117">You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="f13dc-118">Работа с контактами и папки контактов</span><span class="sxs-lookup"><span data-stu-id="f13dc-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="f13dc-119">Использование [API контакты](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) для получения, создание, обновление и удаление контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f13dc-119">You can use the [Contacts API](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) to get, create, update, and delete contacts in a user's mailbox.</span></span> <span data-ttu-id="f13dc-120">Можно также получить папок контактов.</span><span class="sxs-lookup"><span data-stu-id="f13dc-120">You can also get contact folders.</span></span> 
  
## <a name="work-with-file-providers"></a><span data-ttu-id="f13dc-121">Работа с поставщиками файла</span><span class="sxs-lookup"><span data-stu-id="f13dc-121">Work with file providers</span></span>

<span data-ttu-id="f13dc-122">Использование [Интерфейса API REST поставщиков файла](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) для получения, создание, обновление и удаление сведения о поставщиках файлов, поддерживаемые, такие как почтовый ящик, общего банка данных и т. д.</span><span class="sxs-lookup"><span data-stu-id="f13dc-122">You can use the [File Providers REST API](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) to get, create, update, and delete information about supported file providers, such as mailbox, Dropbox, and so on.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="f13dc-123">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f13dc-123">Next steps</span></span>

<span data-ttu-id="f13dc-124">Не забывайте через также посещать страницы [Разработка на платформе Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) , чтобы получить дополнительные сведения о почту, календарь и интерфейсов API, контакты, включая информацию о настройке среды и начало работы с API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="f13dc-124">Head over to the [Developing on the Office 365 platform](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs.</span></span> <span data-ttu-id="f13dc-125">Также не забудьте проверить [начальные проекты и примеры кода,](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) чтобы увидеть эти интерфейсы API в действии.</span><span class="sxs-lookup"><span data-stu-id="f13dc-125">Also be sure to check out the [starter projects and code samples](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f13dc-126">См. также</span><span class="sxs-lookup"><span data-stu-id="f13dc-126">See also</span></span>


- [<span data-ttu-id="f13dc-127">Разработка на платформе Office 365</span><span class="sxs-lookup"><span data-stu-id="f13dc-127">Developing on the Office 365 platform</span></span>](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)
    
- [<span data-ttu-id="f13dc-128">Создание приложения Office 365 ASP.NET MVC</span><span class="sxs-lookup"><span data-stu-id="f13dc-128">Building an Office 365 ASP.NET MVC app</span></span>](http://msdn.microsoft.com/office/office365/howto/Build-your-first-ASPNET-MVC-app%28Office.15%29.aspx)
    
- [<span data-ttu-id="f13dc-129">Операции REST с почтой</span><span class="sxs-lookup"><span data-stu-id="f13dc-129">Mail REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="f13dc-130">Операции REST с календарем</span><span class="sxs-lookup"><span data-stu-id="f13dc-130">Calendar REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="f13dc-131">Операции REST с контактами</span><span class="sxs-lookup"><span data-stu-id="f13dc-131">Contacts REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="f13dc-132">Проекты API Office 365 и примеры кода для начинающих</span><span class="sxs-lookup"><span data-stu-id="f13dc-132">Office 365 APIs starter projects and code samples</span></span>](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)
    

