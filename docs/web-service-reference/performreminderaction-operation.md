---
title: Операция PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Найдите сведения о веб-служб Exchange PerformReminderAction операции.
ms.openlocfilehash: 778fbb508413721f58cfcf9143a5296874e6cd1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834722"
---
# <a name="performreminderaction-operation"></a><span data-ttu-id="b0fe0-103">Операция PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b0fe0-103">PerformReminderAction operation</span></span>

<span data-ttu-id="b0fe0-104">Найдите сведения о **PerformReminderAction** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-104">Find information about the **PerformReminderAction** EWS operation.</span></span> 
  
<span data-ttu-id="b0fe0-105">Операции веб-служб Exchange (EWS) **PerformReminderAction** инициирует действие прекратить или отложить на оповещение.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-105">The **PerformReminderAction** Exchange Web Services (EWS) operation initiates a dismiss or snooze action on a reminder.</span></span> 
  
<span data-ttu-id="b0fe0-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-performreminderaction-operation"></a><span data-ttu-id="b0fe0-107">С помощью операции PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b0fe0-107">Using the PerformReminderAction operation</span></span>

<span data-ttu-id="b0fe0-108">Чтобы закрыть или отложить напоминания (задержка), возвращенные операцией [GetReminders](getreminders-operation.md) можно использовать операцию **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="b0fe0-108">You can use the **PerformReminderAction** operation to dismiss or snooze (delay) reminders returned by the [GetReminders](getreminders-operation.md) operation.</span></span> <span data-ttu-id="b0fe0-109">Чтобы отложить напоминание, установите [Тип действия](actiontype-reminderactiontype.md) в **отложить**и задайте [NewReminderTime](newremindertime.md) значение времени в более поздней версии, чем текущий [ReminderTime](remindertime.md)в противном случае **NewReminderTime** игнорируется сервером.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-109">To snooze a reminder, set the [ActionType](actiontype-reminderactiontype.md) to **Snooze**, and set the [NewReminderTime](newremindertime.md) value to a time later than the current [ReminderTime](remindertime.md), otherwise the **NewReminderTime** is ignored by the server.</span></span> <span data-ttu-id="b0fe0-110">Если оповещение — это вхождение повторяющееся собрание и **отложить** действий на напоминание с **NewReminderTime** , находящегося за напоминание следующее вхождение, напоминания эффективно закрывается.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-110">If the reminder is for an occurrence of a recurring meeting, and the **Snooze** action is taken on the reminder with a **NewReminderTime** that is past the reminder of the next occurrence, the reminder is effectively dismissed.</span></span> 
  
<span data-ttu-id="b0fe0-111">Чтобы отключить напоминание, задайте значение **Прекратить** **Тип действия** .</span><span class="sxs-lookup"><span data-stu-id="b0fe0-111">To dismiss a reminder, set the **ActionType** to **Dismiss**.</span></span> <span data-ttu-id="b0fe0-112">Когда сервер обрабатывает запрос, сервер изменяется значение [IsReminderSet](isreminderset.md) для элемента с **значение True,** значение **False**.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-112">When the server processes the request, the server changes the [IsReminderSet](isreminderset.md) value for the item from **True** to **False**.</span></span>
  
### <a name="performreminderaction-operation-soap-headers"></a><span data-ttu-id="b0fe0-113">Заголовки SOAP PerformReminderAction операции</span><span class="sxs-lookup"><span data-stu-id="b0fe0-113">PerformReminderAction operation SOAP headers</span></span>

<span data-ttu-id="b0fe0-114">Операция **PerformReminderAction** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-114">The **PerformReminderAction** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b0fe0-115">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="b0fe0-115">**Header name**</span></span>|<span data-ttu-id="b0fe0-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0fe0-116">**Element**</span></span>|<span data-ttu-id="b0fe0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0fe0-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b0fe0-118">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="b0fe0-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="b0fe0-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="b0fe0-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b0fe0-120">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="b0fe0-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b0fe0-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="b0fe0-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="b0fe0-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="b0fe0-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b0fe0-124">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="b0fe0-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b0fe0-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="b0fe0-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b0fe0-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b0fe0-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b0fe0-128">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b0fe0-129">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b0fe0-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="b0fe0-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b0fe0-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b0fe0-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b0fe0-132">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b0fe0-133">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a><span data-ttu-id="b0fe0-134">Пример запроса PerformReminderAction операции</span><span class="sxs-lookup"><span data-stu-id="b0fe0-134">PerformReminderAction operation request example</span></span>

<span data-ttu-id="b0fe0-135">В следующем примере запрос операции **PerformReminderAction** показано, как отложить текущего напоминание и задать новый время оповещения.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-135">The following example of a **PerformReminderAction** operation request shows how to snooze a current reminder and set a new reminder time.</span></span> <span data-ttu-id="b0fe0-136">Обратите внимание на то, что вам нужно включить **ChangeKey** для [ItemId](itemid.md) и **NewReminderTime** должен иметь значение времени в более поздней версии, чем **ReminderTime** , возвращенные операцией [GetReminders](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b0fe0-136">Note that you need to include the **ChangeKey** for the [ItemId](itemid.md) and the **NewReminderTime** must be set to a time later than the **ReminderTime** returned by the [GetReminders](getreminders-operation.md) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:PerformReminderAction>
      <m:ReminderItemActions>
        <t:ReminderItemAction>
          <t:ActionType>Snooze</t:ActionType>
          <t:ItemId Id="vwAAAA=="
           ChangeKey="DwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAUDA=="/>
          <t:NewReminderTime>2014-04-16T17:00:00Z</t:NewReminderTime>
        </t:ReminderItemAction>
      </m:ReminderItemActions>
    </m:PerformReminderAction>
  </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> <span data-ttu-id="b0fe0-137">Значение **ItemId** был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-137">The **ItemId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="b0fe0-138">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b0fe0-138">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b0fe0-139">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b0fe0-139">PerformReminderAction</span></span>](performreminderaction.md)
    
- [<span data-ttu-id="b0fe0-140">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="b0fe0-140">ReminderItemActions</span></span>](reminderitemactions.md)
    
- [<span data-ttu-id="b0fe0-141">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="b0fe0-141">ReminderItemAction</span></span>](reminderitemaction.md)
    
- [<span data-ttu-id="b0fe0-142">Тип действия</span><span class="sxs-lookup"><span data-stu-id="b0fe0-142">ActionType</span></span>](actiontype-reminderactiontype.md)
    
- [<span data-ttu-id="b0fe0-143">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="b0fe0-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b0fe0-144">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="b0fe0-144">NewReminderTime</span></span>](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a><span data-ttu-id="b0fe0-145">Успешные операции ответа PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b0fe0-145">Successful PerformReminderAction operation response</span></span>

<span data-ttu-id="b0fe0-146">В следующем примере показано успешного ответа на запрос операции **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="b0fe0-146">The following example shows a successful response to a **PerformReminderAction** operation request.</span></span> <span data-ttu-id="b0fe0-147">Элемент **UpdatedItemIds** содержит **что ItemID** элемента обновленные календаря.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-147">The **UpdatedItemIds** element contains the **ItemIds** of the updated calendar item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b0fe0-148">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b0fe0-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b0fe0-149">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="b0fe0-149">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="b0fe0-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b0fe0-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b0fe0-151">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="b0fe0-151">UpdatedItemIds</span></span>](updateditemids.md)
    
- [<span data-ttu-id="b0fe0-152">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="b0fe0-152">ItemId</span></span>](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a><span data-ttu-id="b0fe0-153">Пример ответа об ошибке PerformReminderAction операции</span><span class="sxs-lookup"><span data-stu-id="b0fe0-153">PerformReminderAction operation error response example</span></span>

<span data-ttu-id="b0fe0-154">В следующем примере показано ответа на запрос операции **PerformReminderAction** , когда не изменений на сервере.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-154">The following example shows a response to a **PerformReminderAction** operation request when no change was made on the server.</span></span> <span data-ttu-id="b0fe0-155">Это ответ был отправлен запрос, но не **UpdatedItemIds** не возвращено, что означает, что нет напоминаний были изменены.</span><span class="sxs-lookup"><span data-stu-id="b0fe0-155">This is a response in which a request was sent, but no **UpdatedItemIds** were returned, meaning no reminders were changed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b0fe0-156">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b0fe0-156">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b0fe0-157">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="b0fe0-157">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="b0fe0-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b0fe0-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b0fe0-159">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="b0fe0-159">UpdatedItemIds</span></span>](updateditemids.md)
    
<span data-ttu-id="b0fe0-160">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="b0fe0-160">For additional error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b0fe0-161">См. также</span><span class="sxs-lookup"><span data-stu-id="b0fe0-161">See also</span></span>


- [<span data-ttu-id="b0fe0-162">Операция GetReminders</span><span class="sxs-lookup"><span data-stu-id="b0fe0-162">GetReminders operation</span></span>](getreminders-operation.md)
    

