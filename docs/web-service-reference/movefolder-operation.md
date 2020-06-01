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
description: Операция MoveFolder перемещает папки из указанной папки и размещает их в другой папке.
ms.openlocfilehash: dc572130ca3b2f2b152abbb4a8b68cc6f67790e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460584"
---
# <a name="movefolder-operation"></a><span data-ttu-id="c62b2-103">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="c62b2-103">MoveFolder operation</span></span>

<span data-ttu-id="c62b2-104">Операция MoveFolder перемещает папки из указанной папки и размещает их в другой папке.</span><span class="sxs-lookup"><span data-stu-id="c62b2-104">The MoveFolder operation moves folders from a specified folder and puts them in another folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c62b2-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="c62b2-105">Remarks</span></span>

<span data-ttu-id="c62b2-106">Операция MoveFolder подобна операции CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="c62b2-106">The MoveFolder operation is similar to the CopyFolder operation.</span></span> <span data-ttu-id="c62b2-107">Невозможно переместить папки "различающиеся папки".</span><span class="sxs-lookup"><span data-stu-id="c62b2-107">You cannot move distinguished folders.</span></span> <span data-ttu-id="c62b2-108">В целевую папку можно переместить сразу несколько папок.</span><span class="sxs-lookup"><span data-stu-id="c62b2-108">You can move multiple folders at one time to the destination folder.</span></span>
  
## <a name="movefolder-request-example"></a><span data-ttu-id="c62b2-109">Пример запроса MoveFolder</span><span class="sxs-lookup"><span data-stu-id="c62b2-109">MoveFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="c62b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c62b2-110">Description</span></span>

<span data-ttu-id="c62b2-111">В приведенном ниже примере запроса MoveFolder показано, как создать запрос на перемещение папки, определенной [FolderId](folderid.md) , и поместить ее в папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="c62b2-111">The following example of a MoveFolder request shows how to form a request to move a folder identified by the [FolderId](folderid.md) and put the folder in the Junk E-mail distinguished folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c62b2-112">Код</span><span class="sxs-lookup"><span data-stu-id="c62b2-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="c62b2-113">Комментарии</span><span class="sxs-lookup"><span data-stu-id="c62b2-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="c62b2-114">Значение атрибута ID элемента [FolderId](folderid.md) было сокращено для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c62b2-114">The value of the ID attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="c62b2-115">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="c62b2-115">Request elements</span></span>

<span data-ttu-id="c62b2-116">Этот запрос MoveFolder включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c62b2-116">This MoveFolder request includes the following elements:</span></span>
  
- [<span data-ttu-id="c62b2-117">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="c62b2-117">MoveFolder</span></span>](movefolder.md)
    
- [<span data-ttu-id="c62b2-118">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="c62b2-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="c62b2-119">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="c62b2-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="c62b2-120">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="c62b2-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c62b2-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="c62b2-121">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="c62b2-122">В схеме представлены дополнительные элементы, которые можно использовать для формирования запроса MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="c62b2-122">See the schema for additional elements that you can use to form a MoveFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="c62b2-123">Расположение схемы по умолчанию находится в виртуальном каталоге EWS на компьютере, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c62b2-123">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="successful-movefolder-response-example"></a><span data-ttu-id="c62b2-124">Пример успешного ответа MoveFolder</span><span class="sxs-lookup"><span data-stu-id="c62b2-124">Successful MoveFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="c62b2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c62b2-125">Description</span></span>

<span data-ttu-id="c62b2-126">В следующем примере показан успешный ответ на запрос MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="c62b2-126">The following example shows a successful response to the MoveFolder request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c62b2-127">Код</span><span class="sxs-lookup"><span data-stu-id="c62b2-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="c62b2-128">Комментарии</span><span class="sxs-lookup"><span data-stu-id="c62b2-128">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="c62b2-129">Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="c62b2-129">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="c62b2-130">FolderId, возвращаемый в ответе, представляет папку, которая была перемещена в новое расположение папки.</span><span class="sxs-lookup"><span data-stu-id="c62b2-130">The FolderId that is returned in the response represents the folder that was moved to the new the folder location.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="c62b2-131">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="c62b2-131">Response elements</span></span>

<span data-ttu-id="c62b2-132">Ответ MoveFolder включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c62b2-132">The MoveFolder response includes the following elements:</span></span>
  
- [<span data-ttu-id="c62b2-133">мовефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="c62b2-133">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="c62b2-134">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="c62b2-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c62b2-135">мовефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="c62b2-135">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="c62b2-136">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="c62b2-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c62b2-137">Folders</span><span class="sxs-lookup"><span data-stu-id="c62b2-137">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c62b2-138">Folder</span><span class="sxs-lookup"><span data-stu-id="c62b2-138">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="c62b2-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="c62b2-139">FolderId</span></span>](folderid.md)
    
## <a name="movefolder-error-response-example"></a><span data-ttu-id="c62b2-140">Пример ответа на сообщение об ошибке MoveFolder</span><span class="sxs-lookup"><span data-stu-id="c62b2-140">MoveFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c62b2-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c62b2-141">Description</span></span>

<span data-ttu-id="c62b2-142">В следующем примере показан ответ об ошибке, возникающий при попытке переместить различающиеся папки.</span><span class="sxs-lookup"><span data-stu-id="c62b2-142">The following example shows an error response that occurs when you try to move a distinguished folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="c62b2-143">Код</span><span class="sxs-lookup"><span data-stu-id="c62b2-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="c62b2-144">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="c62b2-144">Error response elements</span></span>

<span data-ttu-id="c62b2-145">Ответ об ошибке MoveFolder включает следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c62b2-145">The MoveFolder error response includes the following elements:</span></span>
  
- [<span data-ttu-id="c62b2-146">мовефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="c62b2-146">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="c62b2-147">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="c62b2-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c62b2-148">мовефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="c62b2-148">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="c62b2-149">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="c62b2-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c62b2-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="c62b2-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c62b2-151">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="c62b2-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="c62b2-152">Folders</span><span class="sxs-lookup"><span data-stu-id="c62b2-152">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="c62b2-153">См. также</span><span class="sxs-lookup"><span data-stu-id="c62b2-153">See also</span></span>



[<span data-ttu-id="c62b2-154">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="c62b2-154">CopyFolder operation</span></span>](copyfolder-operation.md)

