---
title: Операция SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: b31916b1-bc6c-4451-a475-b7c5417f752d
description: Операция SyncFolderHierarchy синхронизирует папки между компьютером, на котором работает Microsoft Exchange Server 2010 и клиентом.
ms.openlocfilehash: 1c7ad2413064161ba54e8a7a30bfcd6f23f218bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456432"
---
# <a name="syncfolderhierarchy-operation"></a>Операция SyncFolderHierarchy

Операция SyncFolderHierarchy синхронизирует папки между компьютером, на котором работает Microsoft Exchange Server 2010 и клиентом.
  
> [!NOTE]
> Операция SyncFolderHierarchy не возвращает папки при изменении свойств [унреадкаунт](unreadcount.md) или [тоталкаунт](totalcount.md) . 
  
## <a name="syncfolderhierarchy-request-example"></a>Пример запроса SyncFolderHierarchy

### <a name="description"></a>Описание

В приведенном ниже примере запроса SyncFolderHierarchy показано, как синхронизировать иерархию клиентских папок с сервером Exchange. В этом примере показана иерархия папок, которая уже синхронизирована по крайней мере один раз. Элемент [синкстате](syncstate-ex15websvcsotherref.md) не включается в запрос первой попытки синхронизации клиента с сервером Exchange. Первый запрос возвратит все папки в почтовом ящике. Элемент [синкстате](syncstate-ex15websvcsotherref.md) будет возвращен в [синкфолдерхиерарчиреспонсе](syncfolderhierarchyresponse.md). Этот элемент используется для синхронизации состояния последующих запросов SyncFolderHierarchy.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Данные элемента [синкстате](syncstate-ex15websvcsotherref.md) с кодировкой base64 были сокращены для сохранения удобочитаемости. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [SyncFolderHierarchy](syncfolderhierarchy.md)
    
- [фолдершапе](foldershape.md)
    
- [басешапе](baseshape.md)
    
- [синкстате](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> Схема, описывающая эти элементы, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Майкрософт Exchange Server 2007, на котором установлена роль сервера клиентского доступа. 
  
## <a name="successful-syncfolderhierarchy-response"></a>Успешный ответ SyncFolderHierarchy

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос SyncFolderHierarchy. В этом примере выполняется синхронизация новой папки.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AQApAHR=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQApA=" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>NewFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Данные элемента [синкстате](syncstate-ex15websvcsotherref.md) с кодировкой base64 и идентификатора папки были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [синкфолдерхиерарчиреспонсе](syncfolderhierarchyresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [синкфолдерхиерарчиреспонсемессаже](syncfolderhierarchyresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [синкстате](syncstate-ex15websvcsotherref.md)
    
- [инклудесластфолдеринранже](includeslastfolderinrange.md)
    
- [Изменения (иерархия)](changes-hierarchy.md)
    
- [Create (Фолдерсинк)](create-foldersync.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [ParentFolderId](parentfolderid.md)
    
- [фолдеркласс](folderclass.md)
    
- [DisplayName (строка)](displayname-string.md)
    
- [тоталкаунт](totalcount.md)
    
- [чилдфолдеркаунт](childfoldercount.md)
    
- [унреадкаунт](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a>Ответ об ошибке SyncFolderHierarchy

### <a name="description"></a>Описание

В следующем примере показан ответ об ошибке для запроса SyncFolderHierarchy. Эта ошибка вызвана недопустимым Синкстате.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupted or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [синкфолдерхиерарчиреспонсе](syncfolderhierarchyresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [синкфолдерхиерарчиреспонсемессаже](syncfolderhierarchyresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [синкстате](syncstate-ex15websvcsotherref.md)
    
- [инклудесластфолдеринранже](includeslastfolderinrange.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

