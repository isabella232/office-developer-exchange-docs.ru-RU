---
title: Операция DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: b0f92682-4895-4bcf-a4a1-e4c2e8403979
description: Операция DeleteFolder удаление папки из почтового ящика.
ms.openlocfilehash: 0fd7c9d4b04a706dcdb83f41087eaa4f3d45f129
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762033"
---
# <a name="deletefolder-operation"></a><span data-ttu-id="338df-103">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="338df-103">DeleteFolder operation</span></span>

<span data-ttu-id="338df-104">Операция **DeleteFolder** удаление папки из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="338df-104">The **DeleteFolder** operation deletes folders from a mailbox.</span></span> 
  
## <a name="deletefolder-request-example"></a><span data-ttu-id="338df-105">Пример запроса DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="338df-105">DeleteFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="338df-106">Описание</span><span class="sxs-lookup"><span data-stu-id="338df-106">Description</span></span>

<span data-ttu-id="338df-107">В следующем примере запроса **DeleteFolder** показано, как для формирования запроса, чтобы удалить папку.</span><span class="sxs-lookup"><span data-stu-id="338df-107">This following example of a **DeleteFolder** request shows how to form a request to delete a folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="338df-108">Программа</span><span class="sxs-lookup"><span data-stu-id="338df-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="338df-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="338df-109">Comments</span></span>

<span data-ttu-id="338df-110">В этом примере выполняется окончательного удаления в общей папке.</span><span class="sxs-lookup"><span data-stu-id="338df-110">This example performs a hard delete on the folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="338df-111">Идентификатор папки был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="338df-111">The folder ID has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="338df-112">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="338df-112">Request elements</span></span>

<span data-ttu-id="338df-113">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="338df-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="338df-114">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="338df-114">DeleteFolder</span></span>](deletefolder.md)
    
- [<span data-ttu-id="338df-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="338df-115">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="338df-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="338df-116">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="338df-117">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="338df-117">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="338df-118">Чтобы найти другие параметры для запроса **DeleteFolder** операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="338df-118">To find other options for the request message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="338df-119">Запустите в элементе [DeleteFolder](deletefolder.md) .</span><span class="sxs-lookup"><span data-stu-id="338df-119">Start at the [DeleteFolder](deletefolder.md) element.</span></span> 
  
## <a name="successful-deletefolder-response"></a><span data-ttu-id="338df-120">Успешного ответа DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="338df-120">Successful DeleteFolder response</span></span>

### <a name="description"></a><span data-ttu-id="338df-121">Описание</span><span class="sxs-lookup"><span data-stu-id="338df-121">Description</span></span>

<span data-ttu-id="338df-122">В следующем примере показано успешного ответа на запрос **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="338df-122">The following example shows a successful response to the **DeleteFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="338df-123">Программа</span><span class="sxs-lookup"><span data-stu-id="338df-123">Code</span></span>

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
    <DeleteFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="338df-124">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="338df-124">Response elements</span></span>

<span data-ttu-id="338df-125">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="338df-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="338df-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="338df-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="338df-127">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="338df-127">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="338df-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="338df-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="338df-129">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="338df-129">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="338df-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="338df-130">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="338df-131">Чтобы найти другие параметры в сообщении ответа **DeleteFolder** операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="338df-131">To find other options for the response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="338df-132">Запустите в элементе [DeleteFolderResponse](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="338df-132">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="deletefolder-error-response"></a><span data-ttu-id="338df-133">Отклик DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="338df-133">DeleteFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="338df-134">Описание</span><span class="sxs-lookup"><span data-stu-id="338df-134">Description</span></span>

<span data-ttu-id="338df-135">В следующем примере показано ошибочный ответ на запрос **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="338df-135">The following example shows an error response to a **DeleteFolder** request.</span></span> <span data-ttu-id="338df-136">Ошибка была вызвана запрос на удаление папки, который не был представлен в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="338df-136">The error was caused by a request to delete a folder that was not present in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="338df-137">Программа</span><span class="sxs-lookup"><span data-stu-id="338df-137">Code</span></span>

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
    <DeleteFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="338df-138">Комментарии</span><span class="sxs-lookup"><span data-stu-id="338df-138">Comments</span></span>

<span data-ttu-id="338df-139">Операция **DeleteFolder** не может использоваться для различающееся папок.</span><span class="sxs-lookup"><span data-stu-id="338df-139">The **DeleteFolder** operation cannot be used on distinguished folders.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="338df-140">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="338df-140">Error response elements</span></span>

<span data-ttu-id="338df-141">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="338df-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="338df-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="338df-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="338df-143">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="338df-143">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="338df-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="338df-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="338df-145">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="338df-145">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="338df-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="338df-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="338df-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="338df-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="338df-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="338df-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="338df-149">Чтобы найти другие параметры в сообщении об ошибке ответа **DeleteFolder** операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="338df-149">To find other options for the error response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="338df-150">Запустите в элементе [DeleteFolderResponse](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="338df-150">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="338df-151">См. также</span><span class="sxs-lookup"><span data-stu-id="338df-151">See also</span></span>

- [<span data-ttu-id="338df-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="338df-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="338df-153">Удаление папок</span><span class="sxs-lookup"><span data-stu-id="338df-153">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

