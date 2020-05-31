---
title: Операция GetItem
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
description: Найдите сведения о операции GetItem EWS.
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762834"
---
# <a name="getitem-operation"></a><span data-ttu-id="b1030-103">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="b1030-103">GetItem operation</span></span>

<span data-ttu-id="b1030-104">Найдите сведения о операции **GetItem** EWS.</span><span class="sxs-lookup"><span data-stu-id="b1030-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="b1030-105">Операция **GetItem** возвращает элементы из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1030-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="b1030-106">Использование операции GetItem</span><span class="sxs-lookup"><span data-stu-id="b1030-106">Using the GetItem operation</span></span>

<span data-ttu-id="b1030-107">Операция **GetItem** возвращает множество свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="b1030-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="b1030-108">Свойства, возвращаемые в ответе **GetItem** , зависят от запрошенной фигуры, запрашивают дополнительные свойства и тип возвращаемого элемента.</span><span class="sxs-lookup"><span data-stu-id="b1030-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="b1030-109">Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все другие элементы, которые не являются строго типизированными схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="b1030-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="b1030-110">Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов [Message](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="b1030-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="b1030-111">Exchange не возвращает элемент базового [элемента](item.md) в ответах.</span><span class="sxs-lookup"><span data-stu-id="b1030-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="b1030-112">Операция **GetItem** не возвращает вложения.</span><span class="sxs-lookup"><span data-stu-id="b1030-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="b1030-113">Он возвращает метаданные о вложенном элементе или файле.</span><span class="sxs-lookup"><span data-stu-id="b1030-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="b1030-114">Чтобы вернуть вложение, используйте [операцию GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b1030-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="b1030-115">Заголовки SOAP для операции GetItem</span><span class="sxs-lookup"><span data-stu-id="b1030-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="b1030-116">Операция **GetItem** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="b1030-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b1030-117">Header \* \* \* \*</span><span class="sxs-lookup"><span data-stu-id="b1030-117">\*\*\*\*Header\*\*\*\*</span></span>|<span data-ttu-id="b1030-118">\*\*\*\*Element\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="b1030-118">\*\*\*\*Element\*\*\*\*</span></span>|<span data-ttu-id="b1030-119">\*\*\*\*Описание\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="b1030-119">\*\*\*\*Description\*\*\*\*</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b1030-120">**датетимепреЦисион**</span><span class="sxs-lookup"><span data-stu-id="b1030-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="b1030-121">датетимепреЦисион</span><span class="sxs-lookup"><span data-stu-id="b1030-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="b1030-122">Задает разрешение значений данных и времени в ответах от сервера: в секундах или в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="b1030-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="b1030-123">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="b1030-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="b1030-124">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="b1030-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b1030-125">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="b1030-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="b1030-126">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="b1030-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="b1030-127">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="b1030-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b1030-128">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b1030-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="b1030-129">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="b1030-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b1030-130">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="b1030-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b1030-131">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="b1030-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="b1030-132">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="b1030-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b1030-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b1030-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b1030-134">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="b1030-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="b1030-135">**тимезонеконтекст**</span><span class="sxs-lookup"><span data-stu-id="b1030-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="b1030-136">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="b1030-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="b1030-137">Определяет часовой пояс, который будет использоваться для всех ответов сервера.</span><span class="sxs-lookup"><span data-stu-id="b1030-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="b1030-138">Содержание</span><span class="sxs-lookup"><span data-stu-id="b1030-138">In This Section</span></span>

[<span data-ttu-id="b1030-139">Операция GetItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="b1030-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="b1030-140">Операция GetItem (элемент календаря)</span><span class="sxs-lookup"><span data-stu-id="b1030-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="b1030-141">Операция GetItem (задача)</span><span class="sxs-lookup"><span data-stu-id="b1030-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="b1030-142">Операция GetItem (контакт)</span><span class="sxs-lookup"><span data-stu-id="b1030-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="b1030-143">См. также</span><span class="sxs-lookup"><span data-stu-id="b1030-143">See also</span></span>



[<span data-ttu-id="b1030-144">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="b1030-144">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

