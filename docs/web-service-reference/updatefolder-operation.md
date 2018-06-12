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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840324"
---
# <a name="updatefolder-operation"></a>Операцию UpdateFolder

Операция UpdateFolder используется для изменения свойств существующего элемента в хранилище Exchange. Каждую операцию UpdateFolder состоит из следующих компонентов:
  
- Элемент [FolderId](folderid.md) , путь к папке для обновления. 
    
- Внутренний путь элемента в папке, в соответствии с фигуры папки, который определяет данные для обновления.
    
- Папка, содержащая новое значение обновленные поля, если обновление не удаления.
    
## <a name="remarks"></a>Замечания

Три основные обновления действия над элементом. В следующей таблице перечислены эти действия.
  
|**Действие**|**Описание**|
|:-----|:-----|
|Добавление  <br/> |Добавление действия добавляет данные существующего свойства. Он сохраняет данные. Добавьте не применяется ко всем свойствам.  <br/> |
|Set  <br/> |Набор действий заменяет данных для свойства, если он содержит данные, или создает свойство и задает его значение, если не существует. Набор действий применима только для записи свойств.  <br/> |
|Удаление  <br/> |Удаление удаляет свойство из папки. Это отличается от параметра пустое значение. Закончив настройку, свойство не существует для папки. Удалить применима только для записи свойств.  <br/> |
   
## <a name="updatefolder-request-example"></a>Пример запроса UpdateFolder

### <a name="description"></a>Описание

В следующем примере запрос UpdateFolder показано, как обновить отображаемое имя папки. 
  
### <a name="code"></a>Программа

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

### <a name="comments"></a>Комментарии

В этом примере изменяется отображаемое имя папки Новое_имя_папки.
  
> [!NOTE]
> Значения **Id** и **ChangeKey** атрибутов элемента [FolderId](folderid.md) URL были сокращены для удобства чтения. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
В разделе Схема дополнительных элементов, которые можно использовать для формирования запроса UpdateFolder.
  
> [!NOTE]
> Расположение по умолчанию схемы находится в виртуальном каталоге EWS на компьютере, на котором установлена роль сервера клиентского доступа. 
  
## <a name="updatefolder-response-example"></a>Пример ответа UpdateFolder

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос UpdateFolder. В этом примере новый ключ изменения возвращается в соответствии с обновленное состояние папки.
  
### <a name="code"></a>Программа

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

### <a name="comments"></a>Комментарии

> [!NOTE]
> Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость. 
  
Идентификатор папки, возвращаемого в ответе представляет обновленные папки.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Папки](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
## <a name="updatefolder-error-response-example"></a>Пример ответа об ошибке UpdateFolder

### <a name="description"></a>Описание

В следующем примере показано ошибочный ответ на запрос UpdateFolder.
  
### <a name="code"></a>Программа

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

### <a name="comments"></a>Комментарии

В этом примере показано возврату ошибки, возникающие при недопустимый атрибут **ChangeKey** в запросе. 
  
### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Папки](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

