---
title: Операция GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 355bcf93-dc71-4493-b177-622afac5fdb9
description: Операция с папкой возвращает папки из хранилища Exchange.
localization_priority: Priority
ms.openlocfilehash: 9d511f309b9210fd9b5a49ff6c60bc7982992973
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459183"
---
# <a name="getfolder-operation"></a><span data-ttu-id="26811-103">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="26811-103">GetFolder operation</span></span>

<span data-ttu-id="26811-104">Операция с **папкой** возвращает папки из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="26811-104">The **GetFolder** operation gets folders from the Exchange store.</span></span> 
  
## <a name="getfolder-request-example"></a><span data-ttu-id="26811-105">Пример запроса на получение вложенной папки</span><span class="sxs-lookup"><span data-stu-id="26811-105">GetFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="26811-106">Description</span><span class="sxs-lookup"><span data-stu-id="26811-106">Description</span></span>

<span data-ttu-id="26811-107">В приведенном ниже примере запроса на получение **папки** показано, как получить идентификатор папки, отображаемое имя, количество элементов в этой папке, количество дочерних папок и число непрочитанных элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="26811-107">The following example of a **GetFolder** request shows how to obtain a folder identifier, display name, the count of items in that folder, the count of child folders, and the number of unread items in the folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="26811-108">Код</span><span class="sxs-lookup"><span data-stu-id="26811-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="request-elements"></a><span data-ttu-id="26811-109">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="26811-109">Request elements</span></span>

<span data-ttu-id="26811-110">Этот запрос на получение **вложений** включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="26811-110">This **GetFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="26811-111">GetFolder</span><span class="sxs-lookup"><span data-stu-id="26811-111">GetFolder</span></span>](getfolder.md)
    
- [<span data-ttu-id="26811-112">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="26811-112">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="26811-113">басешапе</span><span class="sxs-lookup"><span data-stu-id="26811-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="26811-114">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="26811-114">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="26811-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="26811-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="26811-116">В схеме представлены дополнительные элементы, которые можно использовать для создания запроса на получение **вложенной папки** .</span><span class="sxs-lookup"><span data-stu-id="26811-116">See the schema for additional elements that you can use to form a **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="26811-117">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="26811-117">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span> 
  
## <a name="getfolder-response-example"></a><span data-ttu-id="26811-118">Пример ответа на папку GetResponse</span><span class="sxs-lookup"><span data-stu-id="26811-118">GetFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="26811-119">Description</span><span class="sxs-lookup"><span data-stu-id="26811-119">Description</span></span>

<span data-ttu-id="26811-120">В приведенном ниже примере кода для протокола SOAP показан успешный ответ на запрос на получение **папки** .</span><span class="sxs-lookup"><span data-stu-id="26811-120">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="26811-121">Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="26811-121">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="26811-122">Код</span><span class="sxs-lookup"><span data-stu-id="26811-122">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="26811-123">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="26811-123">Response elements</span></span>

<span data-ttu-id="26811-124">Этот ответ на **папку** содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="26811-124">This **GetFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="26811-125">жетфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="26811-125">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="26811-126">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="26811-126">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="26811-127">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="26811-127">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="26811-128">Folders</span><span class="sxs-lookup"><span data-stu-id="26811-128">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="26811-129">Folder</span><span class="sxs-lookup"><span data-stu-id="26811-129">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="26811-130">FolderId</span><span class="sxs-lookup"><span data-stu-id="26811-130">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="26811-131">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="26811-131">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="26811-132">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="26811-132">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="26811-133">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="26811-133">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="26811-134">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="26811-134">UnreadCount</span></span>](unreadcount.md)
    
## <a name="getfolder-error-response-example"></a><span data-ttu-id="26811-135">Пример отклика на сообщение о вложении в папку</span><span class="sxs-lookup"><span data-stu-id="26811-135">GetFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="26811-136">Description</span><span class="sxs-lookup"><span data-stu-id="26811-136">Description</span></span>

<span data-ttu-id="26811-137">В следующем примере SOAP Body показан ответ об ошибке, вызванный неправильным [FolderId](folderid.md) в запросе.</span><span class="sxs-lookup"><span data-stu-id="26811-137">The following SOAP body example shows an error response that is caused by an incorrect [FolderId](folderid.md) in the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="26811-138">Код</span><span class="sxs-lookup"><span data-stu-id="26811-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="26811-139">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="26811-139">Response elements</span></span>

<span data-ttu-id="26811-140">Сообщение **об** ошибке GetResponse содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="26811-140">This **GetFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="26811-141">жетфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="26811-141">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="26811-142">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="26811-142">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="26811-143">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="26811-143">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="26811-144">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="26811-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="26811-145">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="26811-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="26811-146">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="26811-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="26811-147">Folders</span><span class="sxs-lookup"><span data-stu-id="26811-147">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="version-differences"></a><span data-ttu-id="26811-148">Различия версий</span><span class="sxs-lookup"><span data-stu-id="26811-148">Version differences</span></span>

<span data-ttu-id="26811-149">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365, или локальной версии Exchange, начиная с Exchange 2013, разрешения для папки не возвращаются, если элемент [басешапе](baseshape.md) имеет значение **аллпропертиес** в запросе операции- [папки](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="26811-149">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="26811-150">Чтобы получить разрешения для папки, добавьте элемент [PermissionSet (пермиссионсеттипе)](permissionset-permissionsettype.md) в элемент [аддитионалпропертиес](additionalproperties.md) в запросе на получение **папки** .</span><span class="sxs-lookup"><span data-stu-id="26811-150">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="26811-151">См. также</span><span class="sxs-lookup"><span data-stu-id="26811-151">See also</span></span>



- [<span data-ttu-id="26811-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="26811-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

