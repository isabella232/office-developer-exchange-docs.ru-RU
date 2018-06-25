---
title: Операция CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a10aa5e-3f25-4ec3-a0b9-284c30918a1f
description: Найдите сведения о веб-служб Exchange CreateFolderPath операции.
ms.openlocfilehash: 22561e5086c144e25d7e04b68ec6674b87c4718d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761877"
---
# <a name="createfolderpath-operation"></a><span data-ttu-id="1737f-103">Операция CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="1737f-103">CreateFolderPath operation</span></span>

<span data-ttu-id="1737f-104">Найдите сведения о **CreateFolderPath** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1737f-104">Find information about the **CreateFolderPath** EWS operation.</span></span> 
  
<span data-ttu-id="1737f-105">Операция **CreateFolderPath** создает иерархии папок.</span><span class="sxs-lookup"><span data-stu-id="1737f-105">The **CreateFolderPath** operation creates a folder hierarchy.</span></span> 
  
<span data-ttu-id="1737f-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1737f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-createfolderpath-operation"></a><span data-ttu-id="1737f-107">С помощью операции CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="1737f-107">Using the CreateFolderPath operation</span></span>

<span data-ttu-id="1737f-108">Запрос операции **CreateFolderPath** принимает массив папки и идентификатор родительской папки и создает иерархии папок, на основе порядка папок в массиве.</span><span class="sxs-lookup"><span data-stu-id="1737f-108">The **CreateFolderPath** operation request takes an array of folders and a parent folder identifier and creates a folder hierarchy based on the order of the folders in the array.</span></span> 
  
### <a name="createfolderpath-operation-soap-headers"></a><span data-ttu-id="1737f-109">Заголовки SOAP CreateFolderPath операции</span><span class="sxs-lookup"><span data-stu-id="1737f-109">CreateFolderPath operation SOAP headers</span></span>

<span data-ttu-id="1737f-110">Операция **CreateFolderPath** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1737f-110">The **CreateFolderPath** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="1737f-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="1737f-111">**Header name**</span></span>|<span data-ttu-id="1737f-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1737f-112">**Element**</span></span>|<span data-ttu-id="1737f-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1737f-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1737f-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="1737f-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="1737f-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1737f-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1737f-116">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="1737f-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="1737f-117">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="1737f-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1737f-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="1737f-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="1737f-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="1737f-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="1737f-120">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="1737f-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="1737f-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="1737f-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1737f-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1737f-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1737f-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1737f-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1737f-124">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="1737f-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1737f-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="1737f-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1737f-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1737f-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1737f-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1737f-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1737f-128">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="1737f-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1737f-129">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="1737f-129">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="1737f-130">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="1737f-130">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="1737f-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="1737f-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="1737f-132">Определяет область часовой пояс для свойства **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="1737f-132">Identifies the time zone scope for **DateTime** properties.</span></span> <span data-ttu-id="1737f-133">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="1737f-133">This header is applicable to a request.</span></span>  <br/> |
   
## <a name="createfolderpath-operation-request-example-create-a-folder-hierarchy"></a><span data-ttu-id="1737f-134">Пример запроса CreateFolderPath операции: создание иерархии папок</span><span class="sxs-lookup"><span data-stu-id="1737f-134">CreateFolderPath operation request example: Create a folder hierarchy</span></span>

<span data-ttu-id="1737f-135">В следующем примере запрос операции **CreateFolderPath** показано, как создать структуру иерархии папок, который является три папки глубоко в папке "Входящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1737f-135">The following example of a **CreateFolderPath** operation request shows how to create a folder hierarchy that is three folders deep in the default Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1737f-136">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="1737f-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:CreateFolderPath>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ParentFolderId>
         <m:RelativeFolderPath>
            <t:Folder>
               <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MySecondLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
            </t:Folder>
         </m:RelativeFolderPath>
      </m:CreateFolderPath>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="1737f-137">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1737f-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1737f-138">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="1737f-138">CreateFolderPath</span></span>](createfolderpath.md)
    
- [<span data-ttu-id="1737f-139">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="1737f-139">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="1737f-140">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="1737f-140">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="1737f-141">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="1737f-141">RelativeFolderPath</span></span>](relativefolderpath.md)
    
- [<span data-ttu-id="1737f-142">Folder</span><span class="sxs-lookup"><span data-stu-id="1737f-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="1737f-143">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="1737f-143">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-createfolderpath-operation-response"></a><span data-ttu-id="1737f-144">Успешные операции ответа CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="1737f-144">Successful CreateFolderPath operation response</span></span>

<span data-ttu-id="1737f-145">В следующем примере показано успешного ответа на запрос операции **CreateFolderPath** для создания папки три иерархии папок глубоко в папке "Входящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1737f-145">The following example shows a successful response to a **CreateFolderPath** operation request to create a folder hierarchy three folders deep in the default Inbox folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExYisXAAA=" ChangeKey="AQAAABYAABq6Wxb"/>
                     <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExm4QrAABqxisYAAA=" ChangeKey="AQAAABYAAAm4QrAABq6Wxg"/>
                     <t:DisplayName>MySecondLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTAABqxisZAAA=" ChangeKey="AQAAABYAA6Wxl"/>
                     <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="1737f-146">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1737f-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1737f-147">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="1737f-147">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="1737f-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1737f-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1737f-149">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1737f-149">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="1737f-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1737f-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1737f-151">Папки</span><span class="sxs-lookup"><span data-stu-id="1737f-151">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="1737f-152">Folder</span><span class="sxs-lookup"><span data-stu-id="1737f-152">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="1737f-153">FolderId</span><span class="sxs-lookup"><span data-stu-id="1737f-153">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="1737f-154">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="1737f-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="1737f-155">TotalCount</span><span class="sxs-lookup"><span data-stu-id="1737f-155">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="1737f-156">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="1737f-156">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="1737f-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="1737f-157">UnreadCount</span></span>](unreadcount.md)
    
## <a name="createfolderpath-operation-error-response"></a><span data-ttu-id="1737f-158">Ошибка операции CreateFolderPath ответа</span><span class="sxs-lookup"><span data-stu-id="1737f-158">CreateFolderPath operation error response</span></span>

<span data-ttu-id="1737f-159">В следующем примере показано ошибочный ответ на запрос операции **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="1737f-159">The following example shows an error response to a **CreateFolderPath** operation request.</span></span> <span data-ttu-id="1737f-160">Это ответ на запрос для создания двух папок, первая из которых имеет задать свойство отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="1737f-160">This is a response to a request to create two folders, the first of which does not have a display name property set.</span></span> <span data-ttu-id="1737f-161">Не удается создать первый папку в иерархии без отображаемое имя свойства и не удается создать второй папку, так как не был создан родительской папки в иерархии.</span><span class="sxs-lookup"><span data-stu-id="1737f-161">The first folder in the hierarchy cannot be created without a display name property, and the second folder cannot be created because the parent folder in the hierarchy was not created.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The folder save operation failed due to invalid property values.</m:MessageText>
               <m:ResponseCode>ErrorFolderSavePropertyError</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:MessageXml>
                  <t:FieldURI FieldURI="folder:DisplayName"/>
               </m:MessageXml>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The specified parent folder could not be found.</m:MessageText>
               <m:ResponseCode>ErrorParentFolderNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="1737f-162">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1737f-162">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1737f-163">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="1737f-163">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="1737f-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1737f-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1737f-165">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1737f-165">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="1737f-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="1737f-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1737f-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1737f-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1737f-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1737f-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="1737f-169">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1737f-169">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="1737f-170">FieldURI</span><span class="sxs-lookup"><span data-stu-id="1737f-170">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="1737f-171">Папки</span><span class="sxs-lookup"><span data-stu-id="1737f-171">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="1737f-172">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="1737f-172">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1737f-173">См. также</span><span class="sxs-lookup"><span data-stu-id="1737f-173">See also</span></span>

- [<span data-ttu-id="1737f-174">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1737f-174">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="1737f-175">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="1737f-175">FindFolder operation</span></span>](findfolder-operation.md)
    

