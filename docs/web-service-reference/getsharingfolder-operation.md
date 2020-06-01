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
description: Операция GetSharingFolder получает идентификатор локальной папки указанной общей папки.
ms.openlocfilehash: cf66eb390b0287e89bb8402f26a2e728868a2b18
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460514"
---
# <a name="getsharingfolder-operation"></a><span data-ttu-id="5b5dd-103">Операция GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="5b5dd-103">GetSharingFolder operation</span></span>

<span data-ttu-id="5b5dd-104">Операция **GetSharingFolder** получает идентификатор локальной папки указанной общей папки.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-104">The **GetSharingFolder** operation gets the local folder identifier of a specified shared folder.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="5b5dd-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="5b5dd-105">SOAP Headers</span></span>

<span data-ttu-id="5b5dd-106">Операция **GetSharingFolder** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-106">The **GetSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="5b5dd-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="5b5dd-107">**Header**</span></span>|<span data-ttu-id="5b5dd-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5b5dd-108">**Element**</span></span>|<span data-ttu-id="5b5dd-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b5dd-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5b5dd-110">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="5b5dd-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="5b5dd-111">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="5b5dd-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5b5dd-112">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="5b5dd-113">серверверсион</span><span class="sxs-lookup"><span data-stu-id="5b5dd-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="5b5dd-114">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="5b5dd-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5b5dd-115">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingfolder-request-example"></a><span data-ttu-id="5b5dd-116">Пример запроса GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="5b5dd-116">GetSharingFolder request example</span></span>

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a><span data-ttu-id="5b5dd-117">Извлечение идентификатора локальной папки, указав элемент Шаредфолдерид для общей папки</span><span class="sxs-lookup"><span data-stu-id="5b5dd-117">Getting the Local Folder Identifier by Specifying the SharedFolderId Element of the Folder Being Shared</span></span>

<span data-ttu-id="5b5dd-118">В приведенном ниже примере кода показано, как сформировать запрос на получение идентификатора локальной папки, соответствующей папке, к которой предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-118">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="5b5dd-119">Общая папка идентифицируется SMTP-адресом почтового ящика, содержащего общую папку и элемент [шаредфолдерид](sharedfolderid.md) , представляющий идентификатор этой папки.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-119">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [SharedFolderId](sharedfolderid.md) element that represents the identifier of that folder.</span></span> <span data-ttu-id="5b5dd-120">В этом примере владельцем общей папки является user1@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-120">In this example, the folder that is being shared is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5b5dd-121">Код</span><span class="sxs-lookup"><span data-stu-id="5b5dd-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a><span data-ttu-id="5b5dd-122">Извлечение идентификатора локальной папки, указав элемент DataType для общей папки</span><span class="sxs-lookup"><span data-stu-id="5b5dd-122">Getting the Local Folder Identifier by Specifying the DataType Element of the Folder Being Shared</span></span>

<span data-ttu-id="5b5dd-123">В приведенном ниже примере кода показано, как сформировать запрос на получение идентификатора локальной папки, соответствующей папке, к которой предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-123">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="5b5dd-124">Общая папка определяется SMTP-адресом почтового ящика, содержащего папку, к которой предоставлен общий доступ, и элементом [DataType](datatype.md) , представляющим тип данных в этой папке.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-124">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [DataType](datatype.md) element that represents the type of data in that folder.</span></span> <span data-ttu-id="5b5dd-125">В этом примере папкой, к которой предоставляется общий доступ, относится папка "Контакты", принадлежащая user1@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-125">In this example, the folder that is being shared is the Contacts folder that is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5b5dd-126">Код</span><span class="sxs-lookup"><span data-stu-id="5b5dd-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="5b5dd-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5b5dd-127">Comments</span></span>

<span data-ttu-id="5b5dd-128">Сведения о возможных значениях элемента **DataType** приведены в разделе [DataType](datatype.md).</span><span class="sxs-lookup"><span data-stu-id="5b5dd-128">For information about the possible values of the **DataType** element, see [DataType](datatype.md).</span></span>
  
## <a name="successful-getsharingfolder-response"></a><span data-ttu-id="5b5dd-129">Успешный ответ GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="5b5dd-129">Successful GetSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="5b5dd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5b5dd-130">Description</span></span>

<span data-ttu-id="5b5dd-131">В следующем примере показан успешный ответ на запрос **GetSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="5b5dd-131">The following example shows a successful response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="5b5dd-132">Атрибут **ID** элемента [шарингфолдерид](sharingfolderid.md) представляет идентификатор локальной папки в отношении общего доступа.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-132">The **Id** attribute of the [SharingFolderId](sharingfolderid.md) element represents the identifier of the local folder in the sharing relationship.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5b5dd-133">Код</span><span class="sxs-lookup"><span data-stu-id="5b5dd-133">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a><span data-ttu-id="5b5dd-134">Ответ об ошибке GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="5b5dd-134">GetSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="5b5dd-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5b5dd-135">Description</span></span>

<span data-ttu-id="5b5dd-136">В следующем примере показан ответ об ошибке для запроса **GetSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="5b5dd-136">The following example shows an error response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="5b5dd-137">В этом примере возникла ошибка, так как в запросе указаны элементы [шарингфолдерид](sharingfolderid.md) и [DataType](datatype.md) .</span><span class="sxs-lookup"><span data-stu-id="5b5dd-137">In this example, the error occurred because the request specified both the [SharingFolderId](sharingfolderid.md) and [DataType](datatype.md) elements.</span></span> <span data-ttu-id="5b5dd-138">Обратите внимание, что можно указать только один из этих двух элементов, но не оба.</span><span class="sxs-lookup"><span data-stu-id="5b5dd-138">Note that only one or the other of those two elements can be specified, but not both.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5b5dd-139">Код</span><span class="sxs-lookup"><span data-stu-id="5b5dd-139">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5b5dd-140">См. также</span><span class="sxs-lookup"><span data-stu-id="5b5dd-140">See also</span></span>



[<span data-ttu-id="5b5dd-141">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="5b5dd-141">GetSharingFolder</span></span>](getsharingfolder.md)
  
[<span data-ttu-id="5b5dd-142">жетшарингфолдертипе</span><span class="sxs-lookup"><span data-stu-id="5b5dd-142">GetSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[<span data-ttu-id="5b5dd-143">жетшарингфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="5b5dd-143">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md)
  
[<span data-ttu-id="5b5dd-144">жетшарингфолдерреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="5b5dd-144">GetSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="5b5dd-145">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5b5dd-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="5b5dd-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5b5dd-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

