---
title: обнаружение электронных данных в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Узнайте об eDiscovery в веб-служб Exchange в Exchange.
ms.openlocfilehash: 6491fdd9f2246870a89bfa89bf7d97b972d67c92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760939"
---
# <a name="ediscovery-in-ews-in-exchange"></a><span data-ttu-id="be401-103">обнаружение электронных данных в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="be401-103">eDiscovery in EWS in Exchange</span></span>

<span data-ttu-id="be401-104">Узнайте об eDiscovery в веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="be401-104">Learn about eDiscovery in EWS in Exchange.</span></span>
  
<span data-ttu-id="be401-105">обнаружение электронных данных является федеративным запроса веб-службы, которая позволяет внешних приложений для выполнения запросов данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="be401-105">eDiscovery is a federated query web service that enables external applications to perform queries of Exchange data.</span></span>
  
<span data-ttu-id="be401-106">Обнаружение включает несколько этапов, включая определение и сохранение данных ключа, отбора вниз и просмотра данных и создания данных в суд.</span><span class="sxs-lookup"><span data-stu-id="be401-106">Discovery consists of several phases, including identifying and preserving key data, culling down and reviewing the data, and producing data in court.</span></span> <span data-ttu-id="be401-107">запросов обнаружения электронных данных упростить процесс обнаружения с указанием одного обнаружения рабочего процесса в Exchange и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="be401-107">eDiscovery queries facilitate the discovery process by providing a single discovery workflow across Exchange and SharePoint.</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="be401-108">Операции обнаружения электронных данных</span><span class="sxs-lookup"><span data-stu-id="be401-108">eDiscovery operations</span></span>

<span data-ttu-id="be401-109">Функциональные возможности обнаружения электронных данных, взаимодействующий с веб-служб Exchange доступен через операции, введенные в Exchange Online, Exchange Online как часть Office 365 и версии Exchange, начиная с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="be401-109">The eDiscovery functionality that is exposed by EWS is available via operations introduced in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013.</span></span> 
  
<span data-ttu-id="be401-110">**В таблице 1. Новых операций для обнаружения электронных данных**</span><span class="sxs-lookup"><span data-stu-id="be401-110">**Table 1. New operations for eDiscovery**</span></span>

|<span data-ttu-id="be401-111">**Имя операции**</span><span class="sxs-lookup"><span data-stu-id="be401-111">**Operation name**</span></span>|<span data-ttu-id="be401-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be401-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be401-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="be401-113">GetDiscoverySearchConfiguration</span></span>](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |<span data-ttu-id="be401-114">Получает данные конфигурации для удержания на месте, сохраненные операций поиска обнаружения и почтовые ящики, которые разрешены для поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="be401-114">Gets configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span>  <br/> |
|[<span data-ttu-id="be401-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="be401-115">GetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |<span data-ttu-id="be401-116">Получает состояние запроса на удержание, которая задается с помощью [операции SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="be401-116">Gets the status of a query-based hold, which is set by using the [SetHoldOnMailboxes operation](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span></span>  <br/> |
|[<span data-ttu-id="be401-117">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="be401-117">GetNonIndexableItemDetails</span></span>](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |<span data-ttu-id="be401-118">Извлекает сведения об элементах, которые не могут быть индексированы.</span><span class="sxs-lookup"><span data-stu-id="be401-118">Retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="be401-119">Это включает в себя, но не ограничивается идентификатор элемента, код ошибки, описание ошибки при попытке индексировать элемент, а также дополнительные сведения о файле.</span><span class="sxs-lookup"><span data-stu-id="be401-119">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span>  <br/> |
|[<span data-ttu-id="be401-120">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="be401-120">GetNonIndexableItemStatistics</span></span>](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |<span data-ttu-id="be401-121">Получает число элементов, которые не могут быть индексированы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="be401-121">Retrieves the count of items that cannot be indexed in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="be401-122">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="be401-122">GetSearchableMailboxes</span></span>](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |<span data-ttu-id="be401-123">Получает список почтовых ящиков, который имеет разрешение на поиска или обнаружения электронных данных на клиенте.</span><span class="sxs-lookup"><span data-stu-id="be401-123">Gets a list of mailboxes that the client has permission to search or perform eDiscovery on.</span></span>  <br/> |
|[<span data-ttu-id="be401-124">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="be401-124">SearchMailboxes</span></span>](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |<span data-ttu-id="be401-125">Выполняет поиск элементов в определенных почтовых ящиков, которые соответствуют ключевые слова запроса.</span><span class="sxs-lookup"><span data-stu-id="be401-125">Searches for items in specific mailboxes that match query keywords.</span></span>  <br/> |
|[<span data-ttu-id="be401-126">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="be401-126">SetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |<span data-ttu-id="be401-127">Наборы на основе запроса содержат элементы.</span><span class="sxs-lookup"><span data-stu-id="be401-127">Sets a query-based hold on items.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be401-128">См. также</span><span class="sxs-lookup"><span data-stu-id="be401-128">See also</span></span>

- [<span data-ttu-id="be401-129">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="be401-129">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="be401-130">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="be401-130">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="be401-131">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="be401-131">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

