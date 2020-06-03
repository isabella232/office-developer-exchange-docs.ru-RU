---
title: Операция RemoveImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e788016-68e0-4a3f-9243-03f6b6c6b389
description: Поиск сведений о RemoveImGroupной операции EWS.
ms.openlocfilehash: b5e38404cbb1907a1118ab3ae8e56abb5a8d5e41
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456762"
---
# <a name="removeimgroup-operation"></a><span data-ttu-id="4348a-103">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-103">RemoveImGroup operation</span></span>

<span data-ttu-id="4348a-104">Поиск сведений о **RemoveImGroupной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="4348a-104">Find information about the **RemoveImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="4348a-105">Операция **RemoveImGroup** удаляет из почтового ящика одну группу обмена мгновенными сообщениями (IM).</span><span class="sxs-lookup"><span data-stu-id="4348a-105">The **RemoveImGroup** operation removes a single instant messaging (IM) group from a mailbox.</span></span> 
  
<span data-ttu-id="4348a-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4348a-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimgroup-operation"></a><span data-ttu-id="4348a-107">Использование операции RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-107">Using the RemoveImGroup operation</span></span>

<span data-ttu-id="4348a-108">Операция **RemoveImGroup** принимает только один аргумент идентификатора группы.</span><span class="sxs-lookup"><span data-stu-id="4348a-108">The **RemoveImGroup** operation only takes a single group identifier argument.</span></span> 
  
### <a name="removeimgroup-operation-soap-headers"></a><span data-ttu-id="4348a-109">Заголовки SOAP операции RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-109">RemoveImGroup operation SOAP headers</span></span>

<span data-ttu-id="4348a-110">Операция **RemoveImGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="4348a-110">The **RemoveImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="4348a-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="4348a-111">**Header name**</span></span>|<span data-ttu-id="4348a-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4348a-112">**Element**</span></span>|<span data-ttu-id="4348a-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4348a-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4348a-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="4348a-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="4348a-115">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="4348a-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="4348a-116">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="4348a-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="4348a-117">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="4348a-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4348a-118">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="4348a-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="4348a-119">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="4348a-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="4348a-120">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="4348a-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="4348a-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="4348a-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4348a-122">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="4348a-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="4348a-123">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="4348a-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="4348a-124">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="4348a-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="4348a-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="4348a-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4348a-126">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="4348a-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="4348a-127">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="4348a-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="4348a-128">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="4348a-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="4348a-129">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="4348a-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimgroup-operation-request-example"></a><span data-ttu-id="4348a-130">Пример запроса операции RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-130">RemoveImGroup operation request example</span></span>

<span data-ttu-id="4348a-131">В следующем примере запроса операции **RemoveImGroup** показано, как удалить группу IM.</span><span class="sxs-lookup"><span data-stu-id="4348a-131">The following example of a **RemoveImGroup** operation request shows how to remove an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4348a-132">Идентификатор группы был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="4348a-132">The group ID has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="4348a-133">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4348a-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4348a-134">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-134">RemoveImGroup</span></span>](removeimgroup.md)
    
- [<span data-ttu-id="4348a-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="4348a-135">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimgroup-operation-response"></a><span data-ttu-id="4348a-136">Успешный отклик операции RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-136">Successful RemoveImGroup operation response</span></span>

<span data-ttu-id="4348a-137">В следующем примере показан успешный ответ на запрос операции **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="4348a-137">The following example shows a successful response to a **RemoveImGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Success" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="4348a-138">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4348a-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4348a-139">ремовеимграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="4348a-139">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="4348a-140">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4348a-140">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimgroup-operation-errorinvalidimgroupid-error-response"></a><span data-ttu-id="4348a-141">Ответ об ошибке Ерроринвалидимграупид операции RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-141">RemoveImGroup operation ErrorInvalidImGroupId error response</span></span>

<span data-ttu-id="4348a-142">В следующем примере показан ответ об ошибке для запроса операции **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="4348a-142">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="4348a-143">При попытке удалить группу, которая не существует в почтовом ящике, возникает следующий ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4348a-143">The following error response occurs when an attempt is made to remove a group that does not exist in the mailbox.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Group Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImGroupId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="4348a-144">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4348a-144">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4348a-145">ремовеимграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="4348a-145">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="4348a-146">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="4348a-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="4348a-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4348a-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4348a-148">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="4348a-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="4348a-149">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="4348a-149">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="removeimgroup-operation-errorinvalididmalformed-error-response"></a><span data-ttu-id="4348a-150">Ответ об ошибке Ерроринвалидидмалформед операции RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-150">RemoveImGroup operation ErrorInvalidIdMalformed error response</span></span>

<span data-ttu-id="4348a-151">В следующем примере показан ответ об ошибке для запроса операции **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="4348a-151">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="4348a-152">Следующий ответ об ошибке возникает при попытке удалить группу с неправильно отформатированным идентификатором группы.</span><span class="sxs-lookup"><span data-stu-id="4348a-152">The following error response occurs when an attempt is made to remove a group with an incorrectly formatted group identifier.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="4348a-153">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4348a-153">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4348a-154">ремовеимграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="4348a-154">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="4348a-155">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="4348a-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="4348a-156">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4348a-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4348a-157">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="4348a-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="4348a-158">См. также</span><span class="sxs-lookup"><span data-stu-id="4348a-158">See also</span></span>

- [<span data-ttu-id="4348a-159">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="4348a-159">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="4348a-160">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-160">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="4348a-161">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="4348a-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    

