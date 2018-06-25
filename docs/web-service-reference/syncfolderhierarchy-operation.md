---
title: Операция SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: b31916b1-bc6c-4451-a475-b7c5417f752d
description: Операция SyncFolderHierarchy синхронизирует папок на компьютере, на котором выполняется Microsoft Exchange Server 2010 и клиента.
ms.openlocfilehash: 33c886d5eec64a9ff2ccc667eedfc2d4cc8dcfd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840121"
---
# <a name="syncfolderhierarchy-operation"></a><span data-ttu-id="a359a-103">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="a359a-103">SyncFolderHierarchy operation</span></span>

<span data-ttu-id="a359a-104">Операция SyncFolderHierarchy синхронизирует папок на компьютере, на котором выполняется Microsoft Exchange Server 2010 и клиента.</span><span class="sxs-lookup"><span data-stu-id="a359a-104">The SyncFolderHierarchy operation synchronizes folders between the computer that is running Microsoft Exchange Server 2010 and the client.</span></span>
  
> [!NOTE]
> <span data-ttu-id="a359a-105">При изменении свойства [UnreadCount](unreadcount.md) или [TotalCount](totalcount.md) SyncFolderHierarchy операция не возвращает папок.</span><span class="sxs-lookup"><span data-stu-id="a359a-105">The SyncFolderHierarchy operation does not return folders when the [UnreadCount](unreadcount.md) or [TotalCount](totalcount.md) properties have changed.</span></span> 
  
## <a name="syncfolderhierarchy-request-example"></a><span data-ttu-id="a359a-106">Пример запроса SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="a359a-106">SyncFolderHierarchy request example</span></span>

### <a name="description"></a><span data-ttu-id="a359a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="a359a-107">Description</span></span>

<span data-ttu-id="a359a-108">В следующем примере запрос SyncFolderHierarchy показано, как синхронизировать клиента иерархии папок на сервере Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="a359a-108">The following example of a SyncFolderHierarchy request shows how to synchronize a client folder hierarchy with the Exchange server.</span></span> <span data-ttu-id="a359a-109">В этом примере показана иерархия папок, которая уже была синхронизирована по крайней мере один раз.</span><span class="sxs-lookup"><span data-stu-id="a359a-109">This example shows a folder hierarchy that has already been synchronized at least one time.</span></span> <span data-ttu-id="a359a-110">Элемент [состояние](syncstate-ex15websvcsotherref.md) не входит в запросе для первой попытке синхронизации клиента с сервером Exchange.</span><span class="sxs-lookup"><span data-stu-id="a359a-110">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="a359a-111">Первый запрос возвращает все папки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a359a-111">The first request will return all the folders in the mailbox.</span></span> <span data-ttu-id="a359a-112">[Состояние](syncstate-ex15websvcsotherref.md) будет возвращен в [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span><span class="sxs-lookup"><span data-stu-id="a359a-112">The [SyncState](syncstate-ex15websvcsotherref.md) element will be returned in the [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span></span> <span data-ttu-id="a359a-113">Этот элемент используется для синхронизации состояния для последующих запросов SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="a359a-113">This element is used to synchronize the state for subsequent SyncFolderHierarchy requests.</span></span>
  
### <a name="code"></a><span data-ttu-id="a359a-114">Программа</span><span class="sxs-lookup"><span data-stu-id="a359a-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a359a-115">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a359a-115">Comments</span></span>

<span data-ttu-id="a359a-116">Данные элемента кодировки Base64 [состояние](syncstate-ex15websvcsotherref.md) был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a359a-116">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="a359a-117">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="a359a-117">Request elements</span></span>

<span data-ttu-id="a359a-118">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a359a-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a359a-119">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="a359a-119">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md)
    
- [<span data-ttu-id="a359a-120">FolderShape</span><span class="sxs-lookup"><span data-stu-id="a359a-120">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="a359a-121">BaseShape</span><span class="sxs-lookup"><span data-stu-id="a359a-121">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="a359a-122">Состояние</span><span class="sxs-lookup"><span data-stu-id="a359a-122">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> <span data-ttu-id="a359a-123">Схема, описывающая эти элементы находится в виртуальном каталоге EWS компьютера, на котором работает MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a359a-123">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-syncfolderhierarchy-response"></a><span data-ttu-id="a359a-124">Успешного ответа SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="a359a-124">Successful SyncFolderHierarchy Response</span></span>

### <a name="description"></a><span data-ttu-id="a359a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a359a-125">Description</span></span>

<span data-ttu-id="a359a-126">В следующем примере показано успешного ответа на запрос SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="a359a-126">The following example shows a successful response to the SyncFolderHierarchy request.</span></span> <span data-ttu-id="a359a-127">В этом примере была синхронизирована новую папку.</span><span class="sxs-lookup"><span data-stu-id="a359a-127">In this example, a new folder has been synchronized.</span></span>
  
### <a name="code"></a><span data-ttu-id="a359a-128">Программа</span><span class="sxs-lookup"><span data-stu-id="a359a-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AQApAHR=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQApA=" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>NewFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a359a-129">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a359a-129">Comments</span></span>

<span data-ttu-id="a359a-130">Данные элемента кодировки Base64 [состояние](syncstate-ex15websvcsotherref.md) и данных идентификатор папки URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a359a-130">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the folder identifier data have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="a359a-131">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="a359a-131">Successful response elements</span></span>

<span data-ttu-id="a359a-132">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a359a-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a359a-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a359a-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a359a-134">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="a359a-134">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="a359a-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a359a-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a359a-136">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a359a-136">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="a359a-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a359a-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a359a-138">Состояние</span><span class="sxs-lookup"><span data-stu-id="a359a-138">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a359a-139">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="a359a-139">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
- [<span data-ttu-id="a359a-140">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="a359a-140">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
    
- [<span data-ttu-id="a359a-141">Создание (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="a359a-141">Create (FolderSync)</span></span>](create-foldersync.md)
    
- [<span data-ttu-id="a359a-142">Folder</span><span class="sxs-lookup"><span data-stu-id="a359a-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="a359a-143">FolderId</span><span class="sxs-lookup"><span data-stu-id="a359a-143">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="a359a-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="a359a-144">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="a359a-145">FolderClass</span><span class="sxs-lookup"><span data-stu-id="a359a-145">FolderClass</span></span>](folderclass.md)
    
- [<span data-ttu-id="a359a-146">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="a359a-146">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="a359a-147">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a359a-147">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="a359a-148">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="a359a-148">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="a359a-149">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="a359a-149">UnreadCount</span></span>](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a><span data-ttu-id="a359a-150">Ошибка SyncFolderHierarchy ответа</span><span class="sxs-lookup"><span data-stu-id="a359a-150">SyncFolderHierarchy error response</span></span>

### <a name="description"></a><span data-ttu-id="a359a-151">Описание</span><span class="sxs-lookup"><span data-stu-id="a359a-151">Description</span></span>

<span data-ttu-id="a359a-152">В следующем примере показано ошибочный ответ на запрос SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="a359a-152">The following example shows an error response to a SyncFolderHierarchy request.</span></span> <span data-ttu-id="a359a-153">Эта ошибка была вызвана недопустимое состояние.</span><span class="sxs-lookup"><span data-stu-id="a359a-153">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="a359a-154">Программа</span><span class="sxs-lookup"><span data-stu-id="a359a-154">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupted or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="a359a-155">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="a359a-155">Error response elements</span></span>

<span data-ttu-id="a359a-156">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a359a-156">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="a359a-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a359a-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a359a-158">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="a359a-158">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="a359a-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a359a-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a359a-160">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a359a-160">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="a359a-161">MessageText</span><span class="sxs-lookup"><span data-stu-id="a359a-161">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a359a-162">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a359a-162">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a359a-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a359a-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="a359a-164">Состояние</span><span class="sxs-lookup"><span data-stu-id="a359a-164">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a359a-165">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="a359a-165">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
## <a name="see-also"></a><span data-ttu-id="a359a-166">См. также</span><span class="sxs-lookup"><span data-stu-id="a359a-166">See also</span></span>



- [<span data-ttu-id="a359a-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a359a-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

