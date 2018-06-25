---
title: Операция AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Найдите сведения о веб-служб Exchange AddDistributionGroupToImList операции.
ms.openlocfilehash: 7c562c317890a4cffb9e5844ea41c1096a8595b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761335"
---
# <a name="adddistributiongrouptoimlist-operation"></a><span data-ttu-id="d57bf-103">Операция AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="d57bf-103">AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="d57bf-104">Найдите сведения о **AddDistributionGroupToImList** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d57bf-104">Find information about the **AddDistributionGroupToImList** EWS operation.</span></span> 
  
<span data-ttu-id="d57bf-105">Операции веб-служб Exchange (EWS) **AddDistributionGroupToImList** добавляет группу рассылки для обмена мгновенными сообщениями (IM) списка в единого хранилища контактов.</span><span class="sxs-lookup"><span data-stu-id="d57bf-105">The **AddDistributionGroupToImList** Exchange Web Services (EWS) operation adds a distribution group to the instant messaging (IM) list in the Unified Contact Store.</span></span> 
  
<span data-ttu-id="d57bf-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d57bf-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a><span data-ttu-id="d57bf-107">С помощью операции AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="d57bf-107">Using the AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="d57bf-108">Операция **AddDistributionGroupToImList** принимает один аргумент, определяющий группу рассылки, чтобы добавить в список обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="d57bf-108">The **AddDistributionGroupToImList** operation takes a single argument that identifies a distribution group to add to the IM list.</span></span> <span data-ttu-id="d57bf-109">Эта операция не создает группу рассылки; группа рассылки уже должны быть созданы.</span><span class="sxs-lookup"><span data-stu-id="d57bf-109">This operation does not create a distribution group; the distribution group must already be created.</span></span> 
  
<span data-ttu-id="d57bf-110">Эту операцию можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="d57bf-110">This operation can use the SOAP headers that are listed in the following table.</span></span>
  
<span data-ttu-id="d57bf-111">**В таблице 1. Заголовки SOAP AddDistributionGroupToImList операции**</span><span class="sxs-lookup"><span data-stu-id="d57bf-111">**Table 1. AddDistributionGroupToImList operation SOAP headers**</span></span>

|<span data-ttu-id="d57bf-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="d57bf-112">**Header name**</span></span>|<span data-ttu-id="d57bf-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d57bf-113">**Element**</span></span>|<span data-ttu-id="d57bf-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d57bf-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d57bf-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="d57bf-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d57bf-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d57bf-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d57bf-117">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="d57bf-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="d57bf-118">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="d57bf-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d57bf-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="d57bf-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="d57bf-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="d57bf-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="d57bf-121">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="d57bf-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="d57bf-122">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="d57bf-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d57bf-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d57bf-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d57bf-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d57bf-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d57bf-125">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="d57bf-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d57bf-126">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="d57bf-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d57bf-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d57bf-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d57bf-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d57bf-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d57bf-129">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="d57bf-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d57bf-130">Это применимо для ответа.</span><span class="sxs-lookup"><span data-stu-id="d57bf-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a><span data-ttu-id="d57bf-131">Пример запроса AddDistributionGroupToImList операции</span><span class="sxs-lookup"><span data-stu-id="d57bf-131">AddDistributionGroupToImList operation request example</span></span>

<span data-ttu-id="d57bf-132">В следующем примере запрос операции **AddDistributionGroupToImList** показано, как добавить группу рассылки в список обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="d57bf-132">The following example of an **AddDistributionGroupToImList** operation request shows how to add a distribution group to the IM list.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d57bf-133">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d57bf-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d57bf-134">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="d57bf-134">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist.md)   
- [<span data-ttu-id="d57bf-135">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="d57bf-135">SmtpAddress</span></span>](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a><span data-ttu-id="d57bf-136">Успешные операции ответа AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="d57bf-136">Successful AddDistributionGroupToImList operation response</span></span>

<span data-ttu-id="d57bf-137">В следующем примере показано успешного ответа на запрос операции **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="d57bf-137">The following example shows a successful response to an **AddDistributionGroupToImList** operation request.</span></span> 
  
<span data-ttu-id="d57bf-138">Успешного ответа содержит отображаемое имя группы рассылки, класс хранилища Exchange для веб-служб Exchange идентификатор новой группы рассылки и группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="d57bf-138">The successful response contains the distribution group display name, the Exchange store class for the distribution group, and the EWS identifier of the new distribution group.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <s:Header>
      <t:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"/>
   </s:Header>
   <s:Body>
      <m:AddDistributionGroupToImListResponse ResponseClass="Success">
         <m:ResponseCode>NoError</m:ResponseCode>
         <m:ImGroup>
            <t:DisplayName>distributionlist1@example.com</t:DisplayName>
            <t:GroupType>IPM.DistList.MOC.DG</t:GroupType>
            <t:ExchangeStoreId Id="AAMkAGQ1MjJjAA=" 
                             ChangeKey="EgAAAA=="/>
      </m:ImGroup>
      </m:AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d57bf-139">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d57bf-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d57bf-140">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="d57bf-140">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="d57bf-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d57bf-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d57bf-142">ImGroup</span><span class="sxs-lookup"><span data-stu-id="d57bf-142">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="d57bf-143">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="d57bf-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="d57bf-144">GroupType</span><span class="sxs-lookup"><span data-stu-id="d57bf-144">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="d57bf-145">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="d57bf-145">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a><span data-ttu-id="d57bf-146">Операция AddDistributionGroupToImList ErrorInvalidImDistributionGroupSmtpAddress ошибка ответа</span><span class="sxs-lookup"><span data-stu-id="d57bf-146">AddDistributionGroupToImList operation ErrorInvalidImDistributionGroupSmtpAddress error response</span></span>

<span data-ttu-id="d57bf-147">В следующем примере показано ошибочный ответ на запрос операции **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="d57bf-147">The following example shows an error response to an **AddDistributionGroupToImList** operation request.</span></span> <span data-ttu-id="d57bf-148">Приведенный ниже ответ ошибка возникает при попытке добавить группу рассылки, которая не существует в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d57bf-148">The following error response occurs when an attempt is made to add a distribution group that does not exist in the Exchange store.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d57bf-149">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d57bf-149">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d57bf-150">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="d57bf-150">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="d57bf-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="d57bf-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d57bf-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d57bf-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="d57bf-153">См. также</span><span class="sxs-lookup"><span data-stu-id="d57bf-153">See also</span></span>

- [<span data-ttu-id="d57bf-154">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="d57bf-154">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [<span data-ttu-id="d57bf-155">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="d57bf-155">AddImGroup</span></span>](addimgroup-operation.md)   
- [<span data-ttu-id="d57bf-156">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="d57bf-156">RemoveImGroup</span></span>](removeimgroup-operation.md)
    

