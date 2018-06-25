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
description: Операция CopyFolder копирует папок в почтовом ящике.
ms.openlocfilehash: a83444ff0927a3c8fe075c79d44d02357a737773
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761835"
---
# <a name="copyfolder-operation"></a><span data-ttu-id="51bab-103">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="51bab-103">CopyFolder operation</span></span>

<span data-ttu-id="51bab-104">Операция CopyFolder копирует папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="51bab-104">The CopyFolder operation copies folders in a mailbox.</span></span>
  
## <a name="using-the-copyfolder-operation"></a><span data-ttu-id="51bab-105">С помощью операции CopyFolder</span><span class="sxs-lookup"><span data-stu-id="51bab-105">Using the CopyFolder operation</span></span>

<span data-ttu-id="51bab-106">Операция CopyFolder аналогичен [MoveFolder операции](movefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="51bab-106">The CopyFolder operation is similar to the [MoveFolder operation](movefolder-operation.md).</span></span> <span data-ttu-id="51bab-107">Копирует определенного папки и возвращает **идентификатор** и **ChangeKey** скопированной папки.</span><span class="sxs-lookup"><span data-stu-id="51bab-107">It copies identified folders and returns the **Id** and **ChangeKey** of the copied folders.</span></span> 
  
## <a name="copyfolder-request-example"></a><span data-ttu-id="51bab-108">Пример запроса CopyFolder</span><span class="sxs-lookup"><span data-stu-id="51bab-108">CopyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="51bab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51bab-109">Description</span></span>

<span data-ttu-id="51bab-110">В следующем примере запрос CopyFolder показано, как скопировать папок в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="51bab-110">The following example of a CopyFolder request shows how to copy folders into the Inbox folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="51bab-111">Значение атрибута **Id** элемента [FolderId](folderid.md) был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="51bab-111">The value of the **Id** attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="51bab-112">Программа</span><span class="sxs-lookup"><span data-stu-id="51bab-112">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="51bab-113">Комментарии</span><span class="sxs-lookup"><span data-stu-id="51bab-113">Comments</span></span>

<span data-ttu-id="51bab-114">Папки, можно определить по [DistinguishedFolderId](distinguishedfolderid.md) элемент или элемент [FolderId](folderid.md) для использования в либо [ToFolderId](tofolderid.md) или [FolderIds](folderids.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="51bab-114">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in either the [ToFolderId](tofolderid.md) or the [FolderIds](folderids.md) elements.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="51bab-115">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="51bab-115">Request elements</span></span>

<span data-ttu-id="51bab-116">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="51bab-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="51bab-117">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="51bab-117">CopyFolder</span></span>](copyfolder.md)
    
- [<span data-ttu-id="51bab-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="51bab-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="51bab-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="51bab-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="51bab-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="51bab-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="51bab-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="51bab-121">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="51bab-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="51bab-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="51bab-123">Чтобы найти другие параметры для запроса CopyFolder операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="51bab-123">To find other options for the request message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="51bab-124">Запустите в элементе [CopyFolder](copyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="51bab-124">Start at the [CopyFolder](copyfolder.md) element.</span></span> 
  
## <a name="successful-copyfolder-response"></a><span data-ttu-id="51bab-125">Успешного ответа CopyFolder</span><span class="sxs-lookup"><span data-stu-id="51bab-125">Successful CopyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="51bab-126">Описание</span><span class="sxs-lookup"><span data-stu-id="51bab-126">Description</span></span>

<span data-ttu-id="51bab-127">В следующем примере показано успешного ответа на запрос CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="51bab-127">The following example shows a successful response to the CopyFolder request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="51bab-128">Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="51bab-128">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="51bab-129">Программа</span><span class="sxs-lookup"><span data-stu-id="51bab-129">Code</span></span>

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

### <a name="comment"></a><span data-ttu-id="51bab-130">Комментарий</span><span class="sxs-lookup"><span data-stu-id="51bab-130">Comment</span></span>

<span data-ttu-id="51bab-131">Элемент [FolderId](folderid.md) , возвращаемого в ответе представляет папки, который скопирован в новое расположение папки.</span><span class="sxs-lookup"><span data-stu-id="51bab-131">The [FolderId](folderid.md) element that is returned in the response represents the folder that was copied in the new folder location.</span></span> 
  
### <a name="response-elements"></a><span data-ttu-id="51bab-132">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="51bab-132">Response elements</span></span>

<span data-ttu-id="51bab-133">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="51bab-133">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="51bab-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="51bab-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="51bab-135">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="51bab-135">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="51bab-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="51bab-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="51bab-137">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="51bab-137">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="51bab-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="51bab-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="51bab-139">Папки</span><span class="sxs-lookup"><span data-stu-id="51bab-139">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="51bab-140">Folder</span><span class="sxs-lookup"><span data-stu-id="51bab-140">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="51bab-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="51bab-141">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="51bab-142">Чтобы найти другие параметры в сообщении ответа CopyFolder операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="51bab-142">To find other options for the response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="51bab-143">Запустите в элементе [CopyFolderResponse](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="51bab-143">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="copyfolder-error-response"></a><span data-ttu-id="51bab-144">Отклик CopyFolder</span><span class="sxs-lookup"><span data-stu-id="51bab-144">CopyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="51bab-145">Описание</span><span class="sxs-lookup"><span data-stu-id="51bab-145">Description</span></span>

<span data-ttu-id="51bab-146">В следующем примере показано ошибочный ответ на запрос CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="51bab-146">The following example shows an error response to a CopyFolder request.</span></span> <span data-ttu-id="51bab-147">Произошла ошибка, так как папка с тем же именем отображения уже существует.</span><span class="sxs-lookup"><span data-stu-id="51bab-147">The error occurred because a folder with the same display name already exists.</span></span>
  
### <a name="code"></a><span data-ttu-id="51bab-148">Программа</span><span class="sxs-lookup"><span data-stu-id="51bab-148">Code</span></span>

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

### <a name="error-response-elements"></a><span data-ttu-id="51bab-149">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="51bab-149">Error response elements</span></span>

<span data-ttu-id="51bab-150">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="51bab-150">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="51bab-151">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="51bab-151">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="51bab-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="51bab-152">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="51bab-153">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="51bab-153">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="51bab-154">MessageText</span><span class="sxs-lookup"><span data-stu-id="51bab-154">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="51bab-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="51bab-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="51bab-156">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="51bab-156">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="51bab-157">Папки</span><span class="sxs-lookup"><span data-stu-id="51bab-157">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="51bab-158">Чтобы найти другие параметры в сообщении об ошибке ответа CopyFolder операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="51bab-158">To find other options for the error response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="51bab-159">Запустите в элементе [CopyFolderResponse](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="51bab-159">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="51bab-160">См. также</span><span class="sxs-lookup"><span data-stu-id="51bab-160">See also</span></span>

- [<span data-ttu-id="51bab-161">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="51bab-161">MoveFolder operation</span></span>](movefolder-operation.md)
- [<span data-ttu-id="51bab-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="51bab-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

