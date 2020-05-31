---
title: Операция CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: Операция CopyFolder копирует папки в почтовом ящике.
ms.openlocfilehash: a83444ff0927a3c8fe075c79d44d02357a737773
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761835"
---
# <a name="copyfolder-operation"></a><span data-ttu-id="a568b-103">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="a568b-103">CopyFolder operation</span></span>

<span data-ttu-id="a568b-104">Операция CopyFolder копирует папки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a568b-104">The CopyFolder operation copies folders in a mailbox.</span></span>
  
## <a name="using-the-copyfolder-operation"></a><span data-ttu-id="a568b-105">Использование операции CopyFolder</span><span class="sxs-lookup"><span data-stu-id="a568b-105">Using the CopyFolder operation</span></span>

<span data-ttu-id="a568b-106">Операция CopyFolder подобна [операции MoveFolder](movefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a568b-106">The CopyFolder operation is similar to the [MoveFolder operation](movefolder-operation.md).</span></span> <span data-ttu-id="a568b-107">Он копирует идентифицированные папки и возвращает **идентификатор** и **чанжекэй** скопированных папок.</span><span class="sxs-lookup"><span data-stu-id="a568b-107">It copies identified folders and returns the **Id** and **ChangeKey** of the copied folders.</span></span> 
  
## <a name="copyfolder-request-example"></a><span data-ttu-id="a568b-108">Пример запроса CopyFolder</span><span class="sxs-lookup"><span data-stu-id="a568b-108">CopyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="a568b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a568b-109">Description</span></span>

<span data-ttu-id="a568b-110">В приведенном ниже примере запроса CopyFolder показано, как скопировать папки в папку "Входящие".</span><span class="sxs-lookup"><span data-stu-id="a568b-110">The following example of a CopyFolder request shows how to copy folders into the Inbox folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="a568b-111">Значение атрибута **ID** элемента [FolderId](folderid.md) было сокращено для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a568b-111">The value of the **Id** attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a568b-112">Код</span><span class="sxs-lookup"><span data-stu-id="a568b-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a568b-113">Comments</span><span class="sxs-lookup"><span data-stu-id="a568b-113">Comments</span></span>

<span data-ttu-id="a568b-114">Папки можно определять с помощью элемента [дистингуишедфолдерид](distinguishedfolderid.md) или элемента [FolderId](folderid.md) для использования в элементах [тофолдерид](tofolderid.md) или [фолдеридс](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="a568b-114">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in either the [ToFolderId](tofolderid.md) or the [FolderIds](folderids.md) elements.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="a568b-115">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="a568b-115">Request elements</span></span>

<span data-ttu-id="a568b-116">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a568b-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a568b-117">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="a568b-117">CopyFolder</span></span>](copyfolder.md)
    
- [<span data-ttu-id="a568b-118">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="a568b-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="a568b-119">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="a568b-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="a568b-120">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="a568b-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="a568b-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="a568b-121">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="a568b-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a568b-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="a568b-123">Чтобы найти другие параметры сообщения Request операции CopyFolder, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="a568b-123">To find other options for the request message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a568b-124">Начните с элемента [CopyFolder](copyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="a568b-124">Start at the [CopyFolder](copyfolder.md) element.</span></span> 
  
## <a name="successful-copyfolder-response"></a><span data-ttu-id="a568b-125">Успешный ответ CopyFolder</span><span class="sxs-lookup"><span data-stu-id="a568b-125">Successful CopyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="a568b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a568b-126">Description</span></span>

<span data-ttu-id="a568b-127">В следующем примере показан успешный ответ на запрос CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="a568b-127">The following example shows a successful response to the CopyFolder request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a568b-128">Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a568b-128">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a568b-129">Код</span><span class="sxs-lookup"><span data-stu-id="a568b-129">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="a568b-130">Comment</span><span class="sxs-lookup"><span data-stu-id="a568b-130">Comment</span></span>

<span data-ttu-id="a568b-131">Элемент [FolderId](folderid.md) , возвращаемый в ответе, представляет папку, скопированную в новом расположении папки.</span><span class="sxs-lookup"><span data-stu-id="a568b-131">The [FolderId](folderid.md) element that is returned in the response represents the folder that was copied in the new folder location.</span></span> 
  
### <a name="response-elements"></a><span data-ttu-id="a568b-132">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="a568b-132">Response elements</span></span>

<span data-ttu-id="a568b-133">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a568b-133">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a568b-134">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="a568b-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a568b-135">копифолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="a568b-135">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="a568b-136">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="a568b-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a568b-137">копифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a568b-137">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="a568b-138">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a568b-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a568b-139">Folders</span><span class="sxs-lookup"><span data-stu-id="a568b-139">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a568b-140">Folder</span><span class="sxs-lookup"><span data-stu-id="a568b-140">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="a568b-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="a568b-141">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="a568b-142">Чтобы найти другие параметры для ответного сообщения операции CopyFolder, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="a568b-142">To find other options for the response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a568b-143">Начните с элемента [копифолдерреспонсе](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="a568b-143">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="copyfolder-error-response"></a><span data-ttu-id="a568b-144">Ответ об ошибке CopyFolder</span><span class="sxs-lookup"><span data-stu-id="a568b-144">CopyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="a568b-145">Описание</span><span class="sxs-lookup"><span data-stu-id="a568b-145">Description</span></span>

<span data-ttu-id="a568b-146">В следующем примере показан ответ об ошибке для запроса CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="a568b-146">The following example shows an error response to a CopyFolder request.</span></span> <span data-ttu-id="a568b-147">Ошибка возникла из-за того, что папка с таким отображаемым именем уже существует.</span><span class="sxs-lookup"><span data-stu-id="a568b-147">The error occurred because a folder with the same display name already exists.</span></span>
  
### <a name="code"></a><span data-ttu-id="a568b-148">Код</span><span class="sxs-lookup"><span data-stu-id="a568b-148">Code</span></span>

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
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="a568b-149">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="a568b-149">Error response elements</span></span>

<span data-ttu-id="a568b-150">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a568b-150">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="a568b-151">копифолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="a568b-151">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="a568b-152">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="a568b-152">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a568b-153">копифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a568b-153">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="a568b-154">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="a568b-154">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a568b-155">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a568b-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a568b-156">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="a568b-156">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="a568b-157">Folders</span><span class="sxs-lookup"><span data-stu-id="a568b-157">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="a568b-158">Чтобы найти другие параметры сообщения об ошибке при выполнении операции CopyFolder, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="a568b-158">To find other options for the error response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a568b-159">Начните с элемента [копифолдерреспонсе](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="a568b-159">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a568b-160">См. также</span><span class="sxs-lookup"><span data-stu-id="a568b-160">See also</span></span>

- [<span data-ttu-id="a568b-161">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="a568b-161">MoveFolder operation</span></span>](movefolder-operation.md)
- [<span data-ttu-id="a568b-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a568b-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

