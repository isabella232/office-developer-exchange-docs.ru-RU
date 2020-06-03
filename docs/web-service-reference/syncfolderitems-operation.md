---
title: Операция SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 7f0de089-8876-47ec-a871-df118ceae75d
description: Операция SyncFolderItems синхронизирует элементы между сервером Exchange Server и клиентом.
ms.openlocfilehash: 1a28d895eda11dd43f77ec2662a60a426cfc463c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468147"
---
# <a name="syncfolderitems-operation"></a><span data-ttu-id="0fd2b-103">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0fd2b-103">SyncFolderItems operation</span></span>

<span data-ttu-id="0fd2b-104">Операция SyncFolderItems синхронизирует элементы между сервером Exchange Server и клиентом.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-104">The SyncFolderItems operation synchronizes items between the Exchange server and the client.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0fd2b-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="0fd2b-105">Remarks</span></span>

<span data-ttu-id="0fd2b-106">Для операции SyncFolderItems будет возвращено не более 512 изменений.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-106">The SyncFolderItems operation will return a maximum of 512 changes.</span></span> <span data-ttu-id="0fd2b-107">Для получения дополнительных изменений необходимо выполнить последующие запросы SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-107">Subsequent SyncFolderItems requests must be performed to get additional changes.</span></span> 
  
<span data-ttu-id="0fd2b-108">SyncFolderItems аналогичен операции FindItem, так как она не может возвращать такие свойства, как текст или вложения.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-108">SyncFolderItems is similar to the FindItem operation in that it cannot return properties like Body or Attachments.</span></span> <span data-ttu-id="0fd2b-109">Если операция SyncFolderItems не возвращает нужные свойства, можно использовать [операцию GetItem](getitem-operation.md) для получения определенного набора свойств для каждого элемента, возвращенного SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-109">If the SyncFolderItems operation does not return the properties that you need, you can use the [GetItem operation](getitem-operation.md) to get a specific set of properties for each item that it returned by SyncFolderItems.</span></span> 
  
## <a name="syncfolderitems-request-example"></a><span data-ttu-id="0fd2b-110">Пример запроса SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0fd2b-110">SyncFolderItems request example</span></span>

### <a name="description"></a><span data-ttu-id="0fd2b-111">Description</span><span class="sxs-lookup"><span data-stu-id="0fd2b-111">Description</span></span>

<span data-ttu-id="0fd2b-112">В приведенном ниже примере запроса SyncFolderItems показано, как синхронизировать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-112">The following example of a SyncFolderItems request shows how to synchronize items in a folder.</span></span> <span data-ttu-id="0fd2b-113">В этом примере показана синхронизация элемента папки, которая не является первой синхронизацией, которая возникла для папки "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="0fd2b-113">This example shows a folder item's synchronization that is not the first synchronization to have occurred for the Sent Items folder.</span></span> <span data-ttu-id="0fd2b-114">Элемент [синкстате](syncstate-ex15websvcsotherref.md) не включается в запрос первой попытки синхронизации клиента с сервером Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-114">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="0fd2b-115">При первой попытке синхронизации элементов в иерархии папок будут возвращены все элементы почтового ящика, кроме элементов, указанных в элементе [Ignore](ignore.md) .</span><span class="sxs-lookup"><span data-stu-id="0fd2b-115">The first attempt to synchronize the items in a folder hierarchy will return all the items in the mailbox, excluding items that are identified in the [Ignore](ignore.md) element.</span></span> <span data-ttu-id="0fd2b-116">Этот запрос SyncFolderItems попытается выполнить синхронизацию всех изменений элементов папки с момента последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-116">This SyncFolderItems request will try to synchronize all changes to the folder items since the last synchronization.</span></span> <span data-ttu-id="0fd2b-117">Этот запрос будет игнорировать попытку синхронизации одного элемента, указанного в элементе [Ignore](ignore.md) .</span><span class="sxs-lookup"><span data-stu-id="0fd2b-117">This request will ignore the attempt to synchronize the one item that is identified in the [Ignore](ignore.md) element.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0fd2b-118">Код</span><span class="sxs-lookup"><span data-stu-id="0fd2b-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
      </ItemShape>
      <SyncFolderId>
        <t:DistinguishedFolderId Id="sentitems"/>
      </SyncFolderId>
      <SyncState>AEbJ94eMOAAA=</SyncState>
      <Ignore>
        <t:ItemId Id="AQApAHRAA==" ChangeKey="CQAAABY"/>
      </Ignore>
      <MaxChangesReturned>100</MaxChangesReturned>
    </SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="0fd2b-119">Комментарии</span><span class="sxs-lookup"><span data-stu-id="0fd2b-119">Comments</span></span>

<span data-ttu-id="0fd2b-120">Данные элемента [синкстате](syncstate-ex15websvcsotherref.md) с кодировкой base64 и атрибут **идентификатора** элемента [ItemId](itemid.md) были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-120">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="0fd2b-121">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="0fd2b-121">Request elements</span></span>

<span data-ttu-id="0fd2b-122">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0fd2b-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0fd2b-123">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0fd2b-123">SyncFolderItems</span></span>](syncfolderitems.md)
    
- [<span data-ttu-id="0fd2b-124">итемшапе</span><span class="sxs-lookup"><span data-stu-id="0fd2b-124">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="0fd2b-125">басешапе</span><span class="sxs-lookup"><span data-stu-id="0fd2b-125">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="0fd2b-126">синкфолдерид</span><span class="sxs-lookup"><span data-stu-id="0fd2b-126">SyncFolderId</span></span>](syncfolderid.md)
    
- [<span data-ttu-id="0fd2b-127">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="0fd2b-127">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="0fd2b-128">синкстате</span><span class="sxs-lookup"><span data-stu-id="0fd2b-128">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0fd2b-129">Ignore</span><span class="sxs-lookup"><span data-stu-id="0fd2b-129">Ignore</span></span>](ignore.md)
    
- [<span data-ttu-id="0fd2b-130">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="0fd2b-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="0fd2b-131">максчанжесретурнед</span><span class="sxs-lookup"><span data-stu-id="0fd2b-131">MaxChangesReturned</span></span>](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a><span data-ttu-id="0fd2b-132">Успешный ответ SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0fd2b-132">Successful SyncFolderItems Response</span></span>

### <a name="description"></a><span data-ttu-id="0fd2b-133">Description</span><span class="sxs-lookup"><span data-stu-id="0fd2b-133">Description</span></span>

<span data-ttu-id="0fd2b-134">В следующем примере показан успешный ответ на запрос SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-134">The following example shows a successful response to the SyncFolderItems request.</span></span> <span data-ttu-id="0fd2b-135">В этом примере приглашение на собрание синхронизируется из папки "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="0fd2b-135">In this example, a meeting request is synchronized from the Sent Items folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="0fd2b-136">Код</span><span class="sxs-lookup"><span data-stu-id="0fd2b-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAA=</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:MeetingRequest>
                <t:ItemId Id="AQApAHRwA==" ChangeKey="CwAAABYA" />
                <t:Subject>Budget Q3</t:Subject>
                <t:Sensitivity>Normal</t:Sensitivity>
                <t:IsOutOfDate>false</t:IsOutOfDate>
                <t:HasBeenProcessed>true</t:HasBeenProcessed>
                <t:ResponseType>NoResponseReceived</t:ResponseType>
                <t:IntendedFreeBusyStatus>Busy</t:IntendedFreeBusyStatus>
                <t:Start>2006-08-02T17:30:00Z</t:Start>
                <t:End>2006-08-02T19:30:00Z</t:End>
                <t:Location>Conference Room 2</t:Location>
                <t:Organizer>
                  <t:Mailbox>
                    <t:Name>Dan Park</t:Name>
                    <t:EmailAddress>dpark@example.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                </t:Organizer>
              </t:MeetingRequest>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="0fd2b-137">Комментарии</span><span class="sxs-lookup"><span data-stu-id="0fd2b-137">Comments</span></span>

<span data-ttu-id="0fd2b-138">Данные элемента [синкстате](syncstate-ex15websvcsotherref.md) с кодировкой base64 и атрибут **идентификатора** элемента [ItemId](itemid.md) были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-138">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="0fd2b-139">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="0fd2b-139">Successful response elements</span></span>

<span data-ttu-id="0fd2b-140">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0fd2b-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0fd2b-141">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="0fd2b-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0fd2b-142">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="0fd2b-142">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="0fd2b-143">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="0fd2b-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0fd2b-144">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="0fd2b-144">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="0fd2b-145">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0fd2b-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0fd2b-146">синкстате</span><span class="sxs-lookup"><span data-stu-id="0fd2b-146">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0fd2b-147">инклудесластитеминранже</span><span class="sxs-lookup"><span data-stu-id="0fd2b-147">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
- [<span data-ttu-id="0fd2b-148">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="0fd2b-148">Changes (Items)</span></span>](changes-items.md)
    
- [<span data-ttu-id="0fd2b-149">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="0fd2b-149">Create (ItemSync)</span></span>](create-itemsync.md)
    
- [<span data-ttu-id="0fd2b-150">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="0fd2b-150">MeetingRequest</span></span>](meetingrequest.md)
    
- [<span data-ttu-id="0fd2b-151">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="0fd2b-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="0fd2b-152">Тема</span><span class="sxs-lookup"><span data-stu-id="0fd2b-152">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="0fd2b-153">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="0fd2b-153">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="0fd2b-154">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="0fd2b-154">IsOutOfDate</span></span>](isoutofdate.md)
    
- [<span data-ttu-id="0fd2b-155">хасбинпроцессед</span><span class="sxs-lookup"><span data-stu-id="0fd2b-155">HasBeenProcessed</span></span>](hasbeenprocessed.md)
    
- [<span data-ttu-id="0fd2b-156">ResponseType</span><span class="sxs-lookup"><span data-stu-id="0fd2b-156">ResponseType</span></span>](responsetype.md)
    
- [<span data-ttu-id="0fd2b-157">интендедфрибусистатус</span><span class="sxs-lookup"><span data-stu-id="0fd2b-157">IntendedFreeBusyStatus</span></span>](intendedfreebusystatus.md)
    
- [<span data-ttu-id="0fd2b-158">Начало</span><span class="sxs-lookup"><span data-stu-id="0fd2b-158">Start</span></span>](start.md)
    
- [<span data-ttu-id="0fd2b-159">Оканчиваться</span><span class="sxs-lookup"><span data-stu-id="0fd2b-159">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0fd2b-160">Location</span><span class="sxs-lookup"><span data-stu-id="0fd2b-160">Location</span></span>](location.md)
    
- [<span data-ttu-id="0fd2b-161">Organizer</span><span class="sxs-lookup"><span data-stu-id="0fd2b-161">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="0fd2b-162">Mailbox</span><span class="sxs-lookup"><span data-stu-id="0fd2b-162">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="0fd2b-163">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0fd2b-163">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="0fd2b-164">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="0fd2b-164">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="0fd2b-165">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0fd2b-165">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a><span data-ttu-id="0fd2b-166">Ответ об ошибке SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0fd2b-166">SyncFolderItems error response</span></span>

### <a name="description"></a><span data-ttu-id="0fd2b-167">Description</span><span class="sxs-lookup"><span data-stu-id="0fd2b-167">Description</span></span>

<span data-ttu-id="0fd2b-168">В следующем примере показан ответ об ошибке для запроса SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-168">The following example shows an error response to a SyncFolderItems request.</span></span> <span data-ttu-id="0fd2b-169">Эта ошибка вызвана недопустимым Синкстате.</span><span class="sxs-lookup"><span data-stu-id="0fd2b-169">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="0fd2b-170">Код</span><span class="sxs-lookup"><span data-stu-id="0fd2b-170">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupt or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="0fd2b-171">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="0fd2b-171">Error response elements</span></span>

<span data-ttu-id="0fd2b-172">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0fd2b-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="0fd2b-173">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="0fd2b-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0fd2b-174">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="0fd2b-174">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="0fd2b-175">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="0fd2b-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0fd2b-176">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="0fd2b-176">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="0fd2b-177">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="0fd2b-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0fd2b-178">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0fd2b-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0fd2b-179">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="0fd2b-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="0fd2b-180">синкстате</span><span class="sxs-lookup"><span data-stu-id="0fd2b-180">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0fd2b-181">инклудесластитеминранже</span><span class="sxs-lookup"><span data-stu-id="0fd2b-181">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
## <a name="see-also"></a><span data-ttu-id="0fd2b-182">См. также</span><span class="sxs-lookup"><span data-stu-id="0fd2b-182">See also</span></span>



- [<span data-ttu-id="0fd2b-183">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0fd2b-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

