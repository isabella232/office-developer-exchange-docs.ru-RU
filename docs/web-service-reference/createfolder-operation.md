---
title: Операция CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: Операция CreateFolder создает папки, папки календарей, папки контактов, папки задач и папки поиска.
ms.openlocfilehash: 125a6d212e5eaf85ace71c048de809f3a05ba9b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457552"
---
# <a name="createfolder-operation"></a>Операция CreateFolder

Операция CreateFolder создает папки, папки календарей, папки контактов, папки задач и папки поиска.
  
## <a name="createfolder-request-example"></a>Пример запроса CreateFolder

### <a name="description"></a>Описание

В приведенном ниже примере запроса CreateFolder показано, как сформировать запрос на создание двух папок в корне почтового ящика.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ParentFolderId>
        <t:DistinguishedFolderId Id="msgfolderroot"/>
      </ParentFolderId>
      <Folders>
        <t:Folder>
          <t:DisplayName>Folder1</t:DisplayName>
        </t:Folder>
        <t:Folder>
          <t:DisplayName>Folder2</t:DisplayName>
        </t:Folder>
      </Folders>
    </CreateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [CreateFolder](createfolder.md)
    
- [ParentFolderId (Таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [DisplayName (строка)](displayname-string.md)
    
> [!NOTE]
> Схема, описывающая эти элементы, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Майкрософт Exchange Server 2007, на котором установлена роль сервера клиентского доступа. 
  
Чтобы найти другие параметры сообщения Request операции CreateFolder, изучите иерархию схемы. Начните с элемента [CreateFolder](createfolder.md) . 
  
> [!NOTE]
> Если вы создаете папку поиска с ограничением с помощью свойства **Calendar: организатора** , последующий вызов get Folder будет возвращать ограничение с помощью свойства **Message: from** . Эти два свойства сопоставляются с одним и тем же базовым свойством MAPI. 
  
Операция CreateFolder поддерживает создание класса настраиваемой папки только при создании папки с помощью универсального элемента типа Folder и установки элемента **фолдеркласс** . 
  
## <a name="successful-createfolder-response-example"></a>Пример успешного ответа CreateFolder

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос CreateFolder. В этом примере ответ возвращает идентификаторы новых папок.
  
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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатефолдерреспонсе](createfolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатефолдерреспонсемессаже](createfolderresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Чтобы найти другие параметры для ответного сообщения операции CreateFolder, изучите иерархию схемы. Начните с элемента [креатефолдерреспонсе](createfolderresponse.md) . 
  
## <a name="createfolder-error-response"></a>Ответ об ошибке CreateFolder

### <a name="description"></a>Описание

В следующем примере показан ответ об ошибке для запроса CreateFolder.
  
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
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A folder with the specified name already exists.</m:MessageText>
          <m:ResponseCode>ErrorFolderExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатефолдерреспонсе](createfolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатефолдерреспонсемессаже](createfolderresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
Чтобы найти другие параметры сообщения об ошибке при выполнении операции CreateFolder, изучите иерархию схемы. Начните с элемента [креатефолдерреспонсе](createfolderresponse.md) . 
  
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)
  
[Операция FindFolder](findfolder-operation.md)
  
 **креатефолдертипе**


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Создание папок (веб-службы Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

