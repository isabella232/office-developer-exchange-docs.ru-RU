---
title: Операция EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: Операция EmptyFolder приводит к очистке папок в почтовом ящике. Кроме того эта операция позволяет удалять вложенные папки указанной папки. При удалении вложенной папке вложенной папке и сообщения в рамках вложенной папке удаляются.
ms.openlocfilehash: 0192744516c5a6d24b95915452bfcffecc2d92b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762326"
---
# <a name="emptyfolder-operation"></a>Операция EmptyFolder

Операция **EmptyFolder** приводит к очистке папок в почтовом ящике. Кроме того эта операция позволяет удалять вложенные папки указанной папки. При удалении вложенной папке вложенной папке и сообщения в рамках вложенной папке удаляются. 
  
## <a name="emptyfolder-request-example"></a>Пример запроса EmptyFolder

### <a name="description"></a>Описание

В следующем примере запроса **EmptyFolder** показано, как для формирования запроса, чтобы полностью очистить папку. В этом примере удаляются все вложенные папки указанной папки. 
  
> [!NOTE]
> Значения **Id** и **ChangeKey** атрибуты элемента [FolderId](folderid.md) URL были сокращены для удобства чтения. 
  
### <a name="code"></a>Программа

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
    </soap:Header>
    <soap:Body>
      <m:EmptyFolder DeleteType="HardDelete" DeleteSubFolders="true">
        <m:FolderIds>
          <t:FolderId Id="AQMkADhhOGU0"  ChangeKey="AQAAABYAAABsMB" />
        </m:FolderIds>
      </m:EmptyFolder>
    </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>Комментарии

В этом примере выполняется окончательного удаления в общей папке.
  
Папки, можно определить по [DistinguishedFolderId](distinguishedfolderid.md) элемент или элемент [FolderId](folderid.md) для использования в элементе [FolderIds](folderids.md) . 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [EmptyFolder](emptyfolder.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
## <a name="successful-emptyfolder-response"></a>Успешного ответа EmptyFolder

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **EmptyFolder** . 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [EmptyFolderResponse](emptyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [EmptyFolderResponseMessage](emptyfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="emptyfolder-error-response"></a>Ошибка EmptyFolder ответа

### <a name="description"></a>Описание

В следующем примере показано ошибочный ответ на запрос **Emptyfolder** . Ошибка была создана, поскольку операции попытка очистить папку, которая не найден в хранилище Exchange. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetFolderResponse](getfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetFolderResponseMessage](getfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Папки](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

