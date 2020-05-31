---
title: обнаружение электронных данных в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Сведения об обнаружении электронных данных в EWS в Exchange.
ms.openlocfilehash: 6491fdd9f2246870a89bfa89bf7d97b972d67c92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760939"
---
# <a name="ediscovery-in-ews-in-exchange"></a><span data-ttu-id="2717c-103">обнаружение электронных данных в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="2717c-103">eDiscovery in EWS in Exchange</span></span>

<span data-ttu-id="2717c-104">Сведения об обнаружении электронных данных в EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2717c-104">Learn about eDiscovery in EWS in Exchange.</span></span>
  
<span data-ttu-id="2717c-105">Обнаружение электронных данных — это веб-служба федеративных запросов, которая позволяет внешним приложениям выполнять запросы данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="2717c-105">eDiscovery is a federated query web service that enables external applications to perform queries of Exchange data.</span></span>
  
<span data-ttu-id="2717c-106">Обнаружение состоит из нескольких этапов, в том числе определения и сохранения данных ключей, отбора и просмотра данных, а также создания данных в суд.</span><span class="sxs-lookup"><span data-stu-id="2717c-106">Discovery consists of several phases, including identifying and preserving key data, culling down and reviewing the data, and producing data in court.</span></span> <span data-ttu-id="2717c-107">запросы eDiscovery упрощают процесс обнаружения, предоставляя единый рабочий процесс обнаружения в Exchange и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2717c-107">eDiscovery queries facilitate the discovery process by providing a single discovery workflow across Exchange and SharePoint.</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="2717c-108">Операции обнаружения электронных данных</span><span class="sxs-lookup"><span data-stu-id="2717c-108">eDiscovery operations</span></span>

<span data-ttu-id="2717c-109">Функции обнаружения электронных данных, предоставляемые EWS, доступны с помощью операций, представленных в Exchange Online, Exchange Online в составе Office 365, и версий Exchange, начинающихся с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="2717c-109">The eDiscovery functionality that is exposed by EWS is available via operations introduced in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013.</span></span> 
  
<span data-ttu-id="2717c-110">**Таблица 1. Новые операции обнаружения электронных данных**</span><span class="sxs-lookup"><span data-stu-id="2717c-110">**Table 1. New operations for eDiscovery**</span></span>

|<span data-ttu-id="2717c-111">**Имя операции**</span><span class="sxs-lookup"><span data-stu-id="2717c-111">**Operation name**</span></span>|<span data-ttu-id="2717c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2717c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2717c-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="2717c-113">GetDiscoverySearchConfiguration</span></span>](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |<span data-ttu-id="2717c-114">Получает сведения о конфигурации для удержаний на месте, сохраненных поисков и почтовых ящиков, которые включены для поиска при обнаружении.</span><span class="sxs-lookup"><span data-stu-id="2717c-114">Gets configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span>  <br/> |
|[<span data-ttu-id="2717c-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="2717c-115">GetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |<span data-ttu-id="2717c-116">Получает состояние хранения на основе запроса, которое задается с помощью [операции SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2717c-116">Gets the status of a query-based hold, which is set by using the [SetHoldOnMailboxes operation](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span></span>  <br/> |
|[<span data-ttu-id="2717c-117">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="2717c-117">GetNonIndexableItemDetails</span></span>](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |<span data-ttu-id="2717c-118">Получает сведения о элементах, которые не удается индексировать.</span><span class="sxs-lookup"><span data-stu-id="2717c-118">Retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="2717c-119">Это относится только к идентификатору элемента, к коду ошибки, описанию ошибки, при попытке индексирования элемента и дополнительной информации о файле.</span><span class="sxs-lookup"><span data-stu-id="2717c-119">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span>  <br/> |
|[<span data-ttu-id="2717c-120">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="2717c-120">GetNonIndexableItemStatistics</span></span>](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |<span data-ttu-id="2717c-121">Получает количество элементов, которые не удается индексировать в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="2717c-121">Retrieves the count of items that cannot be indexed in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2717c-122">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="2717c-122">GetSearchableMailboxes</span></span>](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |<span data-ttu-id="2717c-123">Получает список почтовых ящиков, у которых у клиента есть разрешение на поиск и выполнение обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="2717c-123">Gets a list of mailboxes that the client has permission to search or perform eDiscovery on.</span></span>  <br/> |
|[<span data-ttu-id="2717c-124">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="2717c-124">SearchMailboxes</span></span>](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |<span data-ttu-id="2717c-125">Ищет элементы в определенных почтовых ящиках, которые совпадают с ключевыми словами запроса.</span><span class="sxs-lookup"><span data-stu-id="2717c-125">Searches for items in specific mailboxes that match query keywords.</span></span>  <br/> |
|[<span data-ttu-id="2717c-126">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="2717c-126">SetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |<span data-ttu-id="2717c-127">Задает для элементов удержание на основе запроса.</span><span class="sxs-lookup"><span data-stu-id="2717c-127">Sets a query-based hold on items.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2717c-128">См. также</span><span class="sxs-lookup"><span data-stu-id="2717c-128">See also</span></span>

- [<span data-ttu-id="2717c-129">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="2717c-129">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="2717c-130">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="2717c-130">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="2717c-131">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="2717c-131">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

