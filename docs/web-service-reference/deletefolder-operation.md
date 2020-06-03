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
description: Операция DeleteFolder удаляет папки из почтового ящика.
ms.openlocfilehash: e9bb9199027c2af2cbbb664ef7ad4fa70b7ef718
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455746"
---
# <a name="deletefolder-operation"></a>Операция DeleteFolder

Операция **DeleteFolder** удаляет папки из почтового ящика. 
  
## <a name="deletefolder-request-example"></a>Пример запроса DeleteFolder

### <a name="description"></a>Description

В следующем примере запроса **DeleteFolder** показано, как сформировать запрос на удаление папки. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

В этом примере выполняется окончательное удаление папки.
  
> [!NOTE]
> Идентификатор папки сокращен, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [DeleteFolder](deletefolder.md)
    
- [фолдеридс](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа. 
  
Чтобы найти другие параметры сообщения Request операции **DeleteFolder** , изучите иерархию схемы. Начните с элемента [DeleteFolder](deletefolder.md) . 
  
## <a name="successful-deletefolder-response"></a>Успешный ответ DeleteFolder

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос **DeleteFolder** . 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>Элементы Response

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [делетефолдерреспонсе](deletefolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [делетефолдерреспонсемессаже](deletefolderresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
Чтобы найти другие параметры для ответного сообщения операции **DeleteFolder** , изучите иерархию схемы. Начните с элемента [делетефолдерреспонсе](deletefolderresponse.md) . 
  
## <a name="deletefolder-error-response"></a>Ответ об ошибке DeleteFolder

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке для запроса **DeleteFolder** . Ошибка вызвана запросом на удаление папки, которая отсутствовала в почтовом ящике. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Операцию **DeleteFolder** нельзя использовать для различающихся папок. 
  
### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [делетефолдерреспонсе](deletefolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [делетефолдерреспонсемессаже](deletefolderresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Чтобы найти другие параметры сообщения об ошибке при выполнении операции **DeleteFolder** , изучите иерархию схемы. Начните с элемента [делетефолдерреспонсе](deletefolderresponse.md) . 
  
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Удаление папок](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

