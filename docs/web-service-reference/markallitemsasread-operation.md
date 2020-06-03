---
title: Операция MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: Поиск сведений о MarkAllItemsAsReadной операции EWS.
ms.openlocfilehash: aeeacea1cd5eed723f93027dd1ef75b34605fdfd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530532"
---
# <a name="markallitemsasread-operation"></a><span data-ttu-id="1fa96-103">Операция MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="1fa96-103">MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="1fa96-104">Поиск сведений о **MarkAllItemsAsReadной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="1fa96-104">Find information about the **MarkAllItemsAsRead** EWS operation.</span></span> 
  
<span data-ttu-id="1fa96-105">Операция **MarkAllItemsAsRead** устанавливает свойство- [Read](isread.md) для всех элементов в одной или нескольких папках, чтобы показать, что все элементы прочитаны или не прочитаны.</span><span class="sxs-lookup"><span data-stu-id="1fa96-105">The **MarkAllItemsAsRead** operation sets the [IsRead](isread.md) property on all items, in one or more folders, to indicate that all items are either read or unread.</span></span> 
  
<span data-ttu-id="1fa96-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1fa96-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markallitemsasread-operation"></a><span data-ttu-id="1fa96-107">Использование операции MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="1fa96-107">Using the MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="1fa96-108">С помощью операции **MarkAllItemsAsRead** можно задать свойство- [Read](isread.md) для всех элементов в папках, определенных с помощью идентификатора папки веб-служб Exchange (EWS) или имени папки Exchange по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1fa96-108">The **MarkAllItemsAsRead** operation can set the [IsRead](isread.md) property on all items in folders identified by either the Exchange Web Services (EWS) folder identifier or the default Exchange folder name.</span></span> <span data-ttu-id="1fa96-109">Операция **MarkAllItemsAsRead** также может подавлять отправку уведомлений о прочтении для элементов, помеченных как прочитанные.</span><span class="sxs-lookup"><span data-stu-id="1fa96-109">The **MarkAllItemsAsRead** operation can also suppress the sending of read receipts for items marked as read.</span></span> 
  
### <a name="markallitemsasread-operation-soap-headers"></a><span data-ttu-id="1fa96-110">Заголовки SOAP операции MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="1fa96-110">MarkAllItemsAsRead operation SOAP headers</span></span>

<span data-ttu-id="1fa96-111">Операция **MarkAllItemsAsRead** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="1fa96-111">The **MarkAllItemsAsRead** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="1fa96-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="1fa96-112">**Header name**</span></span>|<span data-ttu-id="1fa96-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1fa96-113">**Element**</span></span>|<span data-ttu-id="1fa96-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1fa96-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1fa96-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="1fa96-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="1fa96-116">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="1fa96-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1fa96-117">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="1fa96-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="1fa96-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="1fa96-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1fa96-119">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="1fa96-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="1fa96-120">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="1fa96-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="1fa96-121">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="1fa96-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="1fa96-122">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="1fa96-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1fa96-123">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="1fa96-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1fa96-124">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="1fa96-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1fa96-125">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="1fa96-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1fa96-126">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="1fa96-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1fa96-127">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="1fa96-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1fa96-128">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="1fa96-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1fa96-129">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="1fa96-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1fa96-130">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="1fa96-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a><span data-ttu-id="1fa96-131">Пример запроса операции MarkAllItemsAsRead: Пометка всех элементов в папке как прочитанных</span><span class="sxs-lookup"><span data-stu-id="1fa96-131">MarkAllItemsAsRead operation request example: Mark all items in a folder as read</span></span>

<span data-ttu-id="1fa96-132">В следующем примере запроса операции **MarkAllItemsAsRead** показано, как задать свойство- [Read](isread.md) , которое также называется флагом чтения, равное **true** всем элементам в папке.</span><span class="sxs-lookup"><span data-stu-id="1fa96-132">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property, which is also called the read flag, to **true** on all items in a folder.</span></span> <span data-ttu-id="1fa96-133">В этом примере также показано, что уведомления о прочтении не отправляются в ответ на запросы уведомления о прочтении.</span><span class="sxs-lookup"><span data-stu-id="1fa96-133">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1fa96-134">Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="1fa96-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="1fa96-135">Для этой операции не требуются ключи изменения.</span><span class="sxs-lookup"><span data-stu-id="1fa96-135">Change keys are not required for this operation.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>true</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1fa96-136">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1fa96-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1fa96-137">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="1fa96-137">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="1fa96-138">реадфлаг</span><span class="sxs-lookup"><span data-stu-id="1fa96-138">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="1fa96-139">суппрессреадрецеиптс</span><span class="sxs-lookup"><span data-stu-id="1fa96-139">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="1fa96-140">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="1fa96-140">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="1fa96-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="1fa96-141">FolderId</span></span>](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a><span data-ttu-id="1fa96-142">Успешный отклик операции MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="1fa96-142">Successful MarkAllItemsAsRead operation response</span></span>

<span data-ttu-id="1fa96-143">В следующем примере показан успешный ответ на запрос операции **MarkAllItemsAsRead** , чтобы пометить все элементы в папке как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="1fa96-143">The following example shows a successful response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="1fa96-144">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1fa96-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1fa96-145">маркаллитемсасреадреспонсе</span><span class="sxs-lookup"><span data-stu-id="1fa96-145">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="1fa96-146">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1fa96-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1fa96-147">маркаллитемсасреадреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="1fa96-147">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="1fa96-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="1fa96-148">ResponseCode</span></span>](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a><span data-ttu-id="1fa96-149">Пример запроса операции MarkAllItemsAsRead: Пометка всех элементов в папке как непрочтенных</span><span class="sxs-lookup"><span data-stu-id="1fa96-149">MarkAllItemsAsRead operation request example: Mark all items in a folder as unread</span></span>

<span data-ttu-id="1fa96-150">В приведенном ниже примере запроса операции **MarkAllItemsAsRead** показано, как задать для свойства [читал](isread.md) значение **false** для всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="1fa96-150">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property to **false** on all items in a folder.</span></span> <span data-ttu-id="1fa96-151">В этом примере также показано, что уведомления о прочтении не отправляются в ответ на запросы уведомления о прочтении.</span><span class="sxs-lookup"><span data-stu-id="1fa96-151">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>false</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1fa96-152">Успешный ответ на запрос на пометку всех элементов как прочитанных совпадает с ответом на запрос, помечающий все элементы как непрочтенные.</span><span class="sxs-lookup"><span data-stu-id="1fa96-152">A successful response to a request to mark all items as read is the same as the response to a request to mark all items as unread.</span></span>
  
<span data-ttu-id="1fa96-153">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1fa96-153">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1fa96-154">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="1fa96-154">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="1fa96-155">реадфлаг</span><span class="sxs-lookup"><span data-stu-id="1fa96-155">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="1fa96-156">суппрессреадрецеиптс</span><span class="sxs-lookup"><span data-stu-id="1fa96-156">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="1fa96-157">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="1fa96-157">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="1fa96-158">FolderId</span><span class="sxs-lookup"><span data-stu-id="1fa96-158">FolderId</span></span>](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a><span data-ttu-id="1fa96-159">Ответ об ошибке операции MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="1fa96-159">MarkAllItemsAsRead operation error response</span></span>

<span data-ttu-id="1fa96-160">В следующем примере показан ответ об ошибке запроса операции **MarkAllItemsAsRead** , чтобы пометить все элементы в папке как прочтенные или непрочтенные, если папка не существует в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1fa96-160">The following example shows an error response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read or unread when the folder does not exist in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Error">
               <m:MessageText>The specified object was not found in the store.</m:MessageText>
               <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="1fa96-161">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1fa96-161">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1fa96-162">маркаллитемсасреадреспонсе</span><span class="sxs-lookup"><span data-stu-id="1fa96-162">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="1fa96-163">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1fa96-163">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1fa96-164">маркаллитемсасреадреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="1fa96-164">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="1fa96-165">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="1fa96-165">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1fa96-166">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="1fa96-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1fa96-167">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="1fa96-167">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="1fa96-168">См. также</span><span class="sxs-lookup"><span data-stu-id="1fa96-168">See also</span></span>

- [<span data-ttu-id="1fa96-169">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1fa96-169">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="1fa96-170">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="1fa96-170">FindFolder operation</span></span>](findfolder-operation.md)
    

