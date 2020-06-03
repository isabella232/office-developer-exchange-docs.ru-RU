---
title: Операция PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Поиск сведений о PerformReminderActionной операции EWS.
ms.openlocfilehash: 4c069d541e9a42167c447a50c405399958d3608d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462292"
---
# <a name="performreminderaction-operation"></a><span data-ttu-id="0ba4e-103">Операция PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="0ba4e-103">PerformReminderAction operation</span></span>

<span data-ttu-id="0ba4e-104">Поиск сведений о **PerformReminderActionной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-104">Find information about the **PerformReminderAction** EWS operation.</span></span> 
  
<span data-ttu-id="0ba4e-105">Операция **PerformReminderAction** веб-служб Exchange (EWS) запускает действие отклонить или отложить отложить напоминание.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-105">The **PerformReminderAction** Exchange Web Services (EWS) operation initiates a dismiss or snooze action on a reminder.</span></span> 
  
<span data-ttu-id="0ba4e-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-performreminderaction-operation"></a><span data-ttu-id="0ba4e-107">Использование операции PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="0ba4e-107">Using the PerformReminderAction operation</span></span>

<span data-ttu-id="0ba4e-108">Вы можете использовать операцию **PerformReminderAction** , чтобы отклонить или отложить напоминания, возвращенные операцией- [напоминаний](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0ba4e-108">You can use the **PerformReminderAction** operation to dismiss or snooze (delay) reminders returned by the [GetReminders](getreminders-operation.md) operation.</span></span> <span data-ttu-id="0ba4e-109">Чтобы отложить напоминание, установите для [объекта, который следует](actiontype-reminderactiontype.md) **отложить**, и задайте для параметра [Невреминдертиме](newremindertime.md) значение времени позже текущего [ReminderTime](remindertime.md), в противном случае **невреминдертиме** игнорируется сервером.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-109">To snooze a reminder, set the [ActionType](actiontype-reminderactiontype.md) to **Snooze**, and set the [NewReminderTime](newremindertime.md) value to a time later than the current [ReminderTime](remindertime.md), otherwise the **NewReminderTime** is ignored by the server.</span></span> <span data-ttu-id="0ba4e-110">Если напоминание относится к экземпляру повторяющегося собрания, а действие " **отложить** " выполняется в памятке с **невреминдертиме** , которое пройдет за сообщение о следующем повторении, то напоминание отменяется.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-110">If the reminder is for an occurrence of a recurring meeting, and the **Snooze** action is taken on the reminder with a **NewReminderTime** that is past the reminder of the next occurrence, the reminder is effectively dismissed.</span></span> 
  
<span data-ttu-id="0ba4e-111">Чтобы отклонить напоминание, задайте для **параметра "объект" значение "** **отклонено**".</span><span class="sxs-lookup"><span data-stu-id="0ba4e-111">To dismiss a reminder, set the **ActionType** to **Dismiss**.</span></span> <span data-ttu-id="0ba4e-112">Когда сервер обрабатывает запрос, сервер изменяет значение параметра [напоминания](isreminderset.md) для элемента с **true** на **false**.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-112">When the server processes the request, the server changes the [IsReminderSet](isreminderset.md) value for the item from **True** to **False**.</span></span>
  
### <a name="performreminderaction-operation-soap-headers"></a><span data-ttu-id="0ba4e-113">Заголовки SOAP операции PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="0ba4e-113">PerformReminderAction operation SOAP headers</span></span>

<span data-ttu-id="0ba4e-114">Операция **PerformReminderAction** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-114">The **PerformReminderAction** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0ba4e-115">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="0ba4e-115">**Header name**</span></span>|<span data-ttu-id="0ba4e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0ba4e-116">**Element**</span></span>|<span data-ttu-id="0ba4e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ba4e-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0ba4e-118">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="0ba4e-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="0ba4e-119">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="0ba4e-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="0ba4e-120">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="0ba4e-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ba4e-122">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="0ba4e-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="0ba4e-123">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="0ba4e-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="0ba4e-124">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="0ba4e-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ba4e-126">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="0ba4e-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0ba4e-127">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="0ba4e-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0ba4e-128">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0ba4e-129">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ba4e-130">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="0ba4e-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0ba4e-131">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="0ba4e-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0ba4e-132">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0ba4e-133">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a><span data-ttu-id="0ba4e-134">Пример запроса операции PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="0ba4e-134">PerformReminderAction operation request example</span></span>

<span data-ttu-id="0ba4e-135">В следующем примере запроса операции **PerformReminderAction** показано, как отложить текущее напоминание и задать новое время оповещения.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-135">The following example of a **PerformReminderAction** operation request shows how to snooze a current reminder and set a new reminder time.</span></span> <span data-ttu-id="0ba4e-136">Обратите внимание, что необходимо включить **чанжекэй** для элемента [ItemId](itemid.md) , а для параметра **невреминдертиме** необходимо задать время позже, чем **ReminderTime** [, возвращенное операцией](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0ba4e-136">Note that you need to include the **ChangeKey** for the [ItemId](itemid.md) and the **NewReminderTime** must be set to a time later than the **ReminderTime** returned by the [GetReminders](getreminders-operation.md) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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
> <span data-ttu-id="0ba4e-137">Значение **ItemId** было сокращено, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-137">The **ItemId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="0ba4e-138">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0ba4e-138">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ba4e-139">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="0ba4e-139">PerformReminderAction</span></span>](performreminderaction.md)
    
- [<span data-ttu-id="0ba4e-140">реминдеритемактионс</span><span class="sxs-lookup"><span data-stu-id="0ba4e-140">ReminderItemActions</span></span>](reminderitemactions.md)
    
- [<span data-ttu-id="0ba4e-141">реминдеритемактион</span><span class="sxs-lookup"><span data-stu-id="0ba4e-141">ReminderItemAction</span></span>](reminderitemaction.md)
    
- [<span data-ttu-id="0ba4e-142">ActionType</span><span class="sxs-lookup"><span data-stu-id="0ba4e-142">ActionType</span></span>](actiontype-reminderactiontype.md)
    
- [<span data-ttu-id="0ba4e-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="0ba4e-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="0ba4e-144">невреминдертиме</span><span class="sxs-lookup"><span data-stu-id="0ba4e-144">NewReminderTime</span></span>](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a><span data-ttu-id="0ba4e-145">Успешный отклик операции PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="0ba4e-145">Successful PerformReminderAction operation response</span></span>

<span data-ttu-id="0ba4e-146">В следующем примере показан успешный ответ на запрос операции **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="0ba4e-146">The following example shows a successful response to a **PerformReminderAction** operation request.</span></span> <span data-ttu-id="0ba4e-147">Элемент **упдатедитемидс** содержит **итемидс** обновленного элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-147">The **UpdatedItemIds** element contains the **ItemIds** of the updated calendar item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0ba4e-148">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0ba4e-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ba4e-149">перформреминдерактионреспонсе</span><span class="sxs-lookup"><span data-stu-id="0ba4e-149">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="0ba4e-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0ba4e-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0ba4e-151">упдатедитемидс</span><span class="sxs-lookup"><span data-stu-id="0ba4e-151">UpdatedItemIds</span></span>](updateditemids.md)
    
- [<span data-ttu-id="0ba4e-152">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="0ba4e-152">ItemId</span></span>](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a><span data-ttu-id="0ba4e-153">Пример ответа на сообщение об ошибке операции PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="0ba4e-153">PerformReminderAction operation error response example</span></span>

<span data-ttu-id="0ba4e-154">В следующем примере показан ответ на запрос операции **PerformReminderAction** , если на сервере не было внесено никаких изменений.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-154">The following example shows a response to a **PerformReminderAction** operation request when no change was made on the server.</span></span> <span data-ttu-id="0ba4e-155">Это ответ, в котором был отправлен запрос, но не было возвращено ни одного **упдатедитемидс** , что означает, что напоминания не были изменены.</span><span class="sxs-lookup"><span data-stu-id="0ba4e-155">This is a response in which a request was sent, but no **UpdatedItemIds** were returned, meaning no reminders were changed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0ba4e-156">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0ba4e-156">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ba4e-157">перформреминдерактионреспонсе</span><span class="sxs-lookup"><span data-stu-id="0ba4e-157">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="0ba4e-158">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0ba4e-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0ba4e-159">упдатедитемидс</span><span class="sxs-lookup"><span data-stu-id="0ba4e-159">UpdatedItemIds</span></span>](updateditemids.md)
    
<span data-ttu-id="0ba4e-160">Дополнительные коды ошибок, являющиеся общими для EWS, можно найти в статье [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="0ba4e-160">For additional error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0ba4e-161">См. также</span><span class="sxs-lookup"><span data-stu-id="0ba4e-161">See also</span></span>


- [<span data-ttu-id="0ba4e-162">Операция GetReminders</span><span class="sxs-lookup"><span data-stu-id="0ba4e-162">GetReminders operation</span></span>](getreminders-operation.md)
    

