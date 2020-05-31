---
title: Операция CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a10aa5e-3f25-4ec3-a0b9-284c30918a1f
description: Поиск сведений о CreateFolderPathной операции EWS.
ms.openlocfilehash: 22561e5086c144e25d7e04b68ec6674b87c4718d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761877"
---
# <a name="createfolderpath-operation"></a><span data-ttu-id="fc71c-103">Операция CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="fc71c-103">CreateFolderPath operation</span></span>

<span data-ttu-id="fc71c-104">Поиск сведений о **CreateFolderPathной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="fc71c-104">Find information about the **CreateFolderPath** EWS operation.</span></span> 
  
<span data-ttu-id="fc71c-105">Операция **CreateFolderPath** создает иерархию папок.</span><span class="sxs-lookup"><span data-stu-id="fc71c-105">The **CreateFolderPath** operation creates a folder hierarchy.</span></span> 
  
<span data-ttu-id="fc71c-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fc71c-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-createfolderpath-operation"></a><span data-ttu-id="fc71c-107">Использование операции CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="fc71c-107">Using the CreateFolderPath operation</span></span>

<span data-ttu-id="fc71c-108">Запрос операции **CreateFolderPath** принимает массив папок и идентификатор родительской папки и создает иерархию папок на основе порядка папок в массиве.</span><span class="sxs-lookup"><span data-stu-id="fc71c-108">The **CreateFolderPath** operation request takes an array of folders and a parent folder identifier and creates a folder hierarchy based on the order of the folders in the array.</span></span> 
  
### <a name="createfolderpath-operation-soap-headers"></a><span data-ttu-id="fc71c-109">Заголовки SOAP операции CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="fc71c-109">CreateFolderPath operation SOAP headers</span></span>

<span data-ttu-id="fc71c-110">Операция **CreateFolderPath** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="fc71c-110">The **CreateFolderPath** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="fc71c-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="fc71c-111">**Header name**</span></span>|<span data-ttu-id="fc71c-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc71c-112">**Element**</span></span>|<span data-ttu-id="fc71c-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc71c-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fc71c-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="fc71c-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="fc71c-115">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="fc71c-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="fc71c-116">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="fc71c-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="fc71c-117">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="fc71c-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fc71c-118">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="fc71c-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="fc71c-119">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="fc71c-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="fc71c-120">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="fc71c-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="fc71c-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="fc71c-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fc71c-122">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="fc71c-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="fc71c-123">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="fc71c-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="fc71c-124">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="fc71c-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="fc71c-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="fc71c-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fc71c-126">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="fc71c-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="fc71c-127">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fc71c-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="fc71c-128">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="fc71c-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="fc71c-129">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="fc71c-129">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="fc71c-130">**тимезонеконтекст**</span><span class="sxs-lookup"><span data-stu-id="fc71c-130">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="fc71c-131">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="fc71c-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="fc71c-132">Определяет область часового пояса для свойств **DateTime** .</span><span class="sxs-lookup"><span data-stu-id="fc71c-132">Identifies the time zone scope for **DateTime** properties.</span></span> <span data-ttu-id="fc71c-133">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="fc71c-133">This header is applicable to a request.</span></span>  <br/> |
   
## <a name="createfolderpath-operation-request-example-create-a-folder-hierarchy"></a><span data-ttu-id="fc71c-134">Пример запроса операции CreateFolderPath: создание иерархии папок</span><span class="sxs-lookup"><span data-stu-id="fc71c-134">CreateFolderPath operation request example: Create a folder hierarchy</span></span>

<span data-ttu-id="fc71c-135">В следующем примере запроса операции **CreateFolderPath** показано, как создать иерархию папок с тремя папками в папке "Входящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc71c-135">The following example of a **CreateFolderPath** operation request shows how to create a folder hierarchy that is three folders deep in the default Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fc71c-136">Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="fc71c-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="fc71c-137">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fc71c-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fc71c-138">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="fc71c-138">CreateFolderPath</span></span>](createfolderpath.md)
    
- [<span data-ttu-id="fc71c-139">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="fc71c-139">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="fc71c-140">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="fc71c-140">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="fc71c-141">релативефолдерпас</span><span class="sxs-lookup"><span data-stu-id="fc71c-141">RelativeFolderPath</span></span>](relativefolderpath.md)
    
- [<span data-ttu-id="fc71c-142">Folder</span><span class="sxs-lookup"><span data-stu-id="fc71c-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="fc71c-143">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="fc71c-143">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-createfolderpath-operation-response"></a><span data-ttu-id="fc71c-144">Успешный отклик операции CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="fc71c-144">Successful CreateFolderPath operation response</span></span>

<span data-ttu-id="fc71c-145">В следующем примере показан успешный ответ на запрос операции **CreateFolderPath** , чтобы создать иерархию папок, вложенную в папку "Входящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc71c-145">The following example shows a successful response to a **CreateFolderPath** operation request to create a folder hierarchy three folders deep in the default Inbox folder.</span></span> 
  
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

<span data-ttu-id="fc71c-146">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fc71c-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fc71c-147">креатефолдерпасреспонсе</span><span class="sxs-lookup"><span data-stu-id="fc71c-147">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="fc71c-148">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fc71c-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fc71c-149">креатефолдерпасреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fc71c-149">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="fc71c-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fc71c-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fc71c-151">Folders</span><span class="sxs-lookup"><span data-stu-id="fc71c-151">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="fc71c-152">Folder</span><span class="sxs-lookup"><span data-stu-id="fc71c-152">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="fc71c-153">FolderId</span><span class="sxs-lookup"><span data-stu-id="fc71c-153">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="fc71c-154">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="fc71c-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="fc71c-155">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="fc71c-155">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="fc71c-156">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="fc71c-156">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="fc71c-157">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="fc71c-157">UnreadCount</span></span>](unreadcount.md)
    
## <a name="createfolderpath-operation-error-response"></a><span data-ttu-id="fc71c-158">Ответ об ошибке операции CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="fc71c-158">CreateFolderPath operation error response</span></span>

<span data-ttu-id="fc71c-159">В следующем примере показан ответ об ошибке для запроса операции **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="fc71c-159">The following example shows an error response to a **CreateFolderPath** operation request.</span></span> <span data-ttu-id="fc71c-160">Это ответ на запрос на создание двух папок, для первого из которых не задано свойство отображаемого имени.</span><span class="sxs-lookup"><span data-stu-id="fc71c-160">This is a response to a request to create two folders, the first of which does not have a display name property set.</span></span> <span data-ttu-id="fc71c-161">Первая папка в иерархии не может быть создана без свойства отображаемого имени, и вторая папка не может быть создана, так как родительская папка в иерархии не была создана.</span><span class="sxs-lookup"><span data-stu-id="fc71c-161">The first folder in the hierarchy cannot be created without a display name property, and the second folder cannot be created because the parent folder in the hierarchy was not created.</span></span> 
  
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

<span data-ttu-id="fc71c-162">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fc71c-162">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fc71c-163">креатефолдерпасреспонсе</span><span class="sxs-lookup"><span data-stu-id="fc71c-163">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="fc71c-164">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fc71c-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fc71c-165">креатефолдерпасреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fc71c-165">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="fc71c-166">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="fc71c-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="fc71c-167">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fc71c-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fc71c-168">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="fc71c-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="fc71c-169">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="fc71c-169">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="fc71c-170">фиелдури</span><span class="sxs-lookup"><span data-stu-id="fc71c-170">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="fc71c-171">Folders</span><span class="sxs-lookup"><span data-stu-id="fc71c-171">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="fc71c-172">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="fc71c-172">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="fc71c-173">См. также</span><span class="sxs-lookup"><span data-stu-id="fc71c-173">See also</span></span>

- [<span data-ttu-id="fc71c-174">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="fc71c-174">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="fc71c-175">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="fc71c-175">FindFolder operation</span></span>](findfolder-operation.md)
    

