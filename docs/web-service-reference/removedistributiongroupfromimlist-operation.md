---
title: Операция RemoveDistributionGroupFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: Найдите сведения о веб-служб Exchange RemoveDistributionGroupFromImList операции.
ms.openlocfilehash: 9999f98a5698dd33c22e22fdf86bd00a2d053b52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835096"
---
# <a name="removedistributiongroupfromimlist-operation"></a><span data-ttu-id="29b98-103">Операция RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="29b98-103">RemoveDistributionGroupFromImList operation</span></span>

<span data-ttu-id="29b98-104">Найдите сведения о **RemoveDistributionGroupFromImList** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="29b98-104">Find information about the **RemoveDistributionGroupFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="29b98-105">Операция **RemoveDistributionGroupFromImList** удаляет группу рассылки в списке обмен мгновенными сообщениями (IM) Lync при Lync с помощью Exchange хранилища контактов.</span><span class="sxs-lookup"><span data-stu-id="29b98-105">The **RemoveDistributionGroupFromImList** operation removes a distribution group from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="29b98-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="29b98-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a><span data-ttu-id="29b98-107">С помощью операции RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="29b98-107">Using the RemoveDistributionGroupFromImList operation</span></span>

<span data-ttu-id="29b98-108">Операция **RemoveDistributionGroupFromImList** принимает один аргумент, определяющий группу рассылки, чтобы удалить из списка Lync обмена мгновенными Сообщениями, хранящиеся на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="29b98-108">The **RemoveDistributionGroupFromImList** operation accepts a single argument that identifies a distribution group to remove from the Lync IM list stored on an Exchange server.</span></span> 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a><span data-ttu-id="29b98-109">Заголовки SOAP RemoveDistributionGroupFromImList операции</span><span class="sxs-lookup"><span data-stu-id="29b98-109">RemoveDistributionGroupFromImList operation SOAP headers</span></span>

<span data-ttu-id="29b98-110">Операция **RemoveDistributionGroupFromImList** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="29b98-110">The **RemoveDistributionGroupFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="29b98-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="29b98-111">**Header name**</span></span>|<span data-ttu-id="29b98-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="29b98-112">**Element**</span></span>|<span data-ttu-id="29b98-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="29b98-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="29b98-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="29b98-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="29b98-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="29b98-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="29b98-116">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="29b98-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="29b98-117">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="29b98-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="29b98-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="29b98-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="29b98-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="29b98-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="29b98-120">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="29b98-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="29b98-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="29b98-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="29b98-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="29b98-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="29b98-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="29b98-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="29b98-124">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="29b98-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="29b98-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="29b98-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="29b98-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="29b98-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="29b98-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="29b98-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="29b98-128">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="29b98-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="29b98-129">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="29b98-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a><span data-ttu-id="29b98-130">Пример запроса RemoveDistributionGroupFromImList операции: удаление группы рассылки из списка обмена мгновенными Сообщениями</span><span class="sxs-lookup"><span data-stu-id="29b98-130">RemoveDistributionGroupFromImList operation request example: Remove a distribution group from an IM list</span></span>

<span data-ttu-id="29b98-131">В следующем примере запрос операции **RemoveDistributionGroupFromImList** показано, как удалить группу рассылки из группы обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="29b98-131">The following example of a **RemoveDistributionGroupFromImList** operation request shows how to remove a distribution group from an IM group.</span></span> <span data-ttu-id="29b98-132">Операция **RemoveDistributionGroupFromImList** принимает идентификатор уникальные группы для идентификации группы рассылки, чтобы удалить из списка обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="29b98-132">The **RemoveDistributionGroupFromImList** operation accepts the unique group identifier to identify the distribution group to remove from the IM list.</span></span> <span data-ttu-id="29b98-133">Элемент [ExchangeStoreId](exchangestoreid.md) , возвращаемого в ответе для [операции GetImItemList](getimitemlist-operation.md) и [AddDistributionGroupToImList операции](adddistributiongrouptoimlist-operation.md) определяет группы рассылки, которые могут быть удалены из списка обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="29b98-133">The [ExchangeStoreId](exchangestoreid.md) element that is returned in the response for the [GetImItemList operation](getimitemlist-operation.md) and the [AddDistributionGroupToImList operation](adddistributiongrouptoimlist-operation.md) identifies distribution groups that can be removed from the IM list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="29b98-134">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="29b98-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveDistributionGroupFromImList>
         <m:GroupId Id="AAMkADEzO4QrAABmEh5oAAA="/>
      </m:RemoveDistributionGroupFromImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="29b98-135">В приглашении на SOAP body используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="29b98-135">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="29b98-136">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="29b98-136">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist.md)
    
- [<span data-ttu-id="29b98-137">GroupId</span><span class="sxs-lookup"><span data-stu-id="29b98-137">GroupId</span></span>](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a><span data-ttu-id="29b98-138">Успешные операции ответа RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="29b98-138">Successful RemoveDistributionGroupFromImList operation response</span></span>

<span data-ttu-id="29b98-139">В следующем примере показано успешного ответа на запрос операции **RemoveDistributionGroupFromImList** удалить группу рассылки из группы обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="29b98-139">The following example shows a successful response to a **RemoveDistributionGroupFromImList** operation request to a remove a distribution group from an IM group.</span></span> 
  
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
      <RemoveDistributionGroupFromImListResponse ResponseClass="Success" 
                                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="29b98-140">В ответе SOAP body используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="29b98-140">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="29b98-141">RemoveDistributionGroupFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="29b98-141">RemoveDistributionGroupFromImListResponse</span></span>](removedistributiongroupfromimlistresponse.md)
    
- [<span data-ttu-id="29b98-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="29b98-142">ResponseCode</span></span>](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a><span data-ttu-id="29b98-143">Пример ответа об ошибке RemoveDistributionGroupFromImList операции</span><span class="sxs-lookup"><span data-stu-id="29b98-143">RemoveDistributionGroupFromImList operation error response example</span></span>

<span data-ttu-id="29b98-144">В следующем примере показано ошибочный ответ на запрос операции **RemoveDistributionGroupFromImList** .</span><span class="sxs-lookup"><span data-stu-id="29b98-144">The following example shows an error response to a **RemoveDistributionGroupFromImList** operation request.</span></span> <span data-ttu-id="29b98-145">Это ответ на запрос, чтобы удалить группу рассылки, которая уже была удалена из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="29b98-145">This is a response to a request to remove a distribution group that has already been removed from the mailbox.</span></span> 
  
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
      <RemoveDistributionGroupFromImListResponse ResponseClass="Error" 
                                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="29b98-146">В ответе ошибка SOAP body используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="29b98-146">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="29b98-147">RemoveDistributionGroupFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="29b98-147">RemoveDistributionGroupFromImListResponse</span></span>](removedistributiongroupfromimlistresponse.md)
    
- [<span data-ttu-id="29b98-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="29b98-148">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="29b98-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="29b98-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="29b98-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="29b98-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="29b98-151">См. также</span><span class="sxs-lookup"><span data-stu-id="29b98-151">See also</span></span>

- [<span data-ttu-id="29b98-152">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="29b98-152">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="29b98-153">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="29b98-153">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="29b98-154">Операция AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="29b98-154">AddDistributionGroupToImList operation</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="29b98-155">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="29b98-155">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

