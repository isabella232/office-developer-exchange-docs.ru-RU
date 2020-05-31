---
title: API Microsoft Graph Outlook для почты, календарей и контактов
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Сведения о API Microsoft Graph, которые можно использовать для доступа к электронной почте, календарям и контактам в Office 365 или Exchange Online.
ms.openlocfilehash: 3065de389157345afd5ed07e302ace99e2048bdf
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353296"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="1df0c-103">Приложения Microsoft Graph REST API для почты, календаря и контактов</span><span class="sxs-lookup"><span data-stu-id="1df0c-103">Microsoft Graph REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="1df0c-104">Найдите сведения о API Microsoft Graph, которые можно использовать для доступа к электронной почте, календарям и контактам в Office 365 или Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1df0c-104">Find information about the Microsoft Graph APIs that you can use to access mail, calendars, and contacts in Office 365 or Exchange Online.</span></span>

<span data-ttu-id="1df0c-105">Office 365 и Exchange Online предоставляют новый способ работы с электронной почтой, календарями и контактами.</span><span class="sxs-lookup"><span data-stu-id="1df0c-105">Office 365 and Exchange Online provide a new way to work with email, calendars, and contacts.</span></span> <span data-ttu-id="1df0c-106">REST API Microsoft Graph, календарь и контакт REST предоставляют мощный и простой в использовании способ доступа к данным Exchange и управления ими.</span><span class="sxs-lookup"><span data-stu-id="1df0c-106">The Microsoft Graph Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data.</span></span> <span data-ttu-id="1df0c-107">Эти API основаны на открытых стандартах: OAuth версии 2,0 для проверки подлинности и OData версии 4,0 и JSON для абстракции данных.</span><span class="sxs-lookup"><span data-stu-id="1df0c-107">These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction.</span></span> <span data-ttu-id="1df0c-108">Это обеспечивает следующие преимущества:</span><span class="sxs-lookup"><span data-stu-id="1df0c-108">This provides the following advantages:</span></span>

- <span data-ttu-id="1df0c-109">Так как эти API требуют OAuth для проверки подлинности, приложению не требуется обрабатывать или хранить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="1df0c-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>

- <span data-ttu-id="1df0c-110">OAuth позволяет запрашивать строго ограниченные разрешения на пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="1df0c-110">OAuth makes it possible to request tightly scoped permissions to user data.</span></span> <span data-ttu-id="1df0c-111">Например, вы можете создать приложение, запросите разрешение и прочесть только календарь пользователя.</span><span class="sxs-lookup"><span data-stu-id="1df0c-111">For example, you might design your application to request permission and read only a user's calendar.</span></span>

## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="1df0c-112">Работать с почтовыми папками и почтовыми папками</span><span class="sxs-lookup"><span data-stu-id="1df0c-112">Work with email and mail folders</span></span>

<span data-ttu-id="1df0c-113">С помощью [почтовых API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) можно получать, создавать, обновлять, удалять, перемещать, копировать и отправлять сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1df0c-113">You can use the [Mail API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) to get, create, update, delete, move, copy, and send email.</span></span> <span data-ttu-id="1df0c-114">Вы также можете получать, создавать, обновлять и удалять почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="1df0c-114">You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="1df0c-115">Работать с событиями, календарями и группами календарей</span><span class="sxs-lookup"><span data-stu-id="1df0c-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="1df0c-116">С помощью [API календаря](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) можно получать, создавать, обновлять и удалять события.</span><span class="sxs-lookup"><span data-stu-id="1df0c-116">You can use the [Calendar API](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) to get, create, update, and delete events.</span></span> <span data-ttu-id="1df0c-117">Вы также можете получать, создавать, обновлять и удалять группы и календари календаря.</span><span class="sxs-lookup"><span data-stu-id="1df0c-117">You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="1df0c-118">Работать с контактами и папками контактов</span><span class="sxs-lookup"><span data-stu-id="1df0c-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="1df0c-119">С помощью [API контактов](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) вы можете получать, создавать, обновлять и удалять контакты в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="1df0c-119">You can use the [Contacts API](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) to get, create, update, and delete contacts in a user's mailbox.</span></span> <span data-ttu-id="1df0c-120">Вы также можете получать папки контактов.</span><span class="sxs-lookup"><span data-stu-id="1df0c-120">You can also get contact folders.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="1df0c-121">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1df0c-121">Next steps</span></span>

<span data-ttu-id="1df0c-122">Перейдите на страницу [Документация по Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview) , чтобы получить дополнительные сведения об интерфейсах API почты, календаря и контактов, в том числе рекомендации по настройке среды и началу работы с API.</span><span class="sxs-lookup"><span data-stu-id="1df0c-122">Head over to the [Microsoft Graph documentation](https://developer.microsoft.com/graph/docs/concepts/overview) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs.</span></span> 

<span data-ttu-id="1df0c-123">Кроме того, ознакомьтесь с [краткими руководствами](https://developer.microsoft.com/graph/quick-start) и [примерами кода](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) , чтобы увидеть эти API в действии.</span><span class="sxs-lookup"><span data-stu-id="1df0c-123">Also be sure to check out the [quick starts](https://developer.microsoft.com/graph/quick-start) and [code samples](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1df0c-124">См. также</span><span class="sxs-lookup"><span data-stu-id="1df0c-124">See also</span></span>

- [<span data-ttu-id="1df0c-125">Документация по Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1df0c-125">Microsoft Graph documentation</span></span>](https://developer.microsoft.com/graph/docs/concepts/overview)   

