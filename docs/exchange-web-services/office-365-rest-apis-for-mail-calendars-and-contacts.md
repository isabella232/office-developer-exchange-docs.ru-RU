---
title: Microsoft Graph Outlook API-Интерфейс для почты, календарям и контактам
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Найдите сведения о Microsoft Graph API, которые можно использовать, чтобы получать доступ к почте, календарям и контактам в Office 365 и Exchange Online.
ms.openlocfilehash: 3065de389157345afd5ed07e302ace99e2048bdf
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353296"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="a0274-103">Microsoft Graph API-интерфейсы REST для почты, календарям и контактам</span><span class="sxs-lookup"><span data-stu-id="a0274-103">Microsoft Graph REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="a0274-104">Найдите сведения о Microsoft Graph API-интерфейсы, которые можно использовать, чтобы получать доступ к почте, календарям и контактам в Office 365 и Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a0274-104">Find information about the Microsoft Graph APIs that you can use to access mail, calendars, and contacts in Office 365 or Exchange Online.</span></span>

<span data-ttu-id="a0274-105">Office 365 и Exchange Online предоставляют новый способ работы с электронной почты, календарям и контактам.</span><span class="sxs-lookup"><span data-stu-id="a0274-105">Office 365 and Exchange Online provide a new way to work with email, calendars, and contacts.</span></span> <span data-ttu-id="a0274-106">Графическое представление Microsoft Mail, календаря и API-интерфейсы REST контактов позволяют мощные и простые в использовании для доступа и работы с данными Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0274-106">The Microsoft Graph Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data.</span></span> <span data-ttu-id="a0274-107">Эти интерфейсы API на основе открытых стандартов: OAuth версии 2.0 для проверки подлинности и OData версии 4.0 и JSON для абстракции данных.</span><span class="sxs-lookup"><span data-stu-id="a0274-107">These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction.</span></span> <span data-ttu-id="a0274-108">Это обеспечивает следующие преимущества:</span><span class="sxs-lookup"><span data-stu-id="a0274-108">This provides the following advantages:</span></span>

- <span data-ttu-id="a0274-109">Так как эти интерфейсы API использующих OAuth для проверки подлинности, приложения не нужно обрабатывать или хранение учетных данных пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0274-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>

- <span data-ttu-id="a0274-110">OAuth позволяет запрашивать тесно заданной областью разрешения для пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="a0274-110">OAuth makes it possible to request tightly scoped permissions to user data.</span></span> <span data-ttu-id="a0274-111">Например можно создать приложение для запроса разрешений и читать только календарь пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0274-111">For example, you might design your application to request permission and read only a user's calendar.</span></span>

## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="a0274-112">Работа с электронной почты и почтовых папок</span><span class="sxs-lookup"><span data-stu-id="a0274-112">Work with email and mail folders</span></span>

<span data-ttu-id="a0274-113">[API почты](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) можно использовать для получения, создание, обновление, удаление, перемещение, копирование и адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a0274-113">You can use the [Mail API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) to get, create, update, delete, move, copy, and send email.</span></span> <span data-ttu-id="a0274-114">Также можно получить, создание, обновление и удаление почтовых папок.</span><span class="sxs-lookup"><span data-stu-id="a0274-114">You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="a0274-115">Работа с событиями, календари и группы календаря</span><span class="sxs-lookup"><span data-stu-id="a0274-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="a0274-116">Использование [API календаря](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) для получения, создание, обновление и удаление событий.</span><span class="sxs-lookup"><span data-stu-id="a0274-116">You can use the [Calendar API](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) to get, create, update, and delete events.</span></span> <span data-ttu-id="a0274-117">Также можно получить, создание, обновление и удаление групп календаря и календарей.</span><span class="sxs-lookup"><span data-stu-id="a0274-117">You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="a0274-118">Работа с контактами и папки контактов</span><span class="sxs-lookup"><span data-stu-id="a0274-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="a0274-119">Использование [API контакты](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) для получения, создание, обновление и удаление контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0274-119">You can use the [Contacts API](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) to get, create, update, and delete contacts in a user's mailbox.</span></span> <span data-ttu-id="a0274-120">Можно также получить папок контактов.</span><span class="sxs-lookup"><span data-stu-id="a0274-120">You can also get contact folders.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="a0274-121">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="a0274-121">Next steps</span></span>

<span data-ttu-id="a0274-122">Не забывайте через также посещать [Документация Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview) страницы, чтобы получить дополнительные сведения о почту, календарь и интерфейсов API, контакты, включая информацию о настройке среды и начало работы с API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="a0274-122">Head over to the [Microsoft Graph documentation](https://developer.microsoft.com/graph/docs/concepts/overview) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs.</span></span> 

<span data-ttu-id="a0274-123">Также необходимо извлечь [краткие руководства](https://developer.microsoft.com/graph/quick-start) и [примеры кода](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) для просмотра этих API-интерфейсы в действии.</span><span class="sxs-lookup"><span data-stu-id="a0274-123">Also be sure to check out the [quick starts](https://developer.microsoft.com/graph/quick-start) and [code samples](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a0274-124">См. также</span><span class="sxs-lookup"><span data-stu-id="a0274-124">See also</span></span>

- [<span data-ttu-id="a0274-125">Документация по Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a0274-125">Microsoft Graph documentation</span></span>](https://developer.microsoft.com/graph/docs/concepts/overview)   

