---
title: Операция RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Найдите сведения о веб-служб Exchange RemoveContactFromImList операции.
ms.openlocfilehash: 036b295a84e86ad74c467572cc52fdf6bbae5191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835080"
---
# <a name="removecontactfromimlist-operation"></a><span data-ttu-id="00b96-103">Операция RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="00b96-103">RemoveContactFromImList operation</span></span>

<span data-ttu-id="00b96-104">Найдите сведения о **RemoveContactFromImList** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="00b96-104">Find information about the **RemoveContactFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="00b96-105">Операция **RemoveContactFromImList** удаляет контактов в списке обмен мгновенными сообщениями (IM) Lync при Lync с помощью Exchange хранилища контактов.</span><span class="sxs-lookup"><span data-stu-id="00b96-105">The **RemoveContactFromImList** operation removes contacts from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="00b96-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00b96-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removecontactfromimlist-operation"></a><span data-ttu-id="00b96-107">С помощью операции RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="00b96-107">Using the RemoveContactFromImList operation</span></span>

<span data-ttu-id="00b96-108">Операция **RemoveContactFromImList** принимает один аргумент, определяющий контакт, чтобы удалить из списка контактов Lync, хранящиеся на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="00b96-108">The **RemoveContactFromImList** operation accepts a single argument that identifies a contact to remove from the Lync contact list stored on an Exchange server.</span></span> <span data-ttu-id="00b96-109">В списке контактов, что эта операция целевых показателей вызывает **Контактов Lync** в Outlook 2013.</span><span class="sxs-lookup"><span data-stu-id="00b96-109">The list of contacts that this operation targets is called **Lync Contacts** in Outlook 2013.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="00b96-110">Не используйте [операцию DeleteItem](deleteitem-operation.md) удалить контакты из списка контактов.</span><span class="sxs-lookup"><span data-stu-id="00b96-110">Do not use the [DeleteItem operation](deleteitem-operation.md) to remove contacts from a contact list.</span></span> <span data-ttu-id="00b96-111">Дополнительной обработки на сервере может потребоваться возникают для поддержки при удалении контакта из списка **Контактов Lync** .</span><span class="sxs-lookup"><span data-stu-id="00b96-111">Additional server-side processing might have to occur to support removing a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="00b96-112">Обратите внимание, что список **Контактов Lync** концептуальные эквивалент папки почтовых ящиков **Контактов Lync** по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="00b96-112">Note that the **Lync Contacts** list is the conceptual equivalent of the default **Lync Contacts** mailbox folder.</span></span> 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a><span data-ttu-id="00b96-113">Заголовки SOAP RemoveContactFromImList операции</span><span class="sxs-lookup"><span data-stu-id="00b96-113">RemoveContactFromImList operation SOAP headers</span></span>

<span data-ttu-id="00b96-114">Операция **RemoveContactFromImList** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="00b96-114">The **RemoveContactFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="00b96-115">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="00b96-115">**Header name**</span></span>|<span data-ttu-id="00b96-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="00b96-116">**Element**</span></span>|<span data-ttu-id="00b96-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00b96-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="00b96-118">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="00b96-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="00b96-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="00b96-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="00b96-120">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="00b96-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="00b96-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="00b96-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="00b96-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="00b96-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="00b96-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="00b96-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="00b96-124">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="00b96-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="00b96-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="00b96-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="00b96-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="00b96-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="00b96-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="00b96-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="00b96-128">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="00b96-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="00b96-129">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="00b96-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="00b96-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="00b96-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="00b96-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="00b96-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="00b96-132">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="00b96-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="00b96-133">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="00b96-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a><span data-ttu-id="00b96-134">Пример запроса RemoveContactFromImList операции: удаление контакта из списка контактов Lync</span><span class="sxs-lookup"><span data-stu-id="00b96-134">RemoveContactFromImList operation request example: Remove a contact from the Lync Contacts list</span></span>

<span data-ttu-id="00b96-135">В следующем примере запрос операции **RemoveContactFromImList** показано, как удалить контакт из списка **Контактов Lync** .</span><span class="sxs-lookup"><span data-stu-id="00b96-135">The following example of a **RemoveContactFromImList** operation request shows how to remove a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="00b96-136">Операция **RemoveContactFromImList** принимает один уникальный идентификатор контакта для идентификации контакта, удаляется из списка **Контактов Lync** .</span><span class="sxs-lookup"><span data-stu-id="00b96-136">The **RemoveContactFromImList** operation accepts a single unique contact identifier to identify the contact that is removed from the **Lync Contacts** list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="00b96-137">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="00b96-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="00b96-138">В приглашении на SOAP body используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="00b96-138">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="00b96-139">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="00b96-139">RemoveContactFromImList</span></span>](removecontactfromimlist.md)
    
- [<span data-ttu-id="00b96-140">ContactId</span><span class="sxs-lookup"><span data-stu-id="00b96-140">ContactId</span></span>](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a><span data-ttu-id="00b96-141">Успешные операции ответа RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="00b96-141">Successful RemoveContactFromImList operation response</span></span>

<span data-ttu-id="00b96-142">В следующем примере показано успешного ответа на запрос операции **RemoveContactFromImList** , чтобы удалить контакт из списка **Контактов Lync** .</span><span class="sxs-lookup"><span data-stu-id="00b96-142">The following example shows a successful response to a **RemoveContactFromImList** operation request to remove a contact from the **Lync Contacts** list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="00b96-143">В ответе SOAP body используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="00b96-143">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="00b96-144">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="00b96-144">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="00b96-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="00b96-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a><span data-ttu-id="00b96-146">Ошибка операции RemoveContactFromImList ответа</span><span class="sxs-lookup"><span data-stu-id="00b96-146">RemoveContactFromImList operation error response</span></span>

<span data-ttu-id="00b96-147">В следующем примере показано ошибочный ответ на запрос операции **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="00b96-147">The following example shows an error response to a **RemoveContactFromImList** operation request.</span></span> <span data-ttu-id="00b96-148">Это ответ на запрос удаление контакта из списка **Контактов Lync** , когда контакт больше не существует в списке.</span><span class="sxs-lookup"><span data-stu-id="00b96-148">This is a response to a request to remove a contact from the **Lync Contacts** list when the contact no longer exists in the list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="00b96-149">В ответе ошибка SOAP body используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="00b96-149">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="00b96-150">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="00b96-150">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="00b96-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="00b96-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="00b96-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="00b96-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="00b96-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="00b96-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="00b96-154">См. также</span><span class="sxs-lookup"><span data-stu-id="00b96-154">See also</span></span>

- [<span data-ttu-id="00b96-155">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="00b96-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="00b96-156">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="00b96-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

