---
title: Операция RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Поиск сведений о RemoveContactFromImListной операции EWS.
ms.openlocfilehash: 8b3d83a0b53bad169d9f3478540e5087901f3a12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458469"
---
# <a name="removecontactfromimlist-operation"></a><span data-ttu-id="3f11b-103">Операция RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="3f11b-103">RemoveContactFromImList operation</span></span>

<span data-ttu-id="3f11b-104">Поиск сведений о **RemoveContactFromImListной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="3f11b-104">Find information about the **RemoveContactFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="3f11b-105">Операция **RemoveContactFromImList** удаляет контакты из списка мгновенных сообщений LYNC (IM), когда Lync использует Exchange для хранилища контактов.</span><span class="sxs-lookup"><span data-stu-id="3f11b-105">The **RemoveContactFromImList** operation removes contacts from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="3f11b-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3f11b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removecontactfromimlist-operation"></a><span data-ttu-id="3f11b-107">Использование операции RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="3f11b-107">Using the RemoveContactFromImList operation</span></span>

<span data-ttu-id="3f11b-108">Операция **RemoveContactFromImList** принимает один аргумент, который определяет контакт, который необходимо удалить из списка контактов Lync, хранящегося на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f11b-108">The **RemoveContactFromImList** operation accepts a single argument that identifies a contact to remove from the Lync contact list stored on an Exchange server.</span></span> <span data-ttu-id="3f11b-109">Список контактов, для которых предназначена эта операция, называется **Контакты Lync** в Outlook 2013.</span><span class="sxs-lookup"><span data-stu-id="3f11b-109">The list of contacts that this operation targets is called **Lync Contacts** in Outlook 2013.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="3f11b-110">Не используйте [операцию DeleteItem](deleteitem-operation.md) для удаления контактов из списка контактов.</span><span class="sxs-lookup"><span data-stu-id="3f11b-110">Do not use the [DeleteItem operation](deleteitem-operation.md) to remove contacts from a contact list.</span></span> <span data-ttu-id="3f11b-111">Для поддержки удаления контакта из списка **контактов Lync** может потребоваться дополнительная обработка на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="3f11b-111">Additional server-side processing might have to occur to support removing a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="3f11b-112">Обратите внимание, что список **контактов Lync** является концептуальным эквивалентом стандартной папки почтовых ящиков **контактов Lync** .</span><span class="sxs-lookup"><span data-stu-id="3f11b-112">Note that the **Lync Contacts** list is the conceptual equivalent of the default **Lync Contacts** mailbox folder.</span></span> 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a><span data-ttu-id="3f11b-113">Заголовки SOAP операции RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="3f11b-113">RemoveContactFromImList operation SOAP headers</span></span>

<span data-ttu-id="3f11b-114">Операция **RemoveContactFromImList** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="3f11b-114">The **RemoveContactFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="3f11b-115">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="3f11b-115">**Header name**</span></span>|<span data-ttu-id="3f11b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f11b-116">**Element**</span></span>|<span data-ttu-id="3f11b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f11b-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3f11b-118">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="3f11b-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="3f11b-119">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="3f11b-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3f11b-120">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="3f11b-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="3f11b-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="3f11b-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3f11b-122">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="3f11b-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="3f11b-123">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="3f11b-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="3f11b-124">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="3f11b-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="3f11b-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="3f11b-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3f11b-126">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="3f11b-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3f11b-127">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="3f11b-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3f11b-128">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="3f11b-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="3f11b-129">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="3f11b-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3f11b-130">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="3f11b-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3f11b-131">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="3f11b-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3f11b-132">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="3f11b-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="3f11b-133">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="3f11b-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a><span data-ttu-id="3f11b-134">Пример запроса операции RemoveContactFromImList: Удаление контакта из списка контактов Lync</span><span class="sxs-lookup"><span data-stu-id="3f11b-134">RemoveContactFromImList operation request example: Remove a contact from the Lync Contacts list</span></span>

<span data-ttu-id="3f11b-135">В следующем примере запроса операции **RemoveContactFromImList** показано, как удалить контакт из списка **контактов Lync** .</span><span class="sxs-lookup"><span data-stu-id="3f11b-135">The following example of a **RemoveContactFromImList** operation request shows how to remove a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="3f11b-136">Операция **RemoveContactFromImList** принимает один уникальный идентификатор контакта для идентификации контакта, который удален из списка **контактов Lync** .</span><span class="sxs-lookup"><span data-stu-id="3f11b-136">The **RemoveContactFromImList** operation accepts a single unique contact identifier to identify the contact that is removed from the **Lync Contacts** list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3f11b-137">Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="3f11b-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="3f11b-138">В теле SOAP запроса используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3f11b-138">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="3f11b-139">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="3f11b-139">RemoveContactFromImList</span></span>](removecontactfromimlist.md)
    
- [<span data-ttu-id="3f11b-140">ContactId</span><span class="sxs-lookup"><span data-stu-id="3f11b-140">ContactId</span></span>](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a><span data-ttu-id="3f11b-141">Успешный отклик операции RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="3f11b-141">Successful RemoveContactFromImList operation response</span></span>

<span data-ttu-id="3f11b-142">В следующем примере показан успешный ответ на запрос операции **RemoveContactFromImList** для удаления контакта из списка **контактов Lync** .</span><span class="sxs-lookup"><span data-stu-id="3f11b-142">The following example shows a successful response to a **RemoveContactFromImList** operation request to remove a contact from the **Lync Contacts** list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3f11b-143">В теле SOAP отклика используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3f11b-143">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="3f11b-144">ремовеконтактфромимлистреспонсе</span><span class="sxs-lookup"><span data-stu-id="3f11b-144">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="3f11b-145">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3f11b-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a><span data-ttu-id="3f11b-146">Ответ об ошибке операции RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="3f11b-146">RemoveContactFromImList operation error response</span></span>

<span data-ttu-id="3f11b-147">В следующем примере показан ответ об ошибке для запроса операции **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="3f11b-147">The following example shows an error response to a **RemoveContactFromImList** operation request.</span></span> <span data-ttu-id="3f11b-148">Это ответ на запрос на удаление контакта из списка **контактов Lync** , когда контакт больше не существует в списке.</span><span class="sxs-lookup"><span data-stu-id="3f11b-148">This is a response to a request to remove a contact from the **Lync Contacts** list when the contact no longer exists in the list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="3f11b-149">В теле SOAP отклика об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3f11b-149">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="3f11b-150">ремовеконтактфромимлистреспонсе</span><span class="sxs-lookup"><span data-stu-id="3f11b-150">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="3f11b-151">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="3f11b-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3f11b-152">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3f11b-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3f11b-153">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="3f11b-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="3f11b-154">См. также</span><span class="sxs-lookup"><span data-stu-id="3f11b-154">See also</span></span>

- [<span data-ttu-id="3f11b-155">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="3f11b-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="3f11b-156">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="3f11b-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

