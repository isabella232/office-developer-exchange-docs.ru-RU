---
title: Операцию UpdateFolder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: 'Операция UpdateFolder используется для изменения свойств существующего элемента в хранилище Exchange. Каждую операцию UpdateFolder состоит из следующих компонентов:'
ms.openlocfilehash: b33937bb09f0dcbe3d3ed61bbf5233423f320d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840324"
---
# <a name="updatefolder-operation"></a><span data-ttu-id="24e9b-104">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="24e9b-104">UpdateFolder operation</span></span>

<span data-ttu-id="24e9b-105">Операция UpdateFolder используется для изменения свойств существующего элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="24e9b-105">The UpdateFolder operation is used to modify properties of an existing item in the Exchange store.</span></span> <span data-ttu-id="24e9b-106">Каждую операцию UpdateFolder состоит из следующих компонентов:</span><span class="sxs-lookup"><span data-stu-id="24e9b-106">Each UpdateFolder operation consists of the following:</span></span>
  
- <span data-ttu-id="24e9b-107">Элемент [FolderId](folderid.md) , путь к папке для обновления.</span><span class="sxs-lookup"><span data-stu-id="24e9b-107">A [FolderId](folderid.md) element that specifies a folder to update.</span></span> 
    
- <span data-ttu-id="24e9b-108">Внутренний путь элемента в папке, в соответствии с фигуры папки, который определяет данные для обновления.</span><span class="sxs-lookup"><span data-stu-id="24e9b-108">An internal path of an element in the folder, as specified by the folder shape, which specifies the data to update.</span></span>
    
- <span data-ttu-id="24e9b-109">Папка, содержащая новое значение обновленные поля, если обновление не удаления.</span><span class="sxs-lookup"><span data-stu-id="24e9b-109">A folder that contains the new value of the updated field, if the update is not a deletion.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="24e9b-110">Замечания</span><span class="sxs-lookup"><span data-stu-id="24e9b-110">Remarks</span></span>

<span data-ttu-id="24e9b-111">Три основные обновления действия над элементом.</span><span class="sxs-lookup"><span data-stu-id="24e9b-111">Three basic update actions can be performed on an item.</span></span> <span data-ttu-id="24e9b-112">В следующей таблице перечислены эти действия.</span><span class="sxs-lookup"><span data-stu-id="24e9b-112">These actions are listed in the following table.</span></span>
  
|<span data-ttu-id="24e9b-113">**Действие**</span><span class="sxs-lookup"><span data-stu-id="24e9b-113">**Action**</span></span>|<span data-ttu-id="24e9b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24e9b-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24e9b-115">Добавление</span><span class="sxs-lookup"><span data-stu-id="24e9b-115">Append</span></span>  <br/> |<span data-ttu-id="24e9b-116">Добавление действия добавляет данные существующего свойства.</span><span class="sxs-lookup"><span data-stu-id="24e9b-116">The append action adds data to an existing property.</span></span> <span data-ttu-id="24e9b-117">Он сохраняет данные.</span><span class="sxs-lookup"><span data-stu-id="24e9b-117">It preserves the data that is currently there.</span></span> <span data-ttu-id="24e9b-118">Добавьте не применяется ко всем свойствам.</span><span class="sxs-lookup"><span data-stu-id="24e9b-118">Append is not applicable to all properties.</span></span>  <br/> |
|<span data-ttu-id="24e9b-119">Set</span><span class="sxs-lookup"><span data-stu-id="24e9b-119">Set</span></span>  <br/> |<span data-ttu-id="24e9b-120">Набор действий заменяет данных для свойства, если он содержит данные, или создает свойство и задает его значение, если не существует.</span><span class="sxs-lookup"><span data-stu-id="24e9b-120">The set action replaces data for a property if it contains data, or creates the property and sets its value if it does not exist.</span></span> <span data-ttu-id="24e9b-121">Набор действий применима только для записи свойств.</span><span class="sxs-lookup"><span data-stu-id="24e9b-121">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="24e9b-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="24e9b-122">Delete</span></span>  <br/> |<span data-ttu-id="24e9b-123">Удаление удаляет свойство из папки.</span><span class="sxs-lookup"><span data-stu-id="24e9b-123">The delete action removes a property from a folder.</span></span> <span data-ttu-id="24e9b-124">Это отличается от параметра пустое значение.</span><span class="sxs-lookup"><span data-stu-id="24e9b-124">This is different than setting it to an empty value.</span></span> <span data-ttu-id="24e9b-125">Закончив настройку, свойство не существует для папки.</span><span class="sxs-lookup"><span data-stu-id="24e9b-125">When complete, the property does not exist for the folder.</span></span> <span data-ttu-id="24e9b-126">Удалить применима только для записи свойств.</span><span class="sxs-lookup"><span data-stu-id="24e9b-126">Delete is only applicable to writable properties.</span></span>  <br/> |
   
## <a name="updatefolder-request-example"></a><span data-ttu-id="24e9b-127">Пример запроса UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="24e9b-127">UpdateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="24e9b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="24e9b-128">Description</span></span>

<span data-ttu-id="24e9b-129">В следующем примере запрос UpdateFolder показано, как обновить отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="24e9b-129">The following example of an UpdateFolder request shows how to update a folder display name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="24e9b-130">Программа</span><span class="sxs-lookup"><span data-stu-id="24e9b-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AScA" ChangeKey="GO3u/"/>
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName"/>
              <t:Folder>
                <t:DisplayName>NewFolderName</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </FolderChanges>
    </UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="24e9b-131">Комментарии</span><span class="sxs-lookup"><span data-stu-id="24e9b-131">Comments</span></span>

<span data-ttu-id="24e9b-132">В этом примере изменяется отображаемое имя папки Новое_имя_папки.</span><span class="sxs-lookup"><span data-stu-id="24e9b-132">This example changes the display name of the folder to NewFolderName.</span></span>
  
> [!NOTE]
> <span data-ttu-id="24e9b-133">Значения **Id** и **ChangeKey** атрибутов элемента [FolderId](folderid.md) URL были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="24e9b-133">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="24e9b-134">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="24e9b-134">Request elements</span></span>

<span data-ttu-id="24e9b-135">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="24e9b-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="24e9b-136">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="24e9b-136">UpdateFolder</span></span>](updatefolder.md)
    
- [<span data-ttu-id="24e9b-137">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="24e9b-137">FolderChanges</span></span>](folderchanges.md)
    
- [<span data-ttu-id="24e9b-138">FolderChange</span><span class="sxs-lookup"><span data-stu-id="24e9b-138">FolderChange</span></span>](folderchange.md)
    
- [<span data-ttu-id="24e9b-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="24e9b-139">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="24e9b-140">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="24e9b-140">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="24e9b-141">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="24e9b-141">SetFolderField</span></span>](setfolderfield.md)
    
- [<span data-ttu-id="24e9b-142">FieldURI</span><span class="sxs-lookup"><span data-stu-id="24e9b-142">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="24e9b-143">Folder</span><span class="sxs-lookup"><span data-stu-id="24e9b-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="24e9b-144">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="24e9b-144">DisplayName (string)</span></span>](displayname-string.md)
    
<span data-ttu-id="24e9b-145">В разделе Схема дополнительных элементов, которые можно использовать для формирования запроса UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="24e9b-145">See the schema for additional elements that you can use to form an UpdateFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="24e9b-146">Расположение по умолчанию схемы находится в виртуальном каталоге EWS на компьютере, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="24e9b-146">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="updatefolder-response-example"></a><span data-ttu-id="24e9b-147">Пример ответа UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="24e9b-147">UpdateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="24e9b-148">Описание</span><span class="sxs-lookup"><span data-stu-id="24e9b-148">Description</span></span>

<span data-ttu-id="24e9b-149">В следующем примере показано успешного ответа на запрос UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="24e9b-149">The following example shows a successful response to the UpdateFolder request.</span></span> <span data-ttu-id="24e9b-150">В этом примере новый ключ изменения возвращается в соответствии с обновленное состояние папки.</span><span class="sxs-lookup"><span data-stu-id="24e9b-150">In this example, the new change key is returned to reflect the updated status of the folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="24e9b-151">Программа</span><span class="sxs-lookup"><span data-stu-id="24e9b-151">Code</span></span>

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
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFVz" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="24e9b-152">Комментарии</span><span class="sxs-lookup"><span data-stu-id="24e9b-152">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="24e9b-153">Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="24e9b-153">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="24e9b-154">Идентификатор папки, возвращаемого в ответе представляет обновленные папки.</span><span class="sxs-lookup"><span data-stu-id="24e9b-154">The folder ID that is returned in the response represents the updated folder.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="24e9b-155">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="24e9b-155">Successful response elements</span></span>

<span data-ttu-id="24e9b-156">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="24e9b-156">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="24e9b-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="24e9b-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="24e9b-158">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="24e9b-158">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="24e9b-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="24e9b-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="24e9b-160">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="24e9b-160">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="24e9b-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="24e9b-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="24e9b-162">Папки</span><span class="sxs-lookup"><span data-stu-id="24e9b-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="24e9b-163">Folder</span><span class="sxs-lookup"><span data-stu-id="24e9b-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="24e9b-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="24e9b-164">FolderId</span></span>](folderid.md)
    
## <a name="updatefolder-error-response-example"></a><span data-ttu-id="24e9b-165">Пример ответа об ошибке UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="24e9b-165">UpdateFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="24e9b-166">Описание</span><span class="sxs-lookup"><span data-stu-id="24e9b-166">Description</span></span>

<span data-ttu-id="24e9b-167">В следующем примере показано ошибочный ответ на запрос UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="24e9b-167">The following example shows an error response to an UpdateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="24e9b-168">Программа</span><span class="sxs-lookup"><span data-stu-id="24e9b-168">Code</span></span>

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
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="24e9b-169">Комментарии</span><span class="sxs-lookup"><span data-stu-id="24e9b-169">Comments</span></span>

<span data-ttu-id="24e9b-170">В этом примере показано возврату ошибки, возникающие при недопустимый атрибут **ChangeKey** в запросе.</span><span class="sxs-lookup"><span data-stu-id="24e9b-170">This example shows an error response that is caused by an invalid **ChangeKey** attribute in the request.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="24e9b-171">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="24e9b-171">Error response elements</span></span>

<span data-ttu-id="24e9b-172">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="24e9b-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="24e9b-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="24e9b-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="24e9b-174">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="24e9b-174">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="24e9b-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="24e9b-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="24e9b-176">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="24e9b-176">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="24e9b-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="24e9b-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="24e9b-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="24e9b-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="24e9b-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="24e9b-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="24e9b-180">Папки</span><span class="sxs-lookup"><span data-stu-id="24e9b-180">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="24e9b-181">См. также</span><span class="sxs-lookup"><span data-stu-id="24e9b-181">See also</span></span>



- [<span data-ttu-id="24e9b-182">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="24e9b-182">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

