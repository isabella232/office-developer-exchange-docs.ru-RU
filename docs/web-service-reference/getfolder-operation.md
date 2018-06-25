---
title: GetFolder Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 355bcf93-dc71-4493-b177-622afac5fdb9
description: Операция GetFolder получает папок из хранилища Exchange.
ms.openlocfilehash: 1d2806e4febb6059b8a866d585bc70f49befbdef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762800"
---
# <a name="getfolder-operation"></a><span data-ttu-id="c439f-103">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="c439f-103">GetFolder operation</span></span>

<span data-ttu-id="c439f-104">Операция **GetFolder** получает папок из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="c439f-104">The **GetFolder** operation gets folders from the Exchange store.</span></span> 
  
## <a name="getfolder-request-example"></a><span data-ttu-id="c439f-105">Пример запроса GetFolder</span><span class="sxs-lookup"><span data-stu-id="c439f-105">GetFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="c439f-106">Описание</span><span class="sxs-lookup"><span data-stu-id="c439f-106">Description</span></span>

<span data-ttu-id="c439f-107">В следующем примере запрос **GetFolder** показано, как получить идентификатор папки, отображаются имя, число элементов в этой папке, количество дочерних папок и количество непрочитанных элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="c439f-107">The following example of a **GetFolder** request shows how to obtain a folder identifier, display name, the count of items in that folder, the count of child folders, and the number of unread items in the folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c439f-108">Программа</span><span class="sxs-lookup"><span data-stu-id="c439f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <FolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </FolderIds>
    </GetFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="c439f-109">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="c439f-109">Request elements</span></span>

<span data-ttu-id="c439f-110">Этот запрос **GetFolder** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c439f-110">This **GetFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="c439f-111">GetFolder</span><span class="sxs-lookup"><span data-stu-id="c439f-111">GetFolder</span></span>](getfolder.md)
    
- [<span data-ttu-id="c439f-112">FolderShape</span><span class="sxs-lookup"><span data-stu-id="c439f-112">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="c439f-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="c439f-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="c439f-114">FolderIds</span><span class="sxs-lookup"><span data-stu-id="c439f-114">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c439f-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c439f-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="c439f-116">В разделе Схема дополнительных элементов, которые можно использовать для формирования запроса **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="c439f-116">See the schema for additional elements that you can use to form a **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c439f-117">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c439f-117">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span> 
  
## <a name="getfolder-response-example"></a><span data-ttu-id="c439f-118">Пример ответа GetFolder</span><span class="sxs-lookup"><span data-stu-id="c439f-118">GetFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="c439f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c439f-119">Description</span></span>

<span data-ttu-id="c439f-120">В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="c439f-120">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c439f-121">Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="c439f-121">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c439f-122">Программа</span><span class="sxs-lookup"><span data-stu-id="c439f-122">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AQApA=" ChangeKey="AQAAAB" />
              <t:DisplayName>Inbox</t:DisplayName>
              <t:TotalCount>2</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:UnreadCount>2</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </GetFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="c439f-123">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="c439f-123">Response elements</span></span>

<span data-ttu-id="c439f-124">В этом ответа **GetFolder** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c439f-124">This **GetFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="c439f-125">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c439f-125">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="c439f-126">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c439f-126">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c439f-127">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c439f-127">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="c439f-128">Папки</span><span class="sxs-lookup"><span data-stu-id="c439f-128">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c439f-129">Folder</span><span class="sxs-lookup"><span data-stu-id="c439f-129">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="c439f-130">FolderId</span><span class="sxs-lookup"><span data-stu-id="c439f-130">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="c439f-131">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="c439f-131">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="c439f-132">TotalCount</span><span class="sxs-lookup"><span data-stu-id="c439f-132">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="c439f-133">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="c439f-133">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="c439f-134">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="c439f-134">UnreadCount</span></span>](unreadcount.md)
    
## <a name="getfolder-error-response-example"></a><span data-ttu-id="c439f-135">Пример ответа об ошибке GetFolder</span><span class="sxs-lookup"><span data-stu-id="c439f-135">GetFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c439f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c439f-136">Description</span></span>

<span data-ttu-id="c439f-137">В следующем примере тело SOAP показано ответ на ошибку, связанную с неправильной [FolderId](folderid.md) в запросе.</span><span class="sxs-lookup"><span data-stu-id="c439f-137">The following SOAP body example shows an error response that is caused by an incorrect [FolderId](folderid.md) in the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c439f-138">Программа</span><span class="sxs-lookup"><span data-stu-id="c439f-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </GetFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="c439f-139">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="c439f-139">Response elements</span></span>

<span data-ttu-id="c439f-140">Отклик в этом **GetFolder** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c439f-140">This **GetFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="c439f-141">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c439f-141">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="c439f-142">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c439f-142">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c439f-143">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c439f-143">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="c439f-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="c439f-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c439f-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c439f-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c439f-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c439f-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="c439f-147">Папки</span><span class="sxs-lookup"><span data-stu-id="c439f-147">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="version-differences"></a><span data-ttu-id="c439f-148">Различия версий</span><span class="sxs-lookup"><span data-stu-id="c439f-148">Version differences</span></span>

<span data-ttu-id="c439f-149">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange 2013 разрешения папок не возвращаются при [BaseShape](baseshape.md) элемент имеет значение **AllProperties** в запросе [GetFolder](getfolder-operation.md) операции.</span><span class="sxs-lookup"><span data-stu-id="c439f-149">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="c439f-150">Для получения разрешений для папки, добавьте в элемент [AdditionalProperties](additionalproperties.md) в запросе **GetFolder** элемент [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) .</span><span class="sxs-lookup"><span data-stu-id="c439f-150">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c439f-151">См. также</span><span class="sxs-lookup"><span data-stu-id="c439f-151">See also</span></span>



- [<span data-ttu-id="c439f-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c439f-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

