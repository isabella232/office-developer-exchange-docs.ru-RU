---
title: Операция DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: b0f92682-4895-4bcf-a4a1-e4c2e8403979
description: Операция DeleteFolder удаление папки из почтового ящика.
ms.openlocfilehash: 0fd7c9d4b04a706dcdb83f41087eaa4f3d45f129
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762033"
---
# <a name="deletefolder-operation"></a>Операция DeleteFolder

Операция **DeleteFolder** удаление папки из почтового ящика. 
  
## <a name="deletefolder-request-example"></a>Пример запроса DeleteFolder

### <a name="description"></a>Описание

В следующем примере запроса **DeleteFolder** показано, как для формирования запроса, чтобы удалить папку. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

В этом примере выполняется окончательного удаления в общей папке.
  
> [!NOTE]
> Идентификатор папки был усечен, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [DeleteFolder](deletefolder.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа. 
  
Чтобы найти другие параметры для запроса **DeleteFolder** операции, изучите иерархия схемы. Запустите в элементе [DeleteFolder](deletefolder.md) . 
  
## <a name="successful-deletefolder-response"></a>Успешного ответа DeleteFolder

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **DeleteFolder** . 
  
### <a name="code"></a>Программа

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
    <DeleteFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>Элементы ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteFolderResponse](deletefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
Чтобы найти другие параметры в сообщении ответа **DeleteFolder** операции, изучите иерархия схемы. Запустите в элементе [DeleteFolderResponse](deletefolderresponse.md) . 
  
## <a name="deletefolder-error-response"></a>Отклик DeleteFolder

### <a name="description"></a>Описание

В следующем примере показано ошибочный ответ на запрос **DeleteFolder** . Ошибка была вызвана запрос на удаление папки, который не был представлен в почтовом ящике. 
  
### <a name="code"></a>Программа

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
    <DeleteFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Операция **DeleteFolder** не может использоваться для различающееся папок. 
  
### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteFolderResponse](deletefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Чтобы найти другие параметры в сообщении об ошибке ответа **DeleteFolder** операции, изучите иерархия схемы. Запустите в элементе [DeleteFolderResponse](deletefolderresponse.md) . 
  
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Удаление папок](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

