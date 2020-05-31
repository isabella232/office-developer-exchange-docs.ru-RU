---
title: Операция CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: Операция CopyFolder копирует папки в почтовом ящике.
ms.openlocfilehash: a83444ff0927a3c8fe075c79d44d02357a737773
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761835"
---
# <a name="copyfolder-operation"></a>Операция CopyFolder

Операция CopyFolder копирует папки в почтовом ящике.
  
## <a name="using-the-copyfolder-operation"></a>Использование операции CopyFolder

Операция CopyFolder подобна [операции MoveFolder](movefolder-operation.md). Он копирует идентифицированные папки и возвращает **идентификатор** и **чанжекэй** скопированных папок. 
  
## <a name="copyfolder-request-example"></a>Пример запроса CopyFolder

### <a name="description"></a>Описание

В приведенном ниже примере запроса CopyFolder показано, как скопировать папки в папку "Входящие".
  
> [!NOTE]
> Значение атрибута **ID** элемента [FolderId](folderid.md) было сокращено для удобочитаемости. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Папки можно определять с помощью элемента [дистингуишедфолдерид](distinguishedfolderid.md) или элемента [FolderId](folderid.md) для использования в элементах [тофолдерид](tofolderid.md) или [фолдеридс](folderids.md) . 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [CopyFolder](copyfolder.md)
    
- [тофолдерид](tofolderid.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [фолдеридс](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
Чтобы найти другие параметры сообщения Request операции CopyFolder, изучите иерархию схемы. Начните с элемента [CopyFolder](copyfolder.md) . 
  
## <a name="successful-copyfolder-response"></a>Успешный ответ CopyFolder

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос CopyFolder. 
  
> [!NOTE]
> Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="code"></a>Код

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
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>Comment

Элемент [FolderId](folderid.md) , возвращаемый в ответе, представляет папку, скопированную в новом расположении папки. 
  
### <a name="response-elements"></a>Элементы Response

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [копифолдерреспонсе](copyfolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [копифолдерреспонсемессаже](copyfolderresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Чтобы найти другие параметры для ответного сообщения операции CopyFolder, изучите иерархию схемы. Начните с элемента [копифолдерреспонсе](copyfolderresponse.md) . 
  
## <a name="copyfolder-error-response"></a>Ответ об ошибке CopyFolder

### <a name="description"></a>Описание

В следующем примере показан ответ об ошибке для запроса CopyFolder. Ошибка возникла из-за того, что папка с таким отображаемым именем уже существует.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [копифолдерреспонсе](copyfolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [копифолдерреспонсемессаже](copyfolderresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
Чтобы найти другие параметры сообщения об ошибке при выполнении операции CopyFolder, изучите иерархию схемы. Начните с элемента [копифолдерреспонсе](copyfolderresponse.md) . 
  
## <a name="see-also"></a>См. также

- [Операция MoveFolder](movefolder-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

