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
ms.openlocfilehash: fb894d9f42358b67f81e9fe8ae41ba61e6f46460
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467363"
---
# <a name="updatefolder-operation"></a><span data-ttu-id="6c8c6-104">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="6c8c6-104">UpdateFolder operation</span></span>

<span data-ttu-id="6c8c6-105">Операция операцию UpdateFolder используется для изменения свойств существующего элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-105">The UpdateFolder operation is used to modify properties of an existing item in the Exchange store.</span></span> <span data-ttu-id="6c8c6-106">Каждая операция операцию UpdateFolder состоит из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="6c8c6-106">Each UpdateFolder operation consists of the following:</span></span>
  
- <span data-ttu-id="6c8c6-107">Элемент [FolderId](folderid.md) , указывающий папку, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-107">A [FolderId](folderid.md) element that specifies a folder to update.</span></span> 
    
- <span data-ttu-id="6c8c6-108">Внутренний путь к элементу в папке, как указано в фигуре папки, в которой задаются данные для обновления.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-108">An internal path of an element in the folder, as specified by the folder shape, which specifies the data to update.</span></span>
    
- <span data-ttu-id="6c8c6-109">Папка, содержащая новое значение обновленного поля, если обновление не является удалением.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-109">A folder that contains the new value of the updated field, if the update is not a deletion.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6c8c6-110">Примечания</span><span class="sxs-lookup"><span data-stu-id="6c8c6-110">Remarks</span></span>

<span data-ttu-id="6c8c6-111">Для элемента можно выполнить три основных действия обновления.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-111">Three basic update actions can be performed on an item.</span></span> <span data-ttu-id="6c8c6-112">Эти действия перечислены в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-112">These actions are listed in the following table.</span></span>
  
|<span data-ttu-id="6c8c6-113">**Действие**</span><span class="sxs-lookup"><span data-stu-id="6c8c6-113">**Action**</span></span>|<span data-ttu-id="6c8c6-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6c8c6-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6c8c6-115">Error</span><span class="sxs-lookup"><span data-stu-id="6c8c6-115">Append</span></span>  <br/> |<span data-ttu-id="6c8c6-116">Действие Append добавляет данные к существующему свойству.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-116">The append action adds data to an existing property.</span></span> <span data-ttu-id="6c8c6-117">Они сохраняют текущие данные.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-117">It preserves the data that is currently there.</span></span> <span data-ttu-id="6c8c6-118">Append не применимо ко всем свойствам.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-118">Append is not applicable to all properties.</span></span>  <br/> |
|<span data-ttu-id="6c8c6-119">Set</span><span class="sxs-lookup"><span data-stu-id="6c8c6-119">Set</span></span>  <br/> |<span data-ttu-id="6c8c6-120">Действие Set замещает данные для свойства, если оно содержит данные, или создает свойство и задает его значение, если оно не существует.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-120">The set action replaces data for a property if it contains data, or creates the property and sets its value if it does not exist.</span></span> <span data-ttu-id="6c8c6-121">Действие Set применяется только к записываемым свойствам.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-121">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="6c8c6-122">Удалить</span><span class="sxs-lookup"><span data-stu-id="6c8c6-122">Delete</span></span>  <br/> |<span data-ttu-id="6c8c6-123">Действие DELETE удаляет свойство из папки.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-123">The delete action removes a property from a folder.</span></span> <span data-ttu-id="6c8c6-124">Это отличается от присвоения пустого значения.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-124">This is different than setting it to an empty value.</span></span> <span data-ttu-id="6c8c6-125">По завершении свойство для папки не существует.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-125">When complete, the property does not exist for the folder.</span></span> <span data-ttu-id="6c8c6-126">DELETE применяется только к записываемым свойствам.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-126">Delete is only applicable to writable properties.</span></span>  <br/> |
   
## <a name="updatefolder-request-example"></a><span data-ttu-id="6c8c6-127">Пример запроса операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="6c8c6-127">UpdateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="6c8c6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6c8c6-128">Description</span></span>

<span data-ttu-id="6c8c6-129">В приведенном ниже примере запроса операцию UpdateFolder показано, как обновить отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-129">The following example of an UpdateFolder request shows how to update a folder display name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6c8c6-130">Код</span><span class="sxs-lookup"><span data-stu-id="6c8c6-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="6c8c6-131">Комментарии</span><span class="sxs-lookup"><span data-stu-id="6c8c6-131">Comments</span></span>

<span data-ttu-id="6c8c6-132">В этом примере показано изменение отображаемого имени папки на Невфолдернаме.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-132">This example changes the display name of the folder to NewFolderName.</span></span>
  
> [!NOTE]
> <span data-ttu-id="6c8c6-133">Значения атрибутов **ID** и **чанжекэй** элемента [FolderId](folderid.md) сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-133">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="6c8c6-134">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="6c8c6-134">Request elements</span></span>

<span data-ttu-id="6c8c6-135">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6c8c6-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="6c8c6-136">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="6c8c6-136">UpdateFolder</span></span>](updatefolder.md)
    
- [<span data-ttu-id="6c8c6-137">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="6c8c6-137">FolderChanges</span></span>](folderchanges.md)
    
- [<span data-ttu-id="6c8c6-138">FolderChange</span><span class="sxs-lookup"><span data-stu-id="6c8c6-138">FolderChange</span></span>](folderchange.md)
    
- [<span data-ttu-id="6c8c6-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="6c8c6-139">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="6c8c6-140">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="6c8c6-140">Updates (Folder)</span></span>](updates-folder.md)
    
- [<span data-ttu-id="6c8c6-141">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="6c8c6-141">SetFolderField</span></span>](setfolderfield.md)
    
- [<span data-ttu-id="6c8c6-142">фиелдури</span><span class="sxs-lookup"><span data-stu-id="6c8c6-142">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="6c8c6-143">Folder</span><span class="sxs-lookup"><span data-stu-id="6c8c6-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="6c8c6-144">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="6c8c6-144">DisplayName (string)</span></span>](displayname-string.md)
    
<span data-ttu-id="6c8c6-145">В схеме представлены дополнительные элементы, которые можно использовать для формирования запроса операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-145">See the schema for additional elements that you can use to form an UpdateFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="6c8c6-146">Расположение схемы по умолчанию находится в виртуальном каталоге EWS на компьютере, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-146">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="updatefolder-response-example"></a><span data-ttu-id="6c8c6-147">Пример отклика операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="6c8c6-147">UpdateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="6c8c6-148">Описание</span><span class="sxs-lookup"><span data-stu-id="6c8c6-148">Description</span></span>

<span data-ttu-id="6c8c6-149">В следующем примере показан успешный ответ на запрос операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-149">The following example shows a successful response to the UpdateFolder request.</span></span> <span data-ttu-id="6c8c6-150">В этом примере возвращается новый ключ изменения, который отражает обновленное состояние папки.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-150">In this example, the new change key is returned to reflect the updated status of the folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="6c8c6-151">Код</span><span class="sxs-lookup"><span data-stu-id="6c8c6-151">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="6c8c6-152">Комментарии</span><span class="sxs-lookup"><span data-stu-id="6c8c6-152">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="6c8c6-153">Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-153">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="6c8c6-154">Идентификатор папки, возвращаемой в ответе, представляет обновленную папку.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-154">The folder ID that is returned in the response represents the updated folder.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="6c8c6-155">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="6c8c6-155">Successful response elements</span></span>

<span data-ttu-id="6c8c6-156">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6c8c6-156">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="6c8c6-157">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6c8c6-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="6c8c6-158">упдатефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="6c8c6-158">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="6c8c6-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6c8c6-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="6c8c6-160">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6c8c6-160">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="6c8c6-161">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6c8c6-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6c8c6-162">Folders</span><span class="sxs-lookup"><span data-stu-id="6c8c6-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="6c8c6-163">Folder</span><span class="sxs-lookup"><span data-stu-id="6c8c6-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="6c8c6-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="6c8c6-164">FolderId</span></span>](folderid.md)
    
## <a name="updatefolder-error-response-example"></a><span data-ttu-id="6c8c6-165">Пример ответа на сообщение об ошибке операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="6c8c6-165">UpdateFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="6c8c6-166">Описание</span><span class="sxs-lookup"><span data-stu-id="6c8c6-166">Description</span></span>

<span data-ttu-id="6c8c6-167">В следующем примере показан ответ об ошибке для запроса операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-167">The following example shows an error response to an UpdateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="6c8c6-168">Код</span><span class="sxs-lookup"><span data-stu-id="6c8c6-168">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="6c8c6-169">Комментарии</span><span class="sxs-lookup"><span data-stu-id="6c8c6-169">Comments</span></span>

<span data-ttu-id="6c8c6-170">В этом примере показан ответ об ошибке, вызванный недопустимым атрибутом **чанжекэй** в запросе.</span><span class="sxs-lookup"><span data-stu-id="6c8c6-170">This example shows an error response that is caused by an invalid **ChangeKey** attribute in the request.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="6c8c6-171">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="6c8c6-171">Error response elements</span></span>

<span data-ttu-id="6c8c6-172">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6c8c6-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="6c8c6-173">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6c8c6-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="6c8c6-174">упдатефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="6c8c6-174">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="6c8c6-175">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6c8c6-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="6c8c6-176">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6c8c6-176">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="6c8c6-177">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="6c8c6-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="6c8c6-178">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6c8c6-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6c8c6-179">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="6c8c6-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="6c8c6-180">Folders</span><span class="sxs-lookup"><span data-stu-id="6c8c6-180">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="6c8c6-181">См. также</span><span class="sxs-lookup"><span data-stu-id="6c8c6-181">See also</span></span>



- [<span data-ttu-id="6c8c6-182">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6c8c6-182">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

