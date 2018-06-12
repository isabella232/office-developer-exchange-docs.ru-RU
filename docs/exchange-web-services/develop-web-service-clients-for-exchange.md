---
title: Разработка клиентов веб-служб для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 899ba15b-336d-4f9b-8563-318c61e43713
description: Здесь вы найдете сведения, которые помогут вам в разработке веб-служб Exchange и клиентских приложений для них.
ms.openlocfilehash: 2b8b032124e45dda7c83932d519ffb87bcdb5514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760933"
---
# <a name="develop-web-service-clients-for-exchange"></a><span data-ttu-id="a9aa9-103">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-103">Develop web service clients for Exchange</span></span>

<span data-ttu-id="a9aa9-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Здесь вы найдете сведения, которые помогут вам в разработке веб-служб Exchange и клиентских приложений для них.</span><span class="sxs-lookup"><span data-stu-id="a9aa9-104">Find information to help you develop EWS and web service client applications for Exchange.</span></span>
  
<span data-ttu-id="a9aa9-105">В статьях этого раздела объясняется, как использовать веб-службы Exchange и веб-службы в клиентских приложениях Exchange для Exchange Online, Exchange Online в рамках Office 365 и локальных версий Exchange, начиная с версии 2013. Кроме того, на примерах показано, как выполнять определенные задачи.</span><span class="sxs-lookup"><span data-stu-id="a9aa9-105">The articles in this section explain how to use EWS and web services in your Exchange client applications for Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange 2013, and provide examples that show you how to perform specific tasks.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="a9aa9-106">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="a9aa9-106">In this section</span></span>

- [<span data-ttu-id="a9aa9-107">Архивация в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-107">Archiving in EWS in Exchange</span></span>](archiving-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-108">Attachments and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-108">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-109">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-109">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-110">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-110">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-111">Группы рассылки и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-111">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-112">обнаружение электронных данных в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-112">eDiscovery in EWS in Exchange</span></span>](ediscovery-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-113">Электронная почта и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-113">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-114">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-114">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-115">Идентификаторы в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-115">Identifiers in Exchange</span></span>](ews-identifiers-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-116">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-116">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-117">Управление папкой "Входящие" и веб-службы Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-117">Inbox management and EWS in Exchange</span></span>](inbox-management-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-118">Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-118">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-119">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-119">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-120">Параметры сохраняемого приложения в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-120">Persistent application settings in EWS in Exchange</span></span>](persistent-application-settings-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-121">Свойства и расширенные свойства в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-121">Properties and extended properties in EWS in Exchange</span></span>](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-122">Наборы свойств и ответ с фигурами в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-122">Property sets and response shapes in EWS in Exchange</span></span>](property-sets-and-response-shapes-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-123">Общих папок в Exchange доступ с EWS</span><span class="sxs-lookup"><span data-stu-id="a9aa9-123">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-124">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-124">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-125">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-125">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-126">Часовые пояса и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-126">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a9aa9-127">Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-127">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    
- [<span data-ttu-id="a9aa9-128">Проверка результатов вызова EWS или EWS управляемых API</span><span class="sxs-lookup"><span data-stu-id="a9aa9-128">Verifying the results of an EWS or EWS Managed API call</span></span>](verifying-the-results-of-an-ews-or-ews-managed-api-call.md)
    
## <a name="see-also"></a><span data-ttu-id="a9aa9-129">См. также</span><span class="sxs-lookup"><span data-stu-id="a9aa9-129">See also</span></span>

- [<span data-ttu-id="a9aa9-130">Сведения об управляемом API EWS, EWS и веб-службах в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-130">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)     
- [<span data-ttu-id="a9aa9-131">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-131">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="a9aa9-132">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-132">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)  
- [<span data-ttu-id="a9aa9-133">Справочник по веб-службам для Exchange</span><span class="sxs-lookup"><span data-stu-id="a9aa9-133">Web services reference for Exchange</span></span>](../web-service-reference/web-services-reference-for-exchange.md)
    

