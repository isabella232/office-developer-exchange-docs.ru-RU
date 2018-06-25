---
title: Операция AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Найдите сведения о веб-служб Exchange AddImGroup операции.
ms.openlocfilehash: 91236f9ad2236b3f6bee600b9d57bcf736090ed7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761341"
---
# <a name="addimgroup-operation"></a><span data-ttu-id="1ffb3-103">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="1ffb3-103">AddImGroup operation</span></span>

<span data-ttu-id="1ffb3-104">Найдите сведения о **AddImGroup** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-104">Find information about the **AddImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="1ffb3-105">Операции веб-служб Exchange (EWS) **AddImGroup** добавляет нового мгновенного обмена мгновенными сообщениями группу в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-105">The **AddImGroup** Exchange Web Services (EWS) operation adds a new instant messaging (IM) group to a mailbox.</span></span> 
  
<span data-ttu-id="1ffb3-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimgroup-operation"></a><span data-ttu-id="1ffb3-107">С помощью операции AddImGroup</span><span class="sxs-lookup"><span data-stu-id="1ffb3-107">Using the AddImGroup operation</span></span>

<span data-ttu-id="1ffb3-108">Операция **AddImGroup** только принимает аргумент одного отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-108">The **AddImGroup** operation only takes a single display name argument.</span></span> 
  
<span data-ttu-id="1ffb3-109">Эта операция возвращает отображаемое имя, тип группы и идентификатор хранилища Exchange новой группы.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-109">This operation returns the display name, group type, and Exchange store identifier of the new group.</span></span>
  
<span data-ttu-id="1ffb3-110">Операция **AddImGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-110">The **AddImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="1ffb3-111">**В таблице 1. Заголовки SOAP AddImGroup операции**</span><span class="sxs-lookup"><span data-stu-id="1ffb3-111">**Table 1. AddImGroup operation SOAP headers**</span></span>

|<span data-ttu-id="1ffb3-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="1ffb3-112">**Header name**</span></span>|<span data-ttu-id="1ffb3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1ffb3-113">**Element**</span></span>|<span data-ttu-id="1ffb3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1ffb3-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1ffb3-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="1ffb3-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="1ffb3-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1ffb3-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1ffb3-117">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="1ffb3-118">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1ffb3-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="1ffb3-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="1ffb3-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="1ffb3-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="1ffb3-121">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="1ffb3-122">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1ffb3-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1ffb3-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1ffb3-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1ffb3-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1ffb3-125">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1ffb3-126">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1ffb3-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1ffb3-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1ffb3-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1ffb3-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1ffb3-129">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1ffb3-130">Это применимо для ответа.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a><span data-ttu-id="1ffb3-131">Пример запроса AddImGroup операции: Создание новой группы обмена мгновенными Сообщениями</span><span class="sxs-lookup"><span data-stu-id="1ffb3-131">AddImGroup operation request example: Create a new IM group</span></span>

<span data-ttu-id="1ffb3-132">Приведенный ниже запрос операции **AddImGroup** показано, как создать группу обмена мгновенными Сообщениями с именем MyCustomerGroup.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-132">The following example of an **AddImGroup** operation request shows how to create an IM group named MyCustomerGroup.</span></span> 
  
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
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1ffb3-133">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1ffb3-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1ffb3-134">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="1ffb3-134">AddImGroup</span></span>](addimgroup.md)
    
- [<span data-ttu-id="1ffb3-135">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="1ffb3-135">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a><span data-ttu-id="1ffb3-136">Успешные операции ответа AddImGroup</span><span class="sxs-lookup"><span data-stu-id="1ffb3-136">Successful AddImGroup operation response</span></span>

<span data-ttu-id="1ffb3-137">В следующем примере показано успешного ответа на запрос операции **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="1ffb3-137">The following example shows a successful response to an **AddImGroup** operation request.</span></span> 
  
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
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="1ffb3-138">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1ffb3-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1ffb3-139">AddImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="1ffb3-139">AddImGroupResponse</span></span>](addimgroupresponse.md)
    
- [<span data-ttu-id="1ffb3-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1ffb3-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1ffb3-141">ImGroup</span><span class="sxs-lookup"><span data-stu-id="1ffb3-141">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="1ffb3-142">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="1ffb3-142">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="1ffb3-143">GroupType</span><span class="sxs-lookup"><span data-stu-id="1ffb3-143">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="1ffb3-144">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="1ffb3-144">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a><span data-ttu-id="1ffb3-145">Ошибка операции AddImGroup ответа</span><span class="sxs-lookup"><span data-stu-id="1ffb3-145">AddImGroup operation error response</span></span>

<span data-ttu-id="1ffb3-146">В следующем примере показано ошибочный ответ на запрос операции **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="1ffb3-146">The following example shows an error response to an **AddImGroup** operation request.</span></span> <span data-ttu-id="1ffb3-147">Это ответ на запрос, который содержит символ, который не может использоваться в поле отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-147">This is a response to a request that contains a character that cannot be used in a display name.</span></span> <span data-ttu-id="1ffb3-148">Обратите внимание на то, что это ошибка SOAP и не сообщение об ошибке на основе схемы.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-148">Note that this is a SOAP fault and not a schema-based error message.</span></span> <span data-ttu-id="1ffb3-149">Отображаемое имя, отправленными в запросе — ~! @# $% ^&amp;, и возникает ошибка на &amp; символов.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-149">The display name submitted in the request is ~!@#$%^&amp;, and the error occurs on the &amp; character.</span></span> <span data-ttu-id="1ffb3-150">&amp; Символ произошло 11 знаков в строке и 33rd в полезных данных запроса.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-150">The &amp; character occurred on the 11th line and 33rd character in the request payload.</span></span> <span data-ttu-id="1ffb3-151">Ответ с кодом HTTP 500.</span><span class="sxs-lookup"><span data-stu-id="1ffb3-151">The response was returned with an HTTP 500 code.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="1ffb3-152">См. также</span><span class="sxs-lookup"><span data-stu-id="1ffb3-152">See also</span></span>

- [<span data-ttu-id="1ffb3-153">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="1ffb3-153">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="1ffb3-154">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="1ffb3-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="1ffb3-155">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="1ffb3-155">SetImGroup</span></span>](setimgroup.md)
    

