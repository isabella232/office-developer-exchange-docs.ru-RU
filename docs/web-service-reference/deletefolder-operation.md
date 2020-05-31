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
description: Операция DeleteFolder удаляет папки из почтового ящика.
ms.openlocfilehash: 0fd7c9d4b04a706dcdb83f41087eaa4f3d45f129
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762033"
---
# <a name="deletefolder-operation"></a><span data-ttu-id="c90f0-103">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c90f0-103">DeleteFolder operation</span></span>

<span data-ttu-id="c90f0-104">Операция **DeleteFolder** удаляет папки из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c90f0-104">The **DeleteFolder** operation deletes folders from a mailbox.</span></span> 
  
## <a name="deletefolder-request-example"></a><span data-ttu-id="c90f0-105">Пример запроса DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c90f0-105">DeleteFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="c90f0-106">Описание</span><span class="sxs-lookup"><span data-stu-id="c90f0-106">Description</span></span>

<span data-ttu-id="c90f0-107">В следующем примере запроса **DeleteFolder** показано, как сформировать запрос на удаление папки.</span><span class="sxs-lookup"><span data-stu-id="c90f0-107">This following example of a **DeleteFolder** request shows how to form a request to delete a folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c90f0-108">Код</span><span class="sxs-lookup"><span data-stu-id="c90f0-108">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="c90f0-109">Comments</span><span class="sxs-lookup"><span data-stu-id="c90f0-109">Comments</span></span>

<span data-ttu-id="c90f0-110">В этом примере выполняется окончательное удаление папки.</span><span class="sxs-lookup"><span data-stu-id="c90f0-110">This example performs a hard delete on the folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="c90f0-111">Идентификатор папки сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="c90f0-111">The folder ID has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="c90f0-112">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="c90f0-112">Request elements</span></span>

<span data-ttu-id="c90f0-113">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c90f0-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c90f0-114">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c90f0-114">DeleteFolder</span></span>](deletefolder.md)
    
- [<span data-ttu-id="c90f0-115">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="c90f0-115">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c90f0-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="c90f0-116">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="c90f0-117">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c90f0-117">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="c90f0-118">Чтобы найти другие параметры сообщения Request операции **DeleteFolder** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="c90f0-118">To find other options for the request message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="c90f0-119">Начните с элемента [DeleteFolder](deletefolder.md) .</span><span class="sxs-lookup"><span data-stu-id="c90f0-119">Start at the [DeleteFolder](deletefolder.md) element.</span></span> 
  
## <a name="successful-deletefolder-response"></a><span data-ttu-id="c90f0-120">Успешный ответ DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c90f0-120">Successful DeleteFolder response</span></span>

### <a name="description"></a><span data-ttu-id="c90f0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c90f0-121">Description</span></span>

<span data-ttu-id="c90f0-122">В следующем примере показан успешный ответ на запрос **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="c90f0-122">The following example shows a successful response to the **DeleteFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c90f0-123">Код</span><span class="sxs-lookup"><span data-stu-id="c90f0-123">Code</span></span>

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

### <a name="response-elements"></a><span data-ttu-id="c90f0-124">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="c90f0-124">Response elements</span></span>

<span data-ttu-id="c90f0-125">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c90f0-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c90f0-126">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="c90f0-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c90f0-127">делетефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="c90f0-127">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="c90f0-128">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="c90f0-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c90f0-129">делетефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="c90f0-129">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="c90f0-130">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="c90f0-130">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="c90f0-131">Чтобы найти другие параметры для ответного сообщения операции **DeleteFolder** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="c90f0-131">To find other options for the response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="c90f0-132">Начните с элемента [делетефолдерреспонсе](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="c90f0-132">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="deletefolder-error-response"></a><span data-ttu-id="c90f0-133">Ответ об ошибке DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="c90f0-133">DeleteFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="c90f0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c90f0-134">Description</span></span>

<span data-ttu-id="c90f0-135">В следующем примере показан ответ об ошибке для запроса **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="c90f0-135">The following example shows an error response to a **DeleteFolder** request.</span></span> <span data-ttu-id="c90f0-136">Ошибка вызвана запросом на удаление папки, которая отсутствовала в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c90f0-136">The error was caused by a request to delete a folder that was not present in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c90f0-137">Код</span><span class="sxs-lookup"><span data-stu-id="c90f0-137">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="c90f0-138">Comments</span><span class="sxs-lookup"><span data-stu-id="c90f0-138">Comments</span></span>

<span data-ttu-id="c90f0-139">Операцию **DeleteFolder** нельзя использовать для различающихся папок.</span><span class="sxs-lookup"><span data-stu-id="c90f0-139">The **DeleteFolder** operation cannot be used on distinguished folders.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="c90f0-140">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="c90f0-140">Error response elements</span></span>

<span data-ttu-id="c90f0-141">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c90f0-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="c90f0-142">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="c90f0-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c90f0-143">делетефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="c90f0-143">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="c90f0-144">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="c90f0-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c90f0-145">делетефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="c90f0-145">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="c90f0-146">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="c90f0-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c90f0-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="c90f0-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c90f0-148">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="c90f0-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="c90f0-149">Чтобы найти другие параметры сообщения об ошибке при выполнении операции **DeleteFolder** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="c90f0-149">To find other options for the error response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="c90f0-150">Начните с элемента [делетефолдерреспонсе](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="c90f0-150">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c90f0-151">См. также</span><span class="sxs-lookup"><span data-stu-id="c90f0-151">See also</span></span>

- [<span data-ttu-id="c90f0-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c90f0-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c90f0-153">Удаление папок</span><span class="sxs-lookup"><span data-stu-id="c90f0-153">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

