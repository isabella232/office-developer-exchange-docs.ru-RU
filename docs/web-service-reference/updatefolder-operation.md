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
# <a name="updatefolder-operation"></a>Операция UpdateFolder

Операция операцию UpdateFolder используется для изменения свойств существующего элемента в хранилище Exchange. Каждая операция операцию UpdateFolder состоит из следующих элементов:
  
- Элемент [FolderId](folderid.md) , указывающий папку, которую требуется обновить. 
    
- Внутренний путь к элементу в папке, как указано в фигуре папки, в которой задаются данные для обновления.
    
- Папка, содержащая новое значение обновленного поля, если обновление не является удалением.
    
## <a name="remarks"></a>Примечания

Для элемента можно выполнить три основных действия обновления. Эти действия перечислены в приведенной ниже таблице.
  
|**Действие**|**Описание**|
|:-----|:-----|
|Error  <br/> |Действие Append добавляет данные к существующему свойству. Они сохраняют текущие данные. Append не применимо ко всем свойствам.  <br/> |
|Set  <br/> |Действие Set замещает данные для свойства, если оно содержит данные, или создает свойство и задает его значение, если оно не существует. Действие Set применяется только к записываемым свойствам.  <br/> |
|Удаление  <br/> |Действие DELETE удаляет свойство из папки. Это отличается от присвоения пустого значения. По завершении свойство для папки не существует. DELETE применяется только к записываемым свойствам.  <br/> |
   
## <a name="updatefolder-request-example"></a>Пример запроса операцию UpdateFolder

### <a name="description"></a>Описание

В приведенном ниже примере запроса операцию UpdateFolder показано, как обновить отображаемое имя папки. 
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

В этом примере показано изменение отображаемого имени папки на Невфолдернаме.
  
> [!NOTE]
> Значения атрибутов **ID** и **чанжекэй** элемента [FolderId](folderid.md) сокращены для удобочитаемости. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [UpdateFolder](updatefolder.md)
    
- [фолдерчанжес](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [сетфолдерфиелд](setfolderfield.md)
    
- [фиелдури](fielduri.md)
    
- [Folder](folder.md)
    
- [DisplayName (строка)](displayname-string.md)
    
В схеме представлены дополнительные элементы, которые можно использовать для формирования запроса операцию UpdateFolder.
  
> [!NOTE]
> Расположение схемы по умолчанию находится в виртуальном каталоге EWS на компьютере, на котором установлена роль сервера клиентского доступа. 
  
## <a name="updatefolder-response-example"></a>Пример отклика операцию UpdateFolder

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос операцию UpdateFolder. В этом примере возвращается новый ключ изменения, который отражает обновленное состояние папки.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

> [!NOTE]
> Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость. 
  
Идентификатор папки, возвращаемой в ответе, представляет обновленную папку.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [упдатефолдерреспонсе](updatefolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [упдатефолдерреспонсемессаже](updatefolderresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
## <a name="updatefolder-error-response-example"></a>Пример ответа на сообщение об ошибке операцию UpdateFolder

### <a name="description"></a>Описание

В следующем примере показан ответ об ошибке для запроса операцию UpdateFolder.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

В этом примере показан ответ об ошибке, вызванный недопустимым атрибутом **чанжекэй** в запросе. 
  
### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [упдатефолдерреспонсе](updatefolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [упдатефолдерреспонсемессаже](updatefolderresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

