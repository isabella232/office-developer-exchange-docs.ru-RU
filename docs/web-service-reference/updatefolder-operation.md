---
title: Операцию UpdateFolder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: 'Операция UpdateFolder используется для изменения свойств существующего элемента в Exchange магазине. Каждая операция UpdateFolder состоит из следующих действий:'
ms.openlocfilehash: be8e39e13681cea34e312158c348c60a94374bec
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541765"
---
# <a name="updatefolder-operation"></a>Операцию UpdateFolder

Операция UpdateFolder используется для изменения свойств существующего элемента в Exchange магазине. Каждая операция UpdateFolder состоит из следующих действий:
  
- Элемент [FolderId,](folderid.md) который указывает папку для обновления. 
    
- Внутренний путь элемента в папке, указанный фигурой папки, которая указывает данные для обновления.
    
- Папка с новым значением обновленного поля, если обновление не является удалением.
    
## <a name="remarks"></a>Заметки

В элементе можно выполнить три базовых действия обновления. Эти действия перечислены в следующей таблице.
  
|**Действие**|**Описание**|
|:-----|:-----|
|Приложение  <br/> |Действие приложения добавляет данные в существующее свойство. Он сохраняет данные, которые находятся в настоящее время. Приложение не применимо к всем свойствам.  <br/> |
|Set  <br/> |Действие набора заменяет данные для свойства, если оно содержит данные, или создает свойство и задает его значение, если оно не существует. Действие набора применимо только к рукописным свойствам.  <br/> |
|Удалить  <br/> |Действие удаления удаляет свойство из папки. Это отличается от установки его на пустое значение. По завершению свойство не существует для папки. Удаление применимо только к writable свойствам.  <br/> |
   
## <a name="updatefolder-request-example"></a>Пример запроса UpdateFolder

### <a name="description"></a>Описание

В следующем примере запроса UpdateFolder показано, как обновить имя отображения папки. 
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Комментарии

В этом примере имя отображения папки изменяется на NewFolderName.
  
> [!NOTE]
> Для читаемости сокращены значения атрибутов **Id** и **ChangeKey** элемента [FolderId.](folderid.md) 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Updates (Folder)](updates-folder.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [DisplayName (string)](displayname-string.md)
    
См. схему дополнительных элементов, которые можно использовать для формирования запроса UpdateFolder.
  
> [!NOTE]
> Расположение схемы по умолчанию находится в виртуальном каталоге EWS на компьютере с установленной ролью сервера клиентского доступа. 
  
## <a name="updatefolder-response-example"></a>Пример ответа UpdateFolder

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос UpdateFolder. В этом примере возвращается новый ключ изменения для отражения обновленного состояния папки.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Комментарии

> [!NOTE]
> ID папки и ключ изменения были сокращены для сохранения читаемости. 
  
Возвращаемая в ответ папка представляет обновленную папку.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
## <a name="updatefolder-error-response-example"></a>Пример ответа на ошибку UpdateFolder

### <a name="description"></a>Описание

В следующем примере показан ответ на ошибку на запрос UpdateFolder.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Комментарии

В этом примере показан ответ на ошибку, вызванный недействительным атрибутом **ChangeKey** в запросе. 
  
### <a name="error-response-elements"></a>Элементы ответа на ошибки

В ответе на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

