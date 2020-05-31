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
description: Операция SyncFolderHierarchy синхронизирует папки между компьютером, на котором работает Microsoft Exchange Server 2010 и клиентом.
ms.openlocfilehash: 33c886d5eec64a9ff2ccc667eedfc2d4cc8dcfd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840121"
---
# <a name="syncfolderhierarchy-operation"></a><span data-ttu-id="1c208-103">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="1c208-103">SyncFolderHierarchy operation</span></span>

<span data-ttu-id="1c208-104">Операция SyncFolderHierarchy синхронизирует папки между компьютером, на котором работает Microsoft Exchange Server 2010 и клиентом.</span><span class="sxs-lookup"><span data-stu-id="1c208-104">The SyncFolderHierarchy operation synchronizes folders between the computer that is running Microsoft Exchange Server 2010 and the client.</span></span>
  
> [!NOTE]
> <span data-ttu-id="1c208-105">Операция SyncFolderHierarchy не возвращает папки при изменении свойств [унреадкаунт](unreadcount.md) или [тоталкаунт](totalcount.md) .</span><span class="sxs-lookup"><span data-stu-id="1c208-105">The SyncFolderHierarchy operation does not return folders when the [UnreadCount](unreadcount.md) or [TotalCount](totalcount.md) properties have changed.</span></span> 
  
## <a name="syncfolderhierarchy-request-example"></a><span data-ttu-id="1c208-106">Пример запроса SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="1c208-106">SyncFolderHierarchy request example</span></span>

### <a name="description"></a><span data-ttu-id="1c208-107">Описание</span><span class="sxs-lookup"><span data-stu-id="1c208-107">Description</span></span>

<span data-ttu-id="1c208-108">В приведенном ниже примере запроса SyncFolderHierarchy показано, как синхронизировать иерархию клиентских папок с сервером Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c208-108">The following example of a SyncFolderHierarchy request shows how to synchronize a client folder hierarchy with the Exchange server.</span></span> <span data-ttu-id="1c208-109">В этом примере показана иерархия папок, которая уже синхронизирована по крайней мере один раз.</span><span class="sxs-lookup"><span data-stu-id="1c208-109">This example shows a folder hierarchy that has already been synchronized at least one time.</span></span> <span data-ttu-id="1c208-110">Элемент [синкстате](syncstate-ex15websvcsotherref.md) не включается в запрос первой попытки синхронизации клиента с сервером Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c208-110">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="1c208-111">Первый запрос возвратит все папки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1c208-111">The first request will return all the folders in the mailbox.</span></span> <span data-ttu-id="1c208-112">Элемент [синкстате](syncstate-ex15websvcsotherref.md) будет возвращен в [синкфолдерхиерарчиреспонсе](syncfolderhierarchyresponse.md).</span><span class="sxs-lookup"><span data-stu-id="1c208-112">The [SyncState](syncstate-ex15websvcsotherref.md) element will be returned in the [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span></span> <span data-ttu-id="1c208-113">Этот элемент используется для синхронизации состояния последующих запросов SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="1c208-113">This element is used to synchronize the state for subsequent SyncFolderHierarchy requests.</span></span>
  
### <a name="code"></a><span data-ttu-id="1c208-114">Код</span><span class="sxs-lookup"><span data-stu-id="1c208-114">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="1c208-115">Comments</span><span class="sxs-lookup"><span data-stu-id="1c208-115">Comments</span></span>

<span data-ttu-id="1c208-116">Данные элемента [синкстате](syncstate-ex15websvcsotherref.md) с кодировкой base64 были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c208-116">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="1c208-117">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="1c208-117">Request elements</span></span>

<span data-ttu-id="1c208-118">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1c208-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="1c208-119">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="1c208-119">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md)
    
- [<span data-ttu-id="1c208-120">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="1c208-120">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="1c208-121">басешапе</span><span class="sxs-lookup"><span data-stu-id="1c208-121">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="1c208-122">синкстате</span><span class="sxs-lookup"><span data-stu-id="1c208-122">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> <span data-ttu-id="1c208-123">Схема, описывающая эти элементы, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Майкрософт Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1c208-123">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-syncfolderhierarchy-response"></a><span data-ttu-id="1c208-124">Успешный ответ SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="1c208-124">Successful SyncFolderHierarchy Response</span></span>

### <a name="description"></a><span data-ttu-id="1c208-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1c208-125">Description</span></span>

<span data-ttu-id="1c208-126">В следующем примере показан успешный ответ на запрос SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="1c208-126">The following example shows a successful response to the SyncFolderHierarchy request.</span></span> <span data-ttu-id="1c208-127">В этом примере выполняется синхронизация новой папки.</span><span class="sxs-lookup"><span data-stu-id="1c208-127">In this example, a new folder has been synchronized.</span></span>
  
### <a name="code"></a><span data-ttu-id="1c208-128">Код</span><span class="sxs-lookup"><span data-stu-id="1c208-128">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="1c208-129">Comments</span><span class="sxs-lookup"><span data-stu-id="1c208-129">Comments</span></span>

<span data-ttu-id="1c208-130">Данные элемента [синкстате](syncstate-ex15websvcsotherref.md) с кодировкой base64 и идентификатора папки были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="1c208-130">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the folder identifier data have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="1c208-131">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="1c208-131">Successful response elements</span></span>

<span data-ttu-id="1c208-132">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1c208-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="1c208-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="1c208-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1c208-134">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="1c208-134">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="1c208-135">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1c208-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1c208-136">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="1c208-136">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="1c208-137">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="1c208-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1c208-138">синкстате</span><span class="sxs-lookup"><span data-stu-id="1c208-138">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="1c208-139">инклудесластфолдеринранже</span><span class="sxs-lookup"><span data-stu-id="1c208-139">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
- [<span data-ttu-id="1c208-140">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="1c208-140">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
    
- [<span data-ttu-id="1c208-141">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="1c208-141">Create (FolderSync)</span></span>](create-foldersync.md)
    
- [<span data-ttu-id="1c208-142">Folder</span><span class="sxs-lookup"><span data-stu-id="1c208-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="1c208-143">FolderId</span><span class="sxs-lookup"><span data-stu-id="1c208-143">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="1c208-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="1c208-144">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="1c208-145">фолдеркласс</span><span class="sxs-lookup"><span data-stu-id="1c208-145">FolderClass</span></span>](folderclass.md)
    
- [<span data-ttu-id="1c208-146">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="1c208-146">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="1c208-147">тоталкаунт</span><span class="sxs-lookup"><span data-stu-id="1c208-147">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="1c208-148">чилдфолдеркаунт</span><span class="sxs-lookup"><span data-stu-id="1c208-148">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="1c208-149">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="1c208-149">UnreadCount</span></span>](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a><span data-ttu-id="1c208-150">Ответ об ошибке SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="1c208-150">SyncFolderHierarchy error response</span></span>

### <a name="description"></a><span data-ttu-id="1c208-151">Описание</span><span class="sxs-lookup"><span data-stu-id="1c208-151">Description</span></span>

<span data-ttu-id="1c208-152">В следующем примере показан ответ об ошибке для запроса SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="1c208-152">The following example shows an error response to a SyncFolderHierarchy request.</span></span> <span data-ttu-id="1c208-153">Эта ошибка вызвана недопустимым Синкстате.</span><span class="sxs-lookup"><span data-stu-id="1c208-153">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="1c208-154">Код</span><span class="sxs-lookup"><span data-stu-id="1c208-154">Code</span></span>

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

### <a name="error-response-elements"></a><span data-ttu-id="1c208-155">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="1c208-155">Error response elements</span></span>

<span data-ttu-id="1c208-156">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1c208-156">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="1c208-157">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="1c208-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1c208-158">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="1c208-158">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="1c208-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1c208-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1c208-160">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="1c208-160">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="1c208-161">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="1c208-161">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1c208-162">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="1c208-162">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1c208-163">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="1c208-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="1c208-164">синкстате</span><span class="sxs-lookup"><span data-stu-id="1c208-164">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="1c208-165">инклудесластфолдеринранже</span><span class="sxs-lookup"><span data-stu-id="1c208-165">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
## <a name="see-also"></a><span data-ttu-id="1c208-166">См. также</span><span class="sxs-lookup"><span data-stu-id="1c208-166">See also</span></span>



- [<span data-ttu-id="1c208-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1c208-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

