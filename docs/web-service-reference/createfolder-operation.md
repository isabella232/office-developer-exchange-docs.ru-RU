---
title: CreateFolder Operation
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
description: Операция CreateFolder создает папки, папкам календаря, контакты папки, папки задач и поиска папок.
ms.openlocfilehash: 97156d4a3747cacbdcf9563d21d93a0aa44c3358
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761874"
---
# <a name="createfolder-operation"></a><span data-ttu-id="7f657-103">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="7f657-103">CreateFolder operation</span></span>

<span data-ttu-id="7f657-104">Операция CreateFolder создает папки, папкам календаря, контакты папки, папки задач и поиска папок.</span><span class="sxs-lookup"><span data-stu-id="7f657-104">The CreateFolder operation creates folders, calendar folders, contacts folders, tasks folders, and search folders.</span></span>
  
## <a name="createfolder-request-example"></a><span data-ttu-id="7f657-105">Пример запроса CreateFolder</span><span class="sxs-lookup"><span data-stu-id="7f657-105">CreateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="7f657-106">Описание</span><span class="sxs-lookup"><span data-stu-id="7f657-106">Description</span></span>

<span data-ttu-id="7f657-107">В следующем примере запрос CreateFolder показано, как для формирования запроса для создания двух новых папок в корне почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7f657-107">The following example of a CreateFolder request shows how to form a request to create two new folders in the mailbox root.</span></span>
  
### <a name="code"></a><span data-ttu-id="7f657-108">Программа</span><span class="sxs-lookup"><span data-stu-id="7f657-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="request-elements"></a><span data-ttu-id="7f657-109">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="7f657-109">Request elements</span></span>

<span data-ttu-id="7f657-110">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7f657-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7f657-111">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="7f657-111">CreateFolder</span></span>](createfolder.md)
    
- [<span data-ttu-id="7f657-112">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="7f657-112">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="7f657-113">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="7f657-113">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="7f657-114">Папки</span><span class="sxs-lookup"><span data-stu-id="7f657-114">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7f657-115">Folder</span><span class="sxs-lookup"><span data-stu-id="7f657-115">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="7f657-116">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="7f657-116">DisplayName (string)</span></span>](displayname-string.md)
    
> [!NOTE]
> <span data-ttu-id="7f657-117">Схема, описывающая эти элементы находится в виртуальном каталоге EWS компьютера, на котором работает MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7f657-117">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="7f657-118">Чтобы найти другие параметры для запроса операции CreateFolder, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="7f657-118">To find other options for the request message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7f657-119">Начать с [CreateFolder](createfolder.md) элемента.</span><span class="sxs-lookup"><span data-stu-id="7f657-119">Start at the [CreateFolder](createfolder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7f657-120">При создании папки поиска с ограничением с помощью свойства **Календаря: Организатор** звонка папки последующие get возвращает ограничений с **сообщения: из** свойство вместо него.</span><span class="sxs-lookup"><span data-stu-id="7f657-120">If you create a search folder with a restriction by using the **calendar:Organizer** property, a subsequent get folder call will return the restriction with the **message:from** property in its place.</span></span> <span data-ttu-id="7f657-121">Эти два свойства сопоставить же базового свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="7f657-121">These two properties map to the same underlying MAPI property.</span></span> 
  
<span data-ttu-id="7f657-122">Операция CreateFolder поддерживает создание класса настраиваемого папки только в том случае, если создать папку с помощью элемента типа общей папки, а значение элемента **FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="7f657-122">The CreateFolder operation supports the creation of a custom folder class only when you create the folder by using a generic folder type element and set the **FolderClass** element.</span></span> 
  
## <a name="successful-createfolder-response-example"></a><span data-ttu-id="7f657-123">Пример успешного ответа CreateFolder</span><span class="sxs-lookup"><span data-stu-id="7f657-123">Successful CreateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="7f657-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7f657-124">Description</span></span>

<span data-ttu-id="7f657-125">В следующем примере показано успешного ответа на запрос CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="7f657-125">The following example shows a successful response to the CreateFolder request.</span></span> <span data-ttu-id="7f657-126">В этом примере возвращается в ответе идентификаторы новые папки.</span><span class="sxs-lookup"><span data-stu-id="7f657-126">In this example, the response returns the identifiers of the new folders.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7f657-127">Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="7f657-127">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7f657-128">Программа</span><span class="sxs-lookup"><span data-stu-id="7f657-128">Code</span></span>

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
    <CreateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="7f657-129">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="7f657-129">Successful response elements</span></span>

<span data-ttu-id="7f657-130">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7f657-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7f657-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7f657-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7f657-132">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="7f657-132">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="7f657-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7f657-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7f657-134">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7f657-134">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="7f657-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f657-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7f657-136">Папки</span><span class="sxs-lookup"><span data-stu-id="7f657-136">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7f657-137">Folder</span><span class="sxs-lookup"><span data-stu-id="7f657-137">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="7f657-138">FolderId</span><span class="sxs-lookup"><span data-stu-id="7f657-138">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="7f657-139">Чтобы найти другие параметры в сообщении ответа операции CreateFolder, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="7f657-139">To find other options for the response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7f657-140">Запустите в элементе [CreateFolderResponse](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="7f657-140">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="createfolder-error-response"></a><span data-ttu-id="7f657-141">Отклик CreateFolder</span><span class="sxs-lookup"><span data-stu-id="7f657-141">CreateFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="7f657-142">Описание</span><span class="sxs-lookup"><span data-stu-id="7f657-142">Description</span></span>

<span data-ttu-id="7f657-143">В следующем примере показано возврату ошибки CreateFolder запрос.</span><span class="sxs-lookup"><span data-stu-id="7f657-143">The following example shows an error response to a CreateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="7f657-144">Программа</span><span class="sxs-lookup"><span data-stu-id="7f657-144">Code</span></span>

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
    <CreateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="7f657-145">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="7f657-145">Error response elements</span></span>

<span data-ttu-id="7f657-146">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7f657-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="7f657-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7f657-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7f657-148">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="7f657-148">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="7f657-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7f657-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7f657-150">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7f657-150">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="7f657-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="7f657-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7f657-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f657-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7f657-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7f657-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="7f657-154">Папки</span><span class="sxs-lookup"><span data-stu-id="7f657-154">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="7f657-155">Чтобы найти другие параметры в сообщении об ошибке ответа операции CreateFolder, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="7f657-155">To find other options for the error response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7f657-156">Запустите в элементе [CreateFolderResponse](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="7f657-156">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7f657-157">См. также</span><span class="sxs-lookup"><span data-stu-id="7f657-157">See also</span></span>



[<span data-ttu-id="7f657-158">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="7f657-158">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="7f657-159">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="7f657-159">FindFolder operation</span></span>](findfolder-operation.md)
  
 <span data-ttu-id="7f657-160">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="7f657-160">**CreateFolderType**</span></span>


- [<span data-ttu-id="7f657-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7f657-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7f657-162">Создание папки (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="7f657-162">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

