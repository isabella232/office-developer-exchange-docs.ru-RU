---
title: Операция RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: Поиск сведений о RemoveImContactFromGroupной операции EWS.
ms.openlocfilehash: 8c9af251014dbddabb439ed5bf5dc35580da6a90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835099"
---
# <a name="removeimcontactfromgroup-operation"></a><span data-ttu-id="d2cd3-103">Операция RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-103">RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="d2cd3-104">Поиск сведений о **RemoveImContactFromGroupной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-104">Find information about the **RemoveImContactFromGroup** EWS operation.</span></span> 
  
<span data-ttu-id="d2cd3-105">Операция **RemoveImContactFromGroup** удаляет один контакт для обмена мгновенными сообщениями из группы обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-105">The **RemoveImContactFromGroup** operation removes a single IM contact from an IM group.</span></span> 
  
<span data-ttu-id="d2cd3-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimcontactfromgroup-operation"></a><span data-ttu-id="d2cd3-107">Использование операции RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-107">Using the RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="d2cd3-108">Для операции **RemoveImContactFromGroup** используются два аргумента: идентификатор элемента контакта и соответствующая группа обмена мгновенными сообщениями, из которой удаляется контакт.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-108">The **RemoveImContactFromGroup** operation takes two arguments: a contact item identifier, and the corresponding instant messaging (IM) group from which the contact is removed.</span></span> 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a><span data-ttu-id="d2cd3-109">Заголовки SOAP операции RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-109">RemoveImContactFromGroup operation SOAP headers</span></span>

<span data-ttu-id="d2cd3-110">Операция **RemoveImContactFromGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-110">The **RemoveImContactFromGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d2cd3-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="d2cd3-111">**Header name**</span></span>|<span data-ttu-id="d2cd3-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d2cd3-112">**Element**</span></span>|<span data-ttu-id="d2cd3-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d2cd3-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d2cd3-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="d2cd3-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d2cd3-115">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="d2cd3-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d2cd3-116">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="d2cd3-117">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d2cd3-118">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="d2cd3-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="d2cd3-119">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="d2cd3-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="d2cd3-120">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="d2cd3-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d2cd3-122">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="d2cd3-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d2cd3-123">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="d2cd3-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d2cd3-124">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d2cd3-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d2cd3-126">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="d2cd3-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d2cd3-127">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="d2cd3-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d2cd3-128">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d2cd3-129">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a><span data-ttu-id="d2cd3-130">Пример запроса операции RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-130">RemoveImContactFromGroup operation request example</span></span>

<span data-ttu-id="d2cd3-131">В следующем примере запроса операции **RemoveImContactFromGroup** показано, как удалить контакт для обмена мгновенными сообщениями из группы обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-131">The following example of a **RemoveImContactFromGroup** operation request shows how to remove an IM contact from an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d2cd3-132">Идентификаторы групп и контактов были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-132">The group and contact identifiers have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="d2cd3-133">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d2cd3-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d2cd3-134">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-134">RemoveImContactFromGroup</span></span>](removeimcontactfromgroup.md)
    
- [<span data-ttu-id="d2cd3-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="d2cd3-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="d2cd3-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="d2cd3-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a><span data-ttu-id="d2cd3-137">Успешный отклик операции RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-137">Successful RemoveImContactFromGroup operation response</span></span>

<span data-ttu-id="d2cd3-138">В следующем примере показан успешный ответ на запрос операции **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="d2cd3-138">The following example shows a successful response to a **RemoveImContactFromGroup** operation request.</span></span> 
  
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

<span data-ttu-id="d2cd3-139">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d2cd3-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d2cd3-140">ремовеимконтактфромграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="d2cd3-140">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="d2cd3-141">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="d2cd3-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="d2cd3-142">Ответ об ошибке Ерроринвалидимконтактид операции RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-142">RemoveImContactFromGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="d2cd3-143">В следующем примере показан ответ об ошибке для запроса операции **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="d2cd3-143">The following example shows an error response to a **RemoveImContactFromGroup** operation request.</span></span> <span data-ttu-id="d2cd3-144">При попытке удалить элемент контакта, который не существует в группе IM, возникает следующий ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d2cd3-144">The following error response occurs when an attempt is made to remove a contact item that does not exist in the IM group.</span></span> 
  
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

<span data-ttu-id="d2cd3-145">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d2cd3-145">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d2cd3-146">ремовеимконтактфромграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="d2cd3-146">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="d2cd3-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="d2cd3-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d2cd3-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="d2cd3-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d2cd3-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="d2cd3-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="d2cd3-150">См. также</span><span class="sxs-lookup"><span data-stu-id="d2cd3-150">See also</span></span>

- [<span data-ttu-id="d2cd3-151">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="d2cd3-151">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="d2cd3-152">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="d2cd3-152">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="d2cd3-153">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-153">AddImContactToGroup</span></span>](addimcontacttogroup-operation.md)
    
- [<span data-ttu-id="d2cd3-154">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-154">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="d2cd3-155">Операция AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-155">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="d2cd3-156">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="d2cd3-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="d2cd3-157">GetImItems</span><span class="sxs-lookup"><span data-stu-id="d2cd3-157">GetImItems</span></span>](getimitems-operation.md)
    
- [<span data-ttu-id="d2cd3-158">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="d2cd3-158">RemoveContactFromImList</span></span>](removecontactfromimlist-operation.md)
    
- [<span data-ttu-id="d2cd3-159">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="d2cd3-159">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist-operation.md)
    
- [<span data-ttu-id="d2cd3-160">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-160">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="d2cd3-161">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="d2cd3-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="d2cd3-162">сетимлистмигратионкомплетед</span><span class="sxs-lookup"><span data-stu-id="d2cd3-162">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted-operation.md)
    

