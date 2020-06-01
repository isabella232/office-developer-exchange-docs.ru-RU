---
title: Операция CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: Операция CreateFolder создает папки, папки календарей, папки контактов, папки задач и папки поиска.
ms.openlocfilehash: 125a6d212e5eaf85ace71c048de809f3a05ba9b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457552"
---
# <a name="createfolder-operation"></a><span data-ttu-id="54e6a-103">Операция CreateFolder</span><span class="sxs-lookup"><span data-stu-id="54e6a-103">CreateFolder operation</span></span>

<span data-ttu-id="54e6a-104">Операция CreateFolder создает папки, папки календарей, папки контактов, папки задач и папки поиска.</span><span class="sxs-lookup"><span data-stu-id="54e6a-104">The CreateFolder operation creates folders, calendar folders, contacts folders, tasks folders, and search folders.</span></span>
  
## <a name="createfolder-request-example"></a><span data-ttu-id="54e6a-105">Пример запроса CreateFolder</span><span class="sxs-lookup"><span data-stu-id="54e6a-105">CreateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="54e6a-106">Описание</span><span class="sxs-lookup"><span data-stu-id="54e6a-106">Description</span></span>

<span data-ttu-id="54e6a-107">В приведенном ниже примере запроса CreateFolder показано, как сформировать запрос на создание двух папок в корне почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="54e6a-107">The following example of a CreateFolder request shows how to form a request to create two new folders in the mailbox root.</span></span>
  
### <a name="code"></a><span data-ttu-id="54e6a-108">Код</span><span class="sxs-lookup"><span data-stu-id="54e6a-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ParentFolderId>
        <t:DistinguishedFolderId Id="msgfolderroot"/>
      </ParentFolderId>
      <Folders>
        <t:Folder>
          <t:DisplayName>Folder1</t:DisplayName>
        </t:Folder>
        <t:Folder>
          <t:DisplayName>Folder2</t:DisplayName>
        </t:Folder>
      </Folders>
    </CreateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="54e6a-109">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="54e6a-109">Request elements</span></span>

<span data-ttu-id="54e6a-110">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="54e6a-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="54e6a-111">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="54e6a-111">CreateFolder</span></span>](createfolder.md)
    
- [<span data-ttu-id="54e6a-112">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="54e6a-112">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="54e6a-113">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="54e6a-113">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="54e6a-114">Folders</span><span class="sxs-lookup"><span data-stu-id="54e6a-114">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="54e6a-115">Folder</span><span class="sxs-lookup"><span data-stu-id="54e6a-115">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="54e6a-116">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="54e6a-116">DisplayName (string)</span></span>](displayname-string.md)
    
> [!NOTE]
> <span data-ttu-id="54e6a-117">Схема, описывающая эти элементы, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Майкрософт Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="54e6a-117">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="54e6a-118">Чтобы найти другие параметры сообщения Request операции CreateFolder, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="54e6a-118">To find other options for the request message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="54e6a-119">Начните с элемента [CreateFolder](createfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="54e6a-119">Start at the [CreateFolder](createfolder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="54e6a-120">Если вы создаете папку поиска с ограничением с помощью свойства **Calendar: организатора** , последующий вызов get Folder будет возвращать ограничение с помощью свойства **Message: from** .</span><span class="sxs-lookup"><span data-stu-id="54e6a-120">If you create a search folder with a restriction by using the **calendar:Organizer** property, a subsequent get folder call will return the restriction with the **message:from** property in its place.</span></span> <span data-ttu-id="54e6a-121">Эти два свойства сопоставляются с одним и тем же базовым свойством MAPI.</span><span class="sxs-lookup"><span data-stu-id="54e6a-121">These two properties map to the same underlying MAPI property.</span></span> 
  
<span data-ttu-id="54e6a-122">Операция CreateFolder поддерживает создание класса настраиваемой папки только при создании папки с помощью универсального элемента типа Folder и установки элемента **фолдеркласс** .</span><span class="sxs-lookup"><span data-stu-id="54e6a-122">The CreateFolder operation supports the creation of a custom folder class only when you create the folder by using a generic folder type element and set the **FolderClass** element.</span></span> 
  
## <a name="successful-createfolder-response-example"></a><span data-ttu-id="54e6a-123">Пример успешного ответа CreateFolder</span><span class="sxs-lookup"><span data-stu-id="54e6a-123">Successful CreateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="54e6a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="54e6a-124">Description</span></span>

<span data-ttu-id="54e6a-125">В следующем примере показан успешный ответ на запрос CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="54e6a-125">The following example shows a successful response to the CreateFolder request.</span></span> <span data-ttu-id="54e6a-126">В этом примере ответ возвращает идентификаторы новых папок.</span><span class="sxs-lookup"><span data-stu-id="54e6a-126">In this example, the response returns the identifiers of the new folders.</span></span>
  
> [!NOTE]
> <span data-ttu-id="54e6a-127">Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="54e6a-127">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="54e6a-128">Код</span><span class="sxs-lookup"><span data-stu-id="54e6a-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="54e6a-129">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="54e6a-129">Successful response elements</span></span>

<span data-ttu-id="54e6a-130">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="54e6a-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="54e6a-131">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="54e6a-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="54e6a-132">креатефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="54e6a-132">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="54e6a-133">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="54e6a-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="54e6a-134">креатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="54e6a-134">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="54e6a-135">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="54e6a-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="54e6a-136">Folders</span><span class="sxs-lookup"><span data-stu-id="54e6a-136">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="54e6a-137">Folder</span><span class="sxs-lookup"><span data-stu-id="54e6a-137">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="54e6a-138">FolderId</span><span class="sxs-lookup"><span data-stu-id="54e6a-138">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="54e6a-139">Чтобы найти другие параметры для ответного сообщения операции CreateFolder, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="54e6a-139">To find other options for the response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="54e6a-140">Начните с элемента [креатефолдерреспонсе](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="54e6a-140">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="createfolder-error-response"></a><span data-ttu-id="54e6a-141">Ответ об ошибке CreateFolder</span><span class="sxs-lookup"><span data-stu-id="54e6a-141">CreateFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="54e6a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="54e6a-142">Description</span></span>

<span data-ttu-id="54e6a-143">В следующем примере показан ответ об ошибке для запроса CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="54e6a-143">The following example shows an error response to a CreateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="54e6a-144">Код</span><span class="sxs-lookup"><span data-stu-id="54e6a-144">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A folder with the specified name already exists.</m:MessageText>
          <m:ResponseCode>ErrorFolderExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="54e6a-145">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="54e6a-145">Error response elements</span></span>

<span data-ttu-id="54e6a-146">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="54e6a-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="54e6a-147">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="54e6a-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="54e6a-148">креатефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="54e6a-148">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="54e6a-149">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="54e6a-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="54e6a-150">креатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="54e6a-150">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="54e6a-151">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="54e6a-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="54e6a-152">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="54e6a-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="54e6a-153">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="54e6a-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="54e6a-154">Folders</span><span class="sxs-lookup"><span data-stu-id="54e6a-154">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="54e6a-155">Чтобы найти другие параметры сообщения об ошибке при выполнении операции CreateFolder, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="54e6a-155">To find other options for the error response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="54e6a-156">Начните с элемента [креатефолдерреспонсе](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="54e6a-156">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="54e6a-157">См. также</span><span class="sxs-lookup"><span data-stu-id="54e6a-157">See also</span></span>



[<span data-ttu-id="54e6a-158">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="54e6a-158">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="54e6a-159">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="54e6a-159">FindFolder operation</span></span>](findfolder-operation.md)
  
 <span data-ttu-id="54e6a-160">**креатефолдертипе**</span><span class="sxs-lookup"><span data-stu-id="54e6a-160">**CreateFolderType**</span></span>


- [<span data-ttu-id="54e6a-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="54e6a-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="54e6a-162">Создание папок (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="54e6a-162">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

