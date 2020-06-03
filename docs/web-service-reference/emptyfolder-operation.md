---
title: Операция EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: Операция EmptyFolder удаляет папки в почтовом ящике. При необходимости эта операция позволяет удалить вложенные папки указанной папки. При удалении вложенной папки удаляются вложенная папка и сообщения в ней.
ms.openlocfilehash: 1913db74d33f1e6750cd158df5870f257d0e7839
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530686"
---
# <a name="emptyfolder-operation"></a><span data-ttu-id="7aea4-105">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7aea4-105">EmptyFolder operation</span></span>

<span data-ttu-id="7aea4-106">Операция **EmptyFolder** удаляет папки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7aea4-106">The **EmptyFolder** operation empties folders in a mailbox.</span></span> <span data-ttu-id="7aea4-107">При необходимости эта операция позволяет удалить вложенные папки указанной папки.</span><span class="sxs-lookup"><span data-stu-id="7aea4-107">Optionally, this operation enables you to delete the subfolders of the specified folder.</span></span> <span data-ttu-id="7aea4-108">При удалении вложенной папки удаляются вложенная папка и сообщения в ней.</span><span class="sxs-lookup"><span data-stu-id="7aea4-108">When a subfolder is deleted, the subfolder and the messages within the subfolder are deleted.</span></span> 
  
## <a name="emptyfolder-request-example"></a><span data-ttu-id="7aea4-109">Пример запроса EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7aea4-109">EmptyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="7aea4-110">Description</span><span class="sxs-lookup"><span data-stu-id="7aea4-110">Description</span></span>

<span data-ttu-id="7aea4-111">В следующем примере запроса **EmptyFolder** показано, как сформировать запрос на очистку папки.</span><span class="sxs-lookup"><span data-stu-id="7aea4-111">This following example of an **EmptyFolder** request shows how to form a request to empty a folder.</span></span> <span data-ttu-id="7aea4-112">В этом примере удаляются все вложенные папки указанной папки.</span><span class="sxs-lookup"><span data-stu-id="7aea4-112">This example deletes all subfolders of the identified folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7aea4-113">Значения **ID** и атрибуты **чанжекэй** элемента [FolderId](folderid.md) были сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7aea4-113">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7aea4-114">Код</span><span class="sxs-lookup"><span data-stu-id="7aea4-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="7aea4-115">Комментарии</span><span class="sxs-lookup"><span data-stu-id="7aea4-115">Comments</span></span>

<span data-ttu-id="7aea4-116">В этом примере выполняется окончательное удаление папки.</span><span class="sxs-lookup"><span data-stu-id="7aea4-116">This example performs a hard delete on the folder.</span></span>
  
<span data-ttu-id="7aea4-117">Папки можно определять с помощью элемента [дистингуишедфолдерид](distinguishedfolderid.md) или элемента [FolderId](folderid.md) для использования в элементе [фолдеридс](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="7aea4-117">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in the [FolderIds](folderids.md) element.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="7aea4-118">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="7aea4-118">Request elements</span></span>

<span data-ttu-id="7aea4-119">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7aea4-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7aea4-120">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7aea4-120">EmptyFolder</span></span>](emptyfolder.md)
    
- [<span data-ttu-id="7aea4-121">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="7aea4-121">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="7aea4-122">FolderId</span><span class="sxs-lookup"><span data-stu-id="7aea4-122">FolderId</span></span>](folderid.md)
    
## <a name="successful-emptyfolder-response"></a><span data-ttu-id="7aea4-123">Успешный ответ EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7aea4-123">Successful EmptyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="7aea4-124">Description</span><span class="sxs-lookup"><span data-stu-id="7aea4-124">Description</span></span>

<span data-ttu-id="7aea4-125">В следующем примере показан успешный ответ на запрос **EmptyFolder** .</span><span class="sxs-lookup"><span data-stu-id="7aea4-125">The following example shows a successful response to the **EmptyFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7aea4-126">Код</span><span class="sxs-lookup"><span data-stu-id="7aea4-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="7aea4-127">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="7aea4-127">Successful response elements</span></span>

<span data-ttu-id="7aea4-128">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7aea4-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7aea4-129">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="7aea4-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7aea4-130">емптифолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="7aea4-130">EmptyFolderResponse</span></span>](emptyfolderresponse.md)
    
- [<span data-ttu-id="7aea4-131">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="7aea4-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7aea4-132">емптифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="7aea4-132">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md)
    
- [<span data-ttu-id="7aea4-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7aea4-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="emptyfolder-error-response"></a><span data-ttu-id="7aea4-134">Ответ об ошибке EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="7aea4-134">EmptyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="7aea4-135">Description</span><span class="sxs-lookup"><span data-stu-id="7aea4-135">Description</span></span>

<span data-ttu-id="7aea4-136">В следующем примере показан ответ об ошибке для запроса **Emptyfolder** .</span><span class="sxs-lookup"><span data-stu-id="7aea4-136">The following example shows an error response to an **Emptyfolder** request.</span></span> <span data-ttu-id="7aea4-137">Ошибка была создана, так как Операция попыталась очистить папку, которая не была найдена в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7aea4-137">The error was created because the operation tried to empty a folder that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7aea4-138">Код</span><span class="sxs-lookup"><span data-stu-id="7aea4-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="error-response-elements"></a><span data-ttu-id="7aea4-139">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="7aea4-139">Error response elements</span></span>

<span data-ttu-id="7aea4-140">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7aea4-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7aea4-141">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="7aea4-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7aea4-142">жетфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="7aea4-142">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="7aea4-143">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="7aea4-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7aea4-144">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="7aea4-144">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="7aea4-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="7aea4-145">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7aea4-146">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7aea4-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7aea4-147">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="7aea4-147">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="7aea4-148">Folders</span><span class="sxs-lookup"><span data-stu-id="7aea4-148">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="7aea4-149">См. также</span><span class="sxs-lookup"><span data-stu-id="7aea4-149">See also</span></span>

- [<span data-ttu-id="7aea4-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7aea4-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

