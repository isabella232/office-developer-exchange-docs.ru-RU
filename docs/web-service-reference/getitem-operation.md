---
title: GetItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Найдите сведения о веб-служб Exchange GetItem операции.
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762834"
---
# <a name="getitem-operation"></a><span data-ttu-id="09945-103">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="09945-103">GetItem operation</span></span>

<span data-ttu-id="09945-104">Найдите сведения о операции **GetItem** веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="09945-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="09945-105">Операции **GetItem** получает элементы из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="09945-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="09945-106">С помощью операции GetItem</span><span class="sxs-lookup"><span data-stu-id="09945-106">Using the GetItem operation</span></span>

<span data-ttu-id="09945-107">Операции **GetItem** Возвращает множество свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="09945-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="09945-108">Свойства, возвращаемые в ответ **GetItem** различаться в зависимости от запрошенного фигуры возвращать запрошенный дополнительных свойств и типа элемента.</span><span class="sxs-lookup"><span data-stu-id="09945-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="09945-109">Элементы [сообщения](message-ex15websvcsotherref.md) представляют сообщения электронной почты и другие элементы, которые не строго типизированные схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="09945-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="09945-110">Элементы, такие как IPM. Общий доступ и IPM.InfoPath возвращаются в виде элементы [сообщения](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="09945-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="09945-111">Exchange не возвращает [базовый элемент](item.md) в ответы.</span><span class="sxs-lookup"><span data-stu-id="09945-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="09945-112">Операции **GetItem** не возвращает вложения.</span><span class="sxs-lookup"><span data-stu-id="09945-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="09945-113">Возвращает метаданные о вложенного элемента или файла.</span><span class="sxs-lookup"><span data-stu-id="09945-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="09945-114">Чтобы вернуть вложение, с помощью [операции GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="09945-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="09945-115">Заголовки SOAP операции GetItem</span><span class="sxs-lookup"><span data-stu-id="09945-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="09945-116">Операции **GetItem** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="09945-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="09945-117">Заголовок \*\*\*</span><span class="sxs-lookup"><span data-stu-id="09945-117">****Header****</span></span>|<span data-ttu-id="09945-118">****Element****</span><span class="sxs-lookup"><span data-stu-id="09945-118">****Element****</span></span>|<span data-ttu-id="09945-119">****Описание****</span><span class="sxs-lookup"><span data-stu-id="09945-119">****Description****</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="09945-120">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="09945-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="09945-121">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="09945-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="09945-122">Указывает разрешение значения времени и данных в ответов с сервера, в секундах или в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="09945-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="09945-123">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="09945-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="09945-124">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="09945-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="09945-125">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="09945-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="09945-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="09945-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="09945-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="09945-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="09945-128">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="09945-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="09945-129">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="09945-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="09945-130">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="09945-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="09945-131">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="09945-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="09945-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="09945-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="09945-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="09945-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="09945-134">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="09945-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="09945-135">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="09945-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="09945-136">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="09945-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="09945-137">Определяет часовой пояс, который будет использоваться для всех ответов с сервера.</span><span class="sxs-lookup"><span data-stu-id="09945-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="09945-138">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="09945-138">In This Section</span></span>

[<span data-ttu-id="09945-139">Операции GetItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="09945-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="09945-140">Операции GetItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="09945-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="09945-141">Операции GetItem (задача)</span><span class="sxs-lookup"><span data-stu-id="09945-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="09945-142">Операции GetItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="09945-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="09945-143">См. также</span><span class="sxs-lookup"><span data-stu-id="09945-143">See also</span></span>



[<span data-ttu-id="09945-144">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="09945-144">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

