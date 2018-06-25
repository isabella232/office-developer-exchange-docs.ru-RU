---
title: Операция AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Найдите сведения о веб-служб Exchange AddImContactToGroup операции.
ms.openlocfilehash: 669d798b6cabc1cab1fc057a3e18c565467440f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761336"
---
# <a name="addimcontacttogroup-operation"></a><span data-ttu-id="fde8f-103">Операция AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="fde8f-103">AddImContactToGroup operation</span></span>

<span data-ttu-id="fde8f-104">Найдите сведения о **AddImContactToGroup** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="fde8f-104">Find information about the **AddImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="fde8f-105">Операции веб-служб Exchange (EWS) **AddImContactToGroup** Добавляет существующий контакт, обмен мгновенными сообщениями (IM) в группу.</span><span class="sxs-lookup"><span data-stu-id="fde8f-105">The **AddImContactToGroup** Exchange Web Services (EWS) operation adds an existing instant messaging (IM) contact to a group.</span></span> 
  
<span data-ttu-id="fde8f-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fde8f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimcontacttogroup-operation"></a><span data-ttu-id="fde8f-107">С помощью операции AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="fde8f-107">Using the AddImContactToGroup operation</span></span>

<span data-ttu-id="fde8f-108">Операция **AddImContactToGroup** может принимать только служб обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="fde8f-108">The **AddImContactToGroup** operation can only accept IM contacts.</span></span> <span data-ttu-id="fde8f-109">Если вы хотите добавить новый контакт обмена мгновенными Сообщениями единого хранилища контактов, с помощью операции [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fde8f-109">If you want to add a new IM contact to the Unified Contact Store, use the [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) operation.</span></span> 
  
<span data-ttu-id="fde8f-110">Операция **AddImContactToGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="fde8f-110">The **AddImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="fde8f-111">**В таблице 1. Заголовки SOAP AddImContactToGroup операции**</span><span class="sxs-lookup"><span data-stu-id="fde8f-111">**Table 1. AddImContactToGroup operation SOAP headers**</span></span>

|<span data-ttu-id="fde8f-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="fde8f-112">**Header name**</span></span>|<span data-ttu-id="fde8f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fde8f-113">**Element**</span></span>|<span data-ttu-id="fde8f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fde8f-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fde8f-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="fde8f-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="fde8f-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="fde8f-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="fde8f-117">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="fde8f-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="fde8f-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="fde8f-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fde8f-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="fde8f-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="fde8f-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="fde8f-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="fde8f-121">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="fde8f-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="fde8f-122">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="fde8f-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fde8f-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="fde8f-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="fde8f-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="fde8f-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="fde8f-125">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="fde8f-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="fde8f-126">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="fde8f-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fde8f-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="fde8f-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="fde8f-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="fde8f-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="fde8f-129">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="fde8f-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="fde8f-130">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="fde8f-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a><span data-ttu-id="fde8f-131">Пример запроса AddImContactToGroup операции: Добавление существующего обмена мгновенными Сообщениями обратитесь к группе обмена мгновенными Сообщениями</span><span class="sxs-lookup"><span data-stu-id="fde8f-131">AddImContactToGroup operation request example: Add an existing IM contact to an IM group</span></span>

<span data-ttu-id="fde8f-132">Приведенный ниже запрос операции **AddImContactToGroup** показано, как добавить существующий контакт обмена мгновенными Сообщениями с группой обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="fde8f-132">The following example of an **AddImContactToGroup** operation request shows how to add an existing IM contact an IM group.</span></span> 
  
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
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="fde8f-133">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fde8f-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fde8f-134">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="fde8f-134">AddImContactToGroup</span></span>](addimcontacttogroup.md)
    
- [<span data-ttu-id="fde8f-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="fde8f-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="fde8f-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="fde8f-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a><span data-ttu-id="fde8f-137">Успешные операции ответа AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="fde8f-137">Successful AddImContactToGroup operation response</span></span>

<span data-ttu-id="fde8f-138">В следующем примере показано успешного ответа на запрос операции **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="fde8f-138">The following example shows a successful response to an **AddImContactToGroup** operation request.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="fde8f-139">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fde8f-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fde8f-140">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="fde8f-140">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="fde8f-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fde8f-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="fde8f-142">Операция AddImContactToGroup ErrorInvalidImContactId ошибка ответа</span><span class="sxs-lookup"><span data-stu-id="fde8f-142">AddImContactToGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="fde8f-143">В следующем примере показано ошибочный ответ на запрос операции **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="fde8f-143">The following example shows an error response to an **AddImContactToGroup** operation request.</span></span> <span data-ttu-id="fde8f-144">Приведенный ниже ответ ошибка возникает при попытке добавить контакт, который не является для обмена мгновенными Сообщениями контакта.</span><span class="sxs-lookup"><span data-stu-id="fde8f-144">The following error response occurs when an attempt is made to add a contact that is not an IM contact.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="fde8f-145">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fde8f-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fde8f-146">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="fde8f-146">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="fde8f-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="fde8f-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="fde8f-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fde8f-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fde8f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fde8f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="fde8f-150">См. также</span><span class="sxs-lookup"><span data-stu-id="fde8f-150">See also</span></span>

- [<span data-ttu-id="fde8f-151">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="fde8f-151">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="fde8f-152">Операция AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="fde8f-152">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="fde8f-153">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="fde8f-153">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="fde8f-154">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="fde8f-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="fde8f-155">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="fde8f-155">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="fde8f-156">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="fde8f-156">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

