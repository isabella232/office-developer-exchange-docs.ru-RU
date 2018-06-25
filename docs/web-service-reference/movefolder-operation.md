---
title: Операция MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: c7233966-6c87-4a14-8156-b1610760176d
description: Операция MoveFolder перемещение папок из указанной папки и помещает их в другую папку.
ms.openlocfilehash: 5da6929f11ce9ba74db190db6d799f25974d2192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834490"
---
# <a name="movefolder-operation"></a><span data-ttu-id="a0254-103">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="a0254-103">MoveFolder operation</span></span>

<span data-ttu-id="a0254-104">Операция MoveFolder перемещение папок из указанной папки и помещает их в другую папку.</span><span class="sxs-lookup"><span data-stu-id="a0254-104">The MoveFolder operation moves folders from a specified folder and puts them in another folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0254-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="a0254-105">Remarks</span></span>

<span data-ttu-id="a0254-106">Операция MoveFolder аналогичен CopyFolder операции.</span><span class="sxs-lookup"><span data-stu-id="a0254-106">The MoveFolder operation is similar to the CopyFolder operation.</span></span> <span data-ttu-id="a0254-107">Невозможно переместить именованные папки.</span><span class="sxs-lookup"><span data-stu-id="a0254-107">You cannot move distinguished folders.</span></span> <span data-ttu-id="a0254-108">Можно переместить несколько папок одновременно в конечную папку.</span><span class="sxs-lookup"><span data-stu-id="a0254-108">You can move multiple folders at one time to the destination folder.</span></span>
  
## <a name="movefolder-request-example"></a><span data-ttu-id="a0254-109">Пример запроса MoveFolder</span><span class="sxs-lookup"><span data-stu-id="a0254-109">MoveFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="a0254-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a0254-110">Description</span></span>

<span data-ttu-id="a0254-111">В следующем примере запрос MoveFolder показано, как для формирования запроса, чтобы переместить папку, определяемую средством [FolderId](folderid.md) и поместите папки в папку нежелательной почты различающееся.</span><span class="sxs-lookup"><span data-stu-id="a0254-111">The following example of a MoveFolder request shows how to form a request to move a folder identified by the [FolderId](folderid.md) and put the folder in the Junk E-mail distinguished folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a0254-112">Программа</span><span class="sxs-lookup"><span data-stu-id="a0254-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="junkemail"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AScAc"/>
      </FolderIds>
    </MoveFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a0254-113">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a0254-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="a0254-114">Значение атрибута ID элемента [FolderId](folderid.md) был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="a0254-114">The value of the ID attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="a0254-115">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="a0254-115">Request elements</span></span>

<span data-ttu-id="a0254-116">Этот запрос MoveFolder содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a0254-116">This MoveFolder request includes the following elements:</span></span>
  
- [<span data-ttu-id="a0254-117">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="a0254-117">MoveFolder</span></span>](movefolder.md)
    
- [<span data-ttu-id="a0254-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="a0254-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="a0254-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="a0254-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="a0254-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="a0254-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="a0254-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="a0254-121">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="a0254-122">В разделе Схема дополнительных элементов, которые можно использовать для формирования запроса MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="a0254-122">See the schema for additional elements that you can use to form a MoveFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="a0254-123">Расположение по умолчанию схемы находится в виртуальном каталоге EWS на компьютере, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a0254-123">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="successful-movefolder-response-example"></a><span data-ttu-id="a0254-124">Пример успешного ответа MoveFolder</span><span class="sxs-lookup"><span data-stu-id="a0254-124">Successful MoveFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="a0254-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a0254-125">Description</span></span>

<span data-ttu-id="a0254-126">В следующем примере показано успешного ответа на запрос MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="a0254-126">The following example shows a successful response to the MoveFolder request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a0254-127">Программа</span><span class="sxs-lookup"><span data-stu-id="a0254-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFV" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a0254-128">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a0254-128">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="a0254-129">Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a0254-129">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="a0254-130">FolderId, возвращаемого в ответе представляет к папке, где был перемещен в новый путь к папке.</span><span class="sxs-lookup"><span data-stu-id="a0254-130">The FolderId that is returned in the response represents the folder that was moved to the new the folder location.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="a0254-131">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="a0254-131">Response elements</span></span>

<span data-ttu-id="a0254-132">Ответ MoveFolder содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a0254-132">The MoveFolder response includes the following elements:</span></span>
  
- [<span data-ttu-id="a0254-133">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a0254-133">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="a0254-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a0254-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a0254-135">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a0254-135">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="a0254-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a0254-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a0254-137">Папки</span><span class="sxs-lookup"><span data-stu-id="a0254-137">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a0254-138">Folder</span><span class="sxs-lookup"><span data-stu-id="a0254-138">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="a0254-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="a0254-139">FolderId</span></span>](folderid.md)
    
## <a name="movefolder-error-response-example"></a><span data-ttu-id="a0254-140">Пример ответа об ошибке MoveFolder</span><span class="sxs-lookup"><span data-stu-id="a0254-140">MoveFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="a0254-141">Описание</span><span class="sxs-lookup"><span data-stu-id="a0254-141">Description</span></span>

<span data-ttu-id="a0254-142">В следующем примере показано возврату ошибки, что происходит при попытке перемещения именованной папки.</span><span class="sxs-lookup"><span data-stu-id="a0254-142">The following example shows an error response that occurs when you try to move a distinguished folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="a0254-143">Программа</span><span class="sxs-lookup"><span data-stu-id="a0254-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot move distinguished folder.</m:MessageText>
          <m:ResponseCode>ErrorMoveDistinguishedFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="a0254-144">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="a0254-144">Error response elements</span></span>

<span data-ttu-id="a0254-145">Отклик MoveFolder содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a0254-145">The MoveFolder error response includes the following elements:</span></span>
  
- [<span data-ttu-id="a0254-146">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a0254-146">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="a0254-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a0254-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a0254-148">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a0254-148">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="a0254-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="a0254-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a0254-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a0254-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a0254-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a0254-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="a0254-152">Папки</span><span class="sxs-lookup"><span data-stu-id="a0254-152">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="a0254-153">См. также</span><span class="sxs-lookup"><span data-stu-id="a0254-153">See also</span></span>



[<span data-ttu-id="a0254-154">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="a0254-154">CopyFolder operation</span></span>](copyfolder-operation.md)

