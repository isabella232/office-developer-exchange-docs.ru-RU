---
title: Операция UpdateFolder
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
description: 'Операция операцию UpdateFolder используется для изменения свойств существующего элемента в хранилище Exchange. Каждая операция операцию UpdateFolder состоит из следующих элементов:'
ms.openlocfilehash: b33937bb09f0dcbe3d3ed61bbf5233423f320d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840324"
---
# <a name="updatefolder-operation"></a><span data-ttu-id="fbf51-104">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="fbf51-104">UpdateFolder operation</span></span>

<span data-ttu-id="fbf51-105">Операция операцию UpdateFolder используется для изменения свойств существующего элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fbf51-105">The UpdateFolder operation is used to modify properties of an existing item in the Exchange store.</span></span> <span data-ttu-id="fbf51-106">Каждая операция операцию UpdateFolder состоит из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="fbf51-106">Each UpdateFolder operation consists of the following:</span></span>
  
- <span data-ttu-id="fbf51-107">Элемент [FolderId](folderid.md) , указывающий папку, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="fbf51-107">A [FolderId](folderid.md) element that specifies a folder to update.</span></span> 
    
- <span data-ttu-id="fbf51-108">Внутренний путь к элементу в папке, как указано в фигуре папки, в которой задаются данные для обновления.</span><span class="sxs-lookup"><span data-stu-id="fbf51-108">An internal path of an element in the folder, as specified by the folder shape, which specifies the data to update.</span></span>
    
- <span data-ttu-id="fbf51-109">Папка, содержащая новое значение обновленного поля, если обновление не является удалением.</span><span class="sxs-lookup"><span data-stu-id="fbf51-109">A folder that contains the new value of the updated field, if the update is not a deletion.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="fbf51-110">Примечания</span><span class="sxs-lookup"><span data-stu-id="fbf51-110">Remarks</span></span>

<span data-ttu-id="fbf51-111">Для элемента можно выполнить три основных действия обновления.</span><span class="sxs-lookup"><span data-stu-id="fbf51-111">Three basic update actions can be performed on an item.</span></span> <span data-ttu-id="fbf51-112">Эти действия перечислены в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="fbf51-112">These actions are listed in the following table.</span></span>
  
|<span data-ttu-id="fbf51-113">**Действие**</span><span class="sxs-lookup"><span data-stu-id="fbf51-113">**Action**</span></span>|<span data-ttu-id="fbf51-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fbf51-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fbf51-115">Error</span><span class="sxs-lookup"><span data-stu-id="fbf51-115">Append</span></span>  <br/> |<span data-ttu-id="fbf51-116">Действие Append добавляет данные к существующему свойству.</span><span class="sxs-lookup"><span data-stu-id="fbf51-116">The append action adds data to an existing property.</span></span> <span data-ttu-id="fbf51-117">Они сохраняют текущие данные.</span><span class="sxs-lookup"><span data-stu-id="fbf51-117">It preserves the data that is currently there.</span></span> <span data-ttu-id="fbf51-118">Append не применимо ко всем свойствам.</span><span class="sxs-lookup"><span data-stu-id="fbf51-118">Append is not applicable to all properties.</span></span>  <br/> |
|<span data-ttu-id="fbf51-119">Set</span><span class="sxs-lookup"><span data-stu-id="fbf51-119">Set</span></span>  <br/> |<span data-ttu-id="fbf51-120">Действие Set замещает данные для свойства, если оно содержит данные, или создает свойство и задает его значение, если оно не существует.</span><span class="sxs-lookup"><span data-stu-id="fbf51-120">The set action replaces data for a property if it contains data, or creates the property and sets its value if it does not exist.</span></span> <span data-ttu-id="fbf51-121">Действие Set применяется только к записываемым свойствам.</span><span class="sxs-lookup"><span data-stu-id="fbf51-121">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="fbf51-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="fbf51-122">Delete</span></span>  <br/> |<span data-ttu-id="fbf51-123">Действие DELETE удаляет свойство из папки.</span><span class="sxs-lookup"><span data-stu-id="fbf51-123">The delete action removes a property from a folder.</span></span> <span data-ttu-id="fbf51-124">Это отличается от присвоения пустого значения.</span><span class="sxs-lookup"><span data-stu-id="fbf51-124">This is different than setting it to an empty value.</span></span> <span data-ttu-id="fbf51-125">По завершении свойство для папки не существует.</span><span class="sxs-lookup"><span data-stu-id="fbf51-125">When complete, the property does not exist for the folder.</span></span> <span data-ttu-id="fbf51-126">DELETE применяется только к записываемым свойствам.</span><span class="sxs-lookup"><span data-stu-id="fbf51-126">Delete is only applicable to writable properties.</span></span>  <br/> |
   
## <a name="updatefolder-request-example"></a><span data-ttu-id="fbf51-127">Пример запроса операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="fbf51-127">UpdateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="fbf51-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fbf51-128">Description</span></span>

<span data-ttu-id="fbf51-129">В приведенном ниже примере запроса операцию UpdateFolder показано, как обновить отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="fbf51-129">The following example of an UpdateFolder request shows how to update a folder display name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fbf51-130">Код</span><span class="sxs-lookup"><span data-stu-id="fbf51-130">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="fbf51-131">Comments</span><span class="sxs-lookup"><span data-stu-id="fbf51-131">Comments</span></span>

<span data-ttu-id="fbf51-132">В этом примере показано изменение отображаемого имени папки на Невфолдернаме.</span><span class="sxs-lookup"><span data-stu-id="fbf51-132">This example changes the display name of the folder to NewFolderName.</span></span>
  
> [!NOTE]
> <span data-ttu-id="fbf51-133">Значения атрибутов **ID** и **чанжекэй** элемента [FolderId](folderid.md) сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fbf51-133">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="fbf51-134">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="fbf51-134">Request elements</span></span>

<span data-ttu-id="fbf51-135">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fbf51-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="fbf51-136">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="fbf51-136">UpdateFolder</span></span>](updatefolder.md)
    
- [<span data-ttu-id="fbf51-137">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="fbf51-137">FolderChanges</span></span>](folderchanges.md)
    
- [<span data-ttu-id="fbf51-138">FolderChange</span><span class="sxs-lookup"><span data-stu-id="fbf51-138">FolderChange</span></span>](folderchange.md)
    
- [<span data-ttu-id="fbf51-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="fbf51-139">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="fbf51-140">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="fbf51-140">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="fbf51-141">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="fbf51-141">SetFolderField</span></span>](setfolderfield.md)
    
- [<span data-ttu-id="fbf51-142">фиелдури</span><span class="sxs-lookup"><span data-stu-id="fbf51-142">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="fbf51-143">Folder</span><span class="sxs-lookup"><span data-stu-id="fbf51-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="fbf51-144">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="fbf51-144">DisplayName (string)</span></span>](displayname-string.md)
    
<span data-ttu-id="fbf51-145">В схеме представлены дополнительные элементы, которые можно использовать для формирования запроса операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="fbf51-145">See the schema for additional elements that you can use to form an UpdateFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="fbf51-146">Расположение схемы по умолчанию находится в виртуальном каталоге EWS на компьютере, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fbf51-146">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="updatefolder-response-example"></a><span data-ttu-id="fbf51-147">Пример отклика операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="fbf51-147">UpdateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="fbf51-148">Описание</span><span class="sxs-lookup"><span data-stu-id="fbf51-148">Description</span></span>

<span data-ttu-id="fbf51-149">В следующем примере показан успешный ответ на запрос операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="fbf51-149">The following example shows a successful response to the UpdateFolder request.</span></span> <span data-ttu-id="fbf51-150">В этом примере возвращается новый ключ изменения, который отражает обновленное состояние папки.</span><span class="sxs-lookup"><span data-stu-id="fbf51-150">In this example, the new change key is returned to reflect the updated status of the folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="fbf51-151">Код</span><span class="sxs-lookup"><span data-stu-id="fbf51-151">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="fbf51-152">Comments</span><span class="sxs-lookup"><span data-stu-id="fbf51-152">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="fbf51-153">Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="fbf51-153">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="fbf51-154">Идентификатор папки, возвращаемой в ответе, представляет обновленную папку.</span><span class="sxs-lookup"><span data-stu-id="fbf51-154">The folder ID that is returned in the response represents the updated folder.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="fbf51-155">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="fbf51-155">Successful response elements</span></span>

<span data-ttu-id="fbf51-156">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fbf51-156">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="fbf51-157">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fbf51-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fbf51-158">упдатефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="fbf51-158">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="fbf51-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fbf51-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fbf51-160">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fbf51-160">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="fbf51-161">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fbf51-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fbf51-162">Folders</span><span class="sxs-lookup"><span data-stu-id="fbf51-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="fbf51-163">Folder</span><span class="sxs-lookup"><span data-stu-id="fbf51-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="fbf51-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="fbf51-164">FolderId</span></span>](folderid.md)
    
## <a name="updatefolder-error-response-example"></a><span data-ttu-id="fbf51-165">Пример ответа на сообщение об ошибке операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="fbf51-165">UpdateFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="fbf51-166">Описание</span><span class="sxs-lookup"><span data-stu-id="fbf51-166">Description</span></span>

<span data-ttu-id="fbf51-167">В следующем примере показан ответ об ошибке для запроса операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="fbf51-167">The following example shows an error response to an UpdateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="fbf51-168">Код</span><span class="sxs-lookup"><span data-stu-id="fbf51-168">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="fbf51-169">Comments</span><span class="sxs-lookup"><span data-stu-id="fbf51-169">Comments</span></span>

<span data-ttu-id="fbf51-170">В этом примере показан ответ об ошибке, вызванный недопустимым атрибутом **чанжекэй** в запросе.</span><span class="sxs-lookup"><span data-stu-id="fbf51-170">This example shows an error response that is caused by an invalid **ChangeKey** attribute in the request.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="fbf51-171">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="fbf51-171">Error response elements</span></span>

<span data-ttu-id="fbf51-172">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fbf51-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="fbf51-173">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fbf51-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fbf51-174">упдатефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="fbf51-174">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="fbf51-175">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fbf51-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fbf51-176">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fbf51-176">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="fbf51-177">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="fbf51-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="fbf51-178">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fbf51-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fbf51-179">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="fbf51-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="fbf51-180">Folders</span><span class="sxs-lookup"><span data-stu-id="fbf51-180">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="fbf51-181">См. также</span><span class="sxs-lookup"><span data-stu-id="fbf51-181">See also</span></span>



- [<span data-ttu-id="fbf51-182">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fbf51-182">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

