---
title: Операция SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2d48aa07-8152-4c3d-a519-061253e80174
description: Найдите сведения о веб-служб Exchange SetImGroup операции.
ms.openlocfilehash: 80980c25888ab3fcae0a761e115c3ac3d578a013
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835421"
---
# <a name="setimgroup-operation"></a><span data-ttu-id="3f268-103">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3f268-103">SetImGroup operation</span></span>

<span data-ttu-id="3f268-104">Найдите сведения о **SetImGroup** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f268-104">Find information about the **SetImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="3f268-105">Операция **SetImGroup** изменяется отображаемое имя обмена мгновенными сообщениями (IM) группы.</span><span class="sxs-lookup"><span data-stu-id="3f268-105">The **SetImGroup** operation changes the display name of an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="3f268-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3f268-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setimgroup-operation"></a><span data-ttu-id="3f268-107">С помощью операции SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3f268-107">Using the SetImGroup operation</span></span>

<span data-ttu-id="3f268-108">Операция **SetImGroup** только принимает аргумент одного отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3f268-108">The **SetImGroup** operation only takes a single display name argument.</span></span> 
  
### <a name="setimgroup-operation-soap-headers"></a><span data-ttu-id="3f268-109">Заголовки SOAP SetImGroup операции</span><span class="sxs-lookup"><span data-stu-id="3f268-109">SetImGroup operation SOAP headers</span></span>

<span data-ttu-id="3f268-110">Операция **SetImGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="3f268-110">The **SetImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="3f268-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="3f268-111">**Header name**</span></span>|<span data-ttu-id="3f268-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f268-112">**Element**</span></span>|<span data-ttu-id="3f268-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f268-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3f268-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="3f268-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="3f268-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="3f268-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3f268-116">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="3f268-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="3f268-117">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="3f268-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3f268-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="3f268-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="3f268-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="3f268-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="3f268-120">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="3f268-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="3f268-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="3f268-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3f268-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="3f268-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3f268-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="3f268-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3f268-124">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="3f268-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="3f268-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="3f268-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3f268-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="3f268-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3f268-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3f268-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3f268-128">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="3f268-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="3f268-129">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="3f268-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setimgroup-operation-request-example"></a><span data-ttu-id="3f268-130">Пример запроса SetImGroup операции</span><span class="sxs-lookup"><span data-stu-id="3f268-130">SetImGroup operation request example</span></span>

<span data-ttu-id="3f268-131">В следующем примере запрос операции **SetImGroup** показано, как изменить отображаемое имя группы, при обмена мгновенными Сообщениями «MyNewGroupName».</span><span class="sxs-lookup"><span data-stu-id="3f268-131">The following example of a **SetImGroup** operation request shows how to change an IM group display name to "MyNewGroupName".</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3f268-132">Идентификатор хранилища Exchange был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="3f268-132">The Exchange store identifier has been shortened to preserve readability.</span></span> 
  
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
      <m:SetImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
         <m:NewDisplayName>MyNewGroupName</m:NewDisplayName>
      </m:SetImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3f268-133">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3f268-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3f268-134">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3f268-134">SetImGroup</span></span>](setimgroup.md)
    
- [<span data-ttu-id="3f268-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="3f268-135">GroupId</span></span>](groupid.md)
    
- [<span data-ttu-id="3f268-136">NewDisplayName</span><span class="sxs-lookup"><span data-stu-id="3f268-136">NewDisplayName</span></span>](newdisplayname.md)
    
## <a name="successful-setimgroup-operation-response"></a><span data-ttu-id="3f268-137">Успешные операции ответа SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3f268-137">Successful SetImGroup operation response</span></span>

<span data-ttu-id="3f268-138">В следующем примере показано успешного ответа на запрос операции **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="3f268-138">The following example shows a successful response to a **SetImGroup** operation request.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         </SetImGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="3f268-139">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3f268-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3f268-140">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3f268-140">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="3f268-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3f268-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="setimgroup-operation-error-response"></a><span data-ttu-id="3f268-142">Ошибка операции SetImGroup ответа</span><span class="sxs-lookup"><span data-stu-id="3f268-142">SetImGroup operation error response</span></span>

<span data-ttu-id="3f268-143">В следующем примере показано ошибочный ответ на запрос операции **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="3f268-143">The following example shows an error response to a **SetImGroup** operation request.</span></span> <span data-ttu-id="3f268-144">Приведенный ниже ответ ошибка возникает при попытке изменить отображаемое имя группы отображаемое имя существующей группы.</span><span class="sxs-lookup"><span data-stu-id="3f268-144">The following error response occurs when an attempt is made to change the group display name to the existing group display name.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>An IM group with the specified display name already exists.</MessageText>
         <ResponseCode>ErrorImGroupDisplayNameAlreadyExists</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3f268-145">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3f268-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3f268-146">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3f268-146">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="3f268-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="3f268-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3f268-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3f268-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3f268-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3f268-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="3f268-150">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="3f268-150">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="3f268-151">См. также</span><span class="sxs-lookup"><span data-stu-id="3f268-151">See also</span></span>

- [<span data-ttu-id="3f268-152">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="3f268-152">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="3f268-153">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="3f268-153">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="3f268-154">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="3f268-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    

