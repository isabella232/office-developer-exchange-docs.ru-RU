---
title: Операция RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: Найдите сведения о веб-служб Exchange RemoveImContactFromGroup операции.
ms.openlocfilehash: 8c9af251014dbddabb439ed5bf5dc35580da6a90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835099"
---
# <a name="removeimcontactfromgroup-operation"></a><span data-ttu-id="c2a98-103">Операция RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-103">RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="c2a98-104">Найдите сведения о **RemoveImContactFromGroup** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2a98-104">Find information about the **RemoveImContactFromGroup** EWS operation.</span></span> 
  
<span data-ttu-id="c2a98-105">Операция **RemoveImContactFromGroup** удаляет с одним контактом обмена мгновенными Сообщениями из группы с обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="c2a98-105">The **RemoveImContactFromGroup** operation removes a single IM contact from an IM group.</span></span> 
  
<span data-ttu-id="c2a98-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c2a98-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimcontactfromgroup-operation"></a><span data-ttu-id="c2a98-107">С помощью операции RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-107">Using the RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="c2a98-108">Операция **RemoveImContactFromGroup** принимает два аргумента: идентификатор элемента контакта и соответствующих обмена мгновенными сообщениями, группа обмена Мгновенными сообщениями, из которого удаляется контакт.</span><span class="sxs-lookup"><span data-stu-id="c2a98-108">The **RemoveImContactFromGroup** operation takes two arguments: a contact item identifier, and the corresponding instant messaging (IM) group from which the contact is removed.</span></span> 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a><span data-ttu-id="c2a98-109">Заголовки SOAP RemoveImContactFromGroup операции</span><span class="sxs-lookup"><span data-stu-id="c2a98-109">RemoveImContactFromGroup operation SOAP headers</span></span>

<span data-ttu-id="c2a98-110">Операция **RemoveImContactFromGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c2a98-110">The **RemoveImContactFromGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c2a98-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="c2a98-111">**Header name**</span></span>|<span data-ttu-id="c2a98-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c2a98-112">**Element**</span></span>|<span data-ttu-id="c2a98-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c2a98-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c2a98-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="c2a98-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="c2a98-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c2a98-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c2a98-116">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="c2a98-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="c2a98-117">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="c2a98-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c2a98-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="c2a98-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="c2a98-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c2a98-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="c2a98-120">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="c2a98-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="c2a98-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="c2a98-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c2a98-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c2a98-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c2a98-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c2a98-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c2a98-124">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="c2a98-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="c2a98-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="c2a98-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c2a98-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c2a98-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c2a98-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c2a98-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c2a98-128">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="c2a98-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="c2a98-129">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="c2a98-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a><span data-ttu-id="c2a98-130">Пример запроса RemoveImContactFromGroup операции</span><span class="sxs-lookup"><span data-stu-id="c2a98-130">RemoveImContactFromGroup operation request example</span></span>

<span data-ttu-id="c2a98-131">В следующем примере запрос операции **RemoveImContactFromGroup** показано, как удалить для обмена мгновенными Сообщениями контакта из группы обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="c2a98-131">The following example of a **RemoveImContactFromGroup** operation request shows how to remove an IM contact from an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c2a98-132">Идентификаторы групп и контактов URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="c2a98-132">The group and contact identifiers have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImContactFromGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTcAAAAvcAAA="
                      ChangeKey="EQAAABYAAABtF8oI7iVOQ"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkbWAAAAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImContactFromGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c2a98-133">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c2a98-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c2a98-134">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-134">RemoveImContactFromGroup</span></span>](removeimcontactfromgroup.md)
    
- [<span data-ttu-id="c2a98-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="c2a98-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="c2a98-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="c2a98-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a><span data-ttu-id="c2a98-137">Успешные операции ответа RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-137">Successful RemoveImContactFromGroup operation response</span></span>

<span data-ttu-id="c2a98-138">В следующем примере показано успешного ответа на запрос операции **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="c2a98-138">The following example shows a successful response to a **RemoveImContactFromGroup** operation request.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Success" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="c2a98-139">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c2a98-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c2a98-140">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="c2a98-140">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="c2a98-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c2a98-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="c2a98-142">Операция RemoveImContactFromGroup ErrorInvalidImContactId ошибка ответа</span><span class="sxs-lookup"><span data-stu-id="c2a98-142">RemoveImContactFromGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="c2a98-143">В следующем примере показано ошибочный ответ на запрос операции **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="c2a98-143">The following example shows an error response to a **RemoveImContactFromGroup** operation request.</span></span> <span data-ttu-id="c2a98-144">Приведенный ниже ответ ошибка возникает при попытке удаления элемента контактов, не существует в группе мгновенные сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2a98-144">The following error response occurs when an attempt is made to remove a contact item that does not exist in the IM group.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Error" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="c2a98-145">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c2a98-145">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c2a98-146">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="c2a98-146">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="c2a98-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="c2a98-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c2a98-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c2a98-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c2a98-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c2a98-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="c2a98-150">См. также</span><span class="sxs-lookup"><span data-stu-id="c2a98-150">See also</span></span>

- [<span data-ttu-id="c2a98-151">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="c2a98-151">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="c2a98-152">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="c2a98-152">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="c2a98-153">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-153">AddImContactToGroup</span></span>](addimcontacttogroup-operation.md)
    
- [<span data-ttu-id="c2a98-154">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-154">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="c2a98-155">Операция AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-155">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="c2a98-156">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="c2a98-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="c2a98-157">GetImItems</span><span class="sxs-lookup"><span data-stu-id="c2a98-157">GetImItems</span></span>](getimitems-operation.md)
    
- [<span data-ttu-id="c2a98-158">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="c2a98-158">RemoveContactFromImList</span></span>](removecontactfromimlist-operation.md)
    
- [<span data-ttu-id="c2a98-159">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="c2a98-159">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist-operation.md)
    
- [<span data-ttu-id="c2a98-160">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-160">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="c2a98-161">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="c2a98-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="c2a98-162">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="c2a98-162">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted-operation.md)
    

