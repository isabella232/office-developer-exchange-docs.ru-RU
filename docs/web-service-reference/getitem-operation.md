---
title: Операция GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Найдите сведения о операции GetItem EWS.
localization_priority: Priority
ms.openlocfilehash: 8871dde183974454fc27dbddda489e6b0a70f3aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463330"
---
# <a name="getitem-operation"></a><span data-ttu-id="2567d-103">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="2567d-103">GetItem operation</span></span>

<span data-ttu-id="2567d-104">Найдите сведения о операции **GetItem** EWS.</span><span class="sxs-lookup"><span data-stu-id="2567d-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="2567d-105">Операция **GetItem** возвращает элементы из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="2567d-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="2567d-106">Использование операции GetItem</span><span class="sxs-lookup"><span data-stu-id="2567d-106">Using the GetItem operation</span></span>

<span data-ttu-id="2567d-107">Операция **GetItem** возвращает множество свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="2567d-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="2567d-108">Свойства, возвращаемые в ответе **GetItem** , зависят от запрошенной фигуры, запрашивают дополнительные свойства и тип возвращаемого элемента.</span><span class="sxs-lookup"><span data-stu-id="2567d-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="2567d-109">Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все другие элементы, которые не являются строго типизированными схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="2567d-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="2567d-110">Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов [Message](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="2567d-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="2567d-111">Exchange не возвращает элемент базового [элемента](item.md) в ответах.</span><span class="sxs-lookup"><span data-stu-id="2567d-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="2567d-112">Операция **GetItem** не возвращает вложения.</span><span class="sxs-lookup"><span data-stu-id="2567d-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="2567d-113">Он возвращает метаданные о вложенном элементе или файле.</span><span class="sxs-lookup"><span data-stu-id="2567d-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="2567d-114">Чтобы вернуть вложение, используйте [операцию GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2567d-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="2567d-115">Заголовки SOAP для операции GetItem</span><span class="sxs-lookup"><span data-stu-id="2567d-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="2567d-116">Операция **GetItem** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="2567d-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="2567d-117">Header \* \* \* \*</span><span class="sxs-lookup"><span data-stu-id="2567d-117">\*\*\*\*Header\*\*\*\*</span></span>|<span data-ttu-id="2567d-118">\*\*\*\*Element\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="2567d-118">\*\*\*\*Element\*\*\*\*</span></span>|<span data-ttu-id="2567d-119">\*\*\*\*Описание\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="2567d-119">\*\*\*\*Description\*\*\*\*</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2567d-120">**датетимепреЦисион**</span><span class="sxs-lookup"><span data-stu-id="2567d-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="2567d-121">датетимепреЦисион</span><span class="sxs-lookup"><span data-stu-id="2567d-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="2567d-122">Задает разрешение значений данных и времени в ответах от сервера: в секундах или в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="2567d-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="2567d-123">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="2567d-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="2567d-124">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="2567d-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2567d-125">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="2567d-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="2567d-126">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="2567d-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="2567d-127">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="2567d-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="2567d-128">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="2567d-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="2567d-129">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="2567d-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="2567d-130">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="2567d-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2567d-131">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="2567d-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="2567d-132">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="2567d-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="2567d-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="2567d-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2567d-134">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="2567d-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="2567d-135">**тимезонеконтекст**</span><span class="sxs-lookup"><span data-stu-id="2567d-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="2567d-136">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="2567d-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="2567d-137">Определяет часовой пояс, который будет использоваться для всех ответов сервера.</span><span class="sxs-lookup"><span data-stu-id="2567d-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="2567d-138">Содержание</span><span class="sxs-lookup"><span data-stu-id="2567d-138">In This Section</span></span>

[<span data-ttu-id="2567d-139">Операция GetItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="2567d-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="2567d-140">Операция GetItem (элемент календаря)</span><span class="sxs-lookup"><span data-stu-id="2567d-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="2567d-141">Операция GetItem (задача)</span><span class="sxs-lookup"><span data-stu-id="2567d-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="2567d-142">Операция GetItem (контакт)</span><span class="sxs-lookup"><span data-stu-id="2567d-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="2567d-143">См. также</span><span class="sxs-lookup"><span data-stu-id="2567d-143">See also</span></span>



[<span data-ttu-id="2567d-144">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="2567d-144">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

