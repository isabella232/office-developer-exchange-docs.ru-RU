---
title: Операция EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: Операция EmptyFolder приводит к очистке папок в почтовом ящике. Кроме того эта операция позволяет удалять вложенные папки указанной папки. При удалении вложенной папке вложенной папке и сообщения в рамках вложенной папке удаляются.
ms.openlocfilehash: 0192744516c5a6d24b95915452bfcffecc2d92b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762326"
---
# <a name="emptyfolder-operation"></a><span data-ttu-id="46475-105">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="46475-105">EmptyFolder operation</span></span>

<span data-ttu-id="46475-106">Операция **EmptyFolder** приводит к очистке папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="46475-106">The **EmptyFolder** operation empties folders in a mailbox.</span></span> <span data-ttu-id="46475-107">Кроме того эта операция позволяет удалять вложенные папки указанной папки.</span><span class="sxs-lookup"><span data-stu-id="46475-107">Optionally, this operation enables you to delete the subfolders of the specified folder.</span></span> <span data-ttu-id="46475-108">При удалении вложенной папке вложенной папке и сообщения в рамках вложенной папке удаляются.</span><span class="sxs-lookup"><span data-stu-id="46475-108">When a subfolder is deleted, the subfolder and the messages within the subfolder are deleted.</span></span> 
  
## <a name="emptyfolder-request-example"></a><span data-ttu-id="46475-109">Пример запроса EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="46475-109">EmptyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="46475-110">Описание</span><span class="sxs-lookup"><span data-stu-id="46475-110">Description</span></span>

<span data-ttu-id="46475-111">В следующем примере запроса **EmptyFolder** показано, как для формирования запроса, чтобы полностью очистить папку.</span><span class="sxs-lookup"><span data-stu-id="46475-111">This following example of an **EmptyFolder** request shows how to form a request to empty a folder.</span></span> <span data-ttu-id="46475-112">В этом примере удаляются все вложенные папки указанной папки.</span><span class="sxs-lookup"><span data-stu-id="46475-112">This example deletes all subfolders of the identified folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="46475-113">Значения **Id** и **ChangeKey** атрибуты элемента [FolderId](folderid.md) URL были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="46475-113">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="46475-114">Программа</span><span class="sxs-lookup"><span data-stu-id="46475-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
    </soap:Header>
    <soap:Body>
      <m:EmptyFolder DeleteType="HardDelete" DeleteSubFolders="true">
        <m:FolderIds>
          <t:FolderId Id="AQMkADhhOGU0"  ChangeKey="AQAAABYAAABsMB" />
        </m:FolderIds>
      </m:EmptyFolder>
    </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="46475-115">Комментарии</span><span class="sxs-lookup"><span data-stu-id="46475-115">Comments</span></span>

<span data-ttu-id="46475-116">В этом примере выполняется окончательного удаления в общей папке.</span><span class="sxs-lookup"><span data-stu-id="46475-116">This example performs a hard delete on the folder.</span></span>
  
<span data-ttu-id="46475-117">Папки, можно определить по [DistinguishedFolderId](distinguishedfolderid.md) элемент или элемент [FolderId](folderid.md) для использования в элементе [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="46475-117">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in the [FolderIds](folderids.md) element.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="46475-118">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="46475-118">Request elements</span></span>

<span data-ttu-id="46475-119">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="46475-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="46475-120">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="46475-120">EmptyFolder</span></span>](emptyfolder.md)
    
- [<span data-ttu-id="46475-121">FolderIds</span><span class="sxs-lookup"><span data-stu-id="46475-121">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="46475-122">FolderId</span><span class="sxs-lookup"><span data-stu-id="46475-122">FolderId</span></span>](folderid.md)
    
## <a name="successful-emptyfolder-response"></a><span data-ttu-id="46475-123">Успешного ответа EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="46475-123">Successful EmptyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="46475-124">Описание</span><span class="sxs-lookup"><span data-stu-id="46475-124">Description</span></span>

<span data-ttu-id="46475-125">В следующем примере показано успешного ответа на запрос **EmptyFolder** .</span><span class="sxs-lookup"><span data-stu-id="46475-125">The following example shows a successful response to the **EmptyFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="46475-126">Программа</span><span class="sxs-lookup"><span data-stu-id="46475-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="46475-127">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="46475-127">Successful response elements</span></span>

<span data-ttu-id="46475-128">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="46475-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="46475-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="46475-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="46475-130">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="46475-130">EmptyFolderResponse</span></span>](emptyfolderresponse.md)
    
- [<span data-ttu-id="46475-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="46475-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="46475-132">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="46475-132">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md)
    
- [<span data-ttu-id="46475-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="46475-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="emptyfolder-error-response"></a><span data-ttu-id="46475-134">Ошибка EmptyFolder ответа</span><span class="sxs-lookup"><span data-stu-id="46475-134">EmptyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="46475-135">Описание</span><span class="sxs-lookup"><span data-stu-id="46475-135">Description</span></span>

<span data-ttu-id="46475-136">В следующем примере показано ошибочный ответ на запрос **Emptyfolder** .</span><span class="sxs-lookup"><span data-stu-id="46475-136">The following example shows an error response to an **Emptyfolder** request.</span></span> <span data-ttu-id="46475-137">Ошибка была создана, поскольку операции попытка очистить папку, которая не найден в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46475-137">The error was created because the operation tried to empty a folder that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="46475-138">Программа</span><span class="sxs-lookup"><span data-stu-id="46475-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="46475-139">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="46475-139">Error response elements</span></span>

<span data-ttu-id="46475-140">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="46475-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="46475-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="46475-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="46475-142">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="46475-142">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="46475-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="46475-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="46475-144">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="46475-144">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="46475-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="46475-145">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="46475-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="46475-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="46475-147">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="46475-147">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="46475-148">Папки</span><span class="sxs-lookup"><span data-stu-id="46475-148">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="46475-149">См. также</span><span class="sxs-lookup"><span data-stu-id="46475-149">See also</span></span>

- [<span data-ttu-id="46475-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46475-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

