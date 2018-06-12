---
title: Операция RemoveImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e788016-68e0-4a3f-9243-03f6b6c6b389
description: Найдите сведения о веб-служб Exchange RemoveImGroup операции.
ms.openlocfilehash: 85b312f0b156125a2d5395658ccea06d831abdde
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835097"
---
# <a name="removeimgroup-operation"></a><span data-ttu-id="3dee6-103">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="3dee6-103">RemoveImGroup operation</span></span>

<span data-ttu-id="3dee6-104">Найдите сведения о **RemoveImGroup** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="3dee6-104">Find information about the **RemoveImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="3dee6-105">Операция **RemoveImGroup** удаляет одну мгновенного обмена сообщениями группу обмена Мгновенными сообщениями из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3dee6-105">The **RemoveImGroup** operation removes a single instant messaging (IM) group from a mailbox.</span></span> 
  
<span data-ttu-id="3dee6-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3dee6-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimgroup-operation"></a><span data-ttu-id="3dee6-107">С помощью операции RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="3dee6-107">Using the RemoveImGroup operation</span></span>

<span data-ttu-id="3dee6-108">Операция **RemoveImGroup** принимает только аргумент идентификатор единая группа.</span><span class="sxs-lookup"><span data-stu-id="3dee6-108">The **RemoveImGroup** operation only takes a single group identifier argument.</span></span> 
  
### <a name="removeimgroup-operation-soap-headers"></a><span data-ttu-id="3dee6-109">Заголовки SOAP RemoveImGroup операции</span><span class="sxs-lookup"><span data-stu-id="3dee6-109">RemoveImGroup operation SOAP headers</span></span>

<span data-ttu-id="3dee6-110">Операция **RemoveImGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="3dee6-110">The **RemoveImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="3dee6-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="3dee6-111">**Header name**</span></span>|<span data-ttu-id="3dee6-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3dee6-112">**Element**</span></span>|<span data-ttu-id="3dee6-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3dee6-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3dee6-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="3dee6-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="3dee6-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="3dee6-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3dee6-116">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="3dee6-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="3dee6-117">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="3dee6-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3dee6-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="3dee6-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="3dee6-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="3dee6-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="3dee6-120">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="3dee6-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="3dee6-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="3dee6-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3dee6-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="3dee6-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3dee6-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="3dee6-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3dee6-124">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="3dee6-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="3dee6-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="3dee6-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3dee6-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="3dee6-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3dee6-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3dee6-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3dee6-128">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="3dee6-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="3dee6-129">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="3dee6-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimgroup-operation-request-example"></a><span data-ttu-id="3dee6-130">Пример запроса RemoveImGroup операции</span><span class="sxs-lookup"><span data-stu-id="3dee6-130">RemoveImGroup operation request example</span></span>

<span data-ttu-id="3dee6-131">В следующем примере запрос операции **RemoveImGroup** показано, как удалить группу обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="3dee6-131">The following example of a **RemoveImGroup** operation request shows how to remove an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3dee6-132">Идентификатор группы был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="3dee6-132">The group ID has been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5hQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3dee6-133">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3dee6-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3dee6-134">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="3dee6-134">RemoveImGroup</span></span>](removeimgroup.md)
    
- [<span data-ttu-id="3dee6-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="3dee6-135">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimgroup-operation-response"></a><span data-ttu-id="3dee6-136">Успешные операции ответа RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="3dee6-136">Successful RemoveImGroup operation response</span></span>

<span data-ttu-id="3dee6-137">В следующем примере показано успешного ответа на запрос операции **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="3dee6-137">The following example shows a successful response to a **RemoveImGroup** operation request.</span></span> 
  
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
      <RemoveImGroupResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3dee6-138">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3dee6-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3dee6-139">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3dee6-139">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="3dee6-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3dee6-140">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimgroup-operation-errorinvalidimgroupid-error-response"></a><span data-ttu-id="3dee6-141">Операция RemoveImGroup ErrorInvalidImGroupId ошибка ответа</span><span class="sxs-lookup"><span data-stu-id="3dee6-141">RemoveImGroup operation ErrorInvalidImGroupId error response</span></span>

<span data-ttu-id="3dee6-142">В следующем примере показано ошибочный ответ на запрос операции **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="3dee6-142">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="3dee6-143">Приведенный ниже ответ ошибка возникает при попытке удалить группу, которая не существует в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3dee6-143">The following error response occurs when an attempt is made to remove a group that does not exist in the mailbox.</span></span> 
  
```XML
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
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Group Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImGroupId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3dee6-144">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3dee6-144">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3dee6-145">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3dee6-145">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="3dee6-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="3dee6-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3dee6-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3dee6-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3dee6-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3dee6-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="3dee6-149">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="3dee6-149">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="removeimgroup-operation-errorinvalididmalformed-error-response"></a><span data-ttu-id="3dee6-150">Операция RemoveImGroup ErrorInvalidIdMalformed ошибка ответа</span><span class="sxs-lookup"><span data-stu-id="3dee6-150">RemoveImGroup operation ErrorInvalidIdMalformed error response</span></span>

<span data-ttu-id="3dee6-151">В следующем примере показано ошибочный ответ на запрос операции **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="3dee6-151">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="3dee6-152">Приведенный ниже ответ ошибка возникает при попытке удалить группу с идентификатором неправильно форматированные группы.</span><span class="sxs-lookup"><span data-stu-id="3dee6-152">The following error response occurs when an attempt is made to remove a group with an incorrectly formatted group identifier.</span></span> 
  
```XML
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
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3dee6-153">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3dee6-153">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3dee6-154">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3dee6-154">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="3dee6-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="3dee6-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3dee6-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3dee6-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3dee6-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3dee6-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="3dee6-158">См. также</span><span class="sxs-lookup"><span data-stu-id="3dee6-158">See also</span></span>

- [<span data-ttu-id="3dee6-159">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="3dee6-159">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="3dee6-160">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="3dee6-160">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="3dee6-161">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3dee6-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    

