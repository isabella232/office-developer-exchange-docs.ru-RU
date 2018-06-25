---
title: Операция GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: 75fee92a-a7f8-4a62-ad2b-17acbaada186
description: Операция GetSharingFolder Получает идентификатор локальной папки указанной общей папке.
ms.openlocfilehash: 23adb10b22623fcbc1dd6b33bd674afafdaa8b19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833670"
---
# <a name="getsharingfolder-operation"></a><span data-ttu-id="44886-103">Операция GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="44886-103">GetSharingFolder operation</span></span>

<span data-ttu-id="44886-104">Операция **GetSharingFolder** Получает идентификатор локальной папки указанной общей папке.</span><span class="sxs-lookup"><span data-stu-id="44886-104">The **GetSharingFolder** operation gets the local folder identifier of a specified shared folder.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="44886-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="44886-105">SOAP Headers</span></span>

<span data-ttu-id="44886-106">Операция **GetSharingFolder** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="44886-106">The **GetSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="44886-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="44886-107">**Header**</span></span>|<span data-ttu-id="44886-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="44886-108">**Element**</span></span>|<span data-ttu-id="44886-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44886-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="44886-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="44886-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="44886-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="44886-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="44886-112">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="44886-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="44886-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="44886-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="44886-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="44886-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="44886-115">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="44886-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingfolder-request-example"></a><span data-ttu-id="44886-116">Пример запроса GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="44886-116">GetSharingFolder request example</span></span>

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a><span data-ttu-id="44886-117">Получение идентификатора локальную папку путем указания элемент SharedFolderId общей папке</span><span class="sxs-lookup"><span data-stu-id="44886-117">Getting the Local Folder Identifier by Specifying the SharedFolderId Element of the Folder Being Shared</span></span>

<span data-ttu-id="44886-118">В следующем примере кода показано, как для формирования запроса, чтобы получить идентификатор локальной папки, соответствующее к папке, где находится в совместном.</span><span class="sxs-lookup"><span data-stu-id="44886-118">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="44886-119">К папке, где находится в совместном идентифицируется по SMTP-адрес почтового ящика, содержащем папку общий и по [SharedFolderId](sharedfolderid.md) элемент, представляющий идентификатор этой папке.</span><span class="sxs-lookup"><span data-stu-id="44886-119">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [SharedFolderId](sharedfolderid.md) element that represents the identifier of that folder.</span></span> <span data-ttu-id="44886-120">В этом примере к папке, где находится в совместном владельцем user1@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="44886-120">In this example, the folder that is being shared is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44886-121">Программа</span><span class="sxs-lookup"><span data-stu-id="44886-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:SharedFolderId>AAMkA=</m:SharedFolderId>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a><span data-ttu-id="44886-122">Начало идентификатор локальной папки, указав тип данных элемента общей папке</span><span class="sxs-lookup"><span data-stu-id="44886-122">Getting the Local Folder Identifier by Specifying the DataType Element of the Folder Being Shared</span></span>

<span data-ttu-id="44886-123">В следующем примере кода показано, как для формирования запроса, чтобы получить идентификатор локальной папки, соответствующее к папке, где находится в совместном.</span><span class="sxs-lookup"><span data-stu-id="44886-123">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="44886-124">К папке, где находится в совместном определяется путем SMTP-адрес почтового ящика, содержащем папку общий и элемент [тип данных](datatype.md) , представляющий тип данных в этой папке.</span><span class="sxs-lookup"><span data-stu-id="44886-124">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [DataType](datatype.md) element that represents the type of data in that folder.</span></span> <span data-ttu-id="44886-125">В этом примере выполняется общей папки — это папка Контакты, владельцем которого является user1@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="44886-125">In this example, the folder that is being shared is the Contacts folder that is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44886-126">Программа</span><span class="sxs-lookup"><span data-stu-id="44886-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:DataType>Contacts</m:DataType>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="44886-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="44886-127">Comments</span></span>

<span data-ttu-id="44886-128">Сведения о возможных значений элемента **типа данных** содержатся в разделе [тип данных](datatype.md).</span><span class="sxs-lookup"><span data-stu-id="44886-128">For information about the possible values of the **DataType** element, see [DataType](datatype.md).</span></span>
  
## <a name="successful-getsharingfolder-response"></a><span data-ttu-id="44886-129">Успешного ответа GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="44886-129">Successful GetSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="44886-130">Описание</span><span class="sxs-lookup"><span data-stu-id="44886-130">Description</span></span>

<span data-ttu-id="44886-131">В следующем примере показано успешного ответа на запрос **GetSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="44886-131">The following example shows a successful response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="44886-132">Атрибут **Id** элемента [SharingFolderId](sharingfolderid.md) представляет идентификатор локальной папки в отношении общего доступа.</span><span class="sxs-lookup"><span data-stu-id="44886-132">The **Id** attribute of the [SharingFolderId](sharingfolderid.md) element represents the identifier of the local folder in the sharing relationship.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44886-133">Программа</span><span class="sxs-lookup"><span data-stu-id="44886-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a><span data-ttu-id="44886-134">Ошибка GetSharingFolder ответа</span><span class="sxs-lookup"><span data-stu-id="44886-134">GetSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="44886-135">Описание</span><span class="sxs-lookup"><span data-stu-id="44886-135">Description</span></span>

<span data-ttu-id="44886-136">В следующем примере показано ошибочный ответ на запрос **GetSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="44886-136">The following example shows an error response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="44886-137">В этом примере произошла ошибка, так как запрос определенных элементов и [SharingFolderId](sharingfolderid.md) и [типа данных](datatype.md) .</span><span class="sxs-lookup"><span data-stu-id="44886-137">In this example, the error occurred because the request specified both the [SharingFolderId](sharingfolderid.md) and [DataType](datatype.md) elements.</span></span> <span data-ttu-id="44886-138">Обратите внимание на то, что только тот или иной этих двух элементов можно указать, но не оба.</span><span class="sxs-lookup"><span data-stu-id="44886-138">Note that only one or the other of those two elements can be specified, but not both.</span></span> 
  
### <a name="code"></a><span data-ttu-id="44886-139">Программа</span><span class="sxs-lookup"><span data-stu-id="44886-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="44886-140">См. также</span><span class="sxs-lookup"><span data-stu-id="44886-140">See also</span></span>



[<span data-ttu-id="44886-141">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="44886-141">GetSharingFolder</span></span>](getsharingfolder.md)
  
[<span data-ttu-id="44886-142">GetSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="44886-142">GetSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[<span data-ttu-id="44886-143">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="44886-143">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md)
  
[<span data-ttu-id="44886-144">GetSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="44886-144">GetSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="44886-145">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="44886-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="44886-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="44886-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

