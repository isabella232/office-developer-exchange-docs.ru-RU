---
title: Операция CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: Операция CreateManagedFolder создает управляемых папок в хранилище Exchange.
ms.openlocfilehash: 2c2af53dc5dbe1e6fcbc7f3b1174a856e51e4905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761909"
---
# <a name="createmanagedfolder-operation"></a>Операция CreateManagedFolder

Операция CreateManagedFolder создает управляемых папок в хранилище Exchange.
  
## <a name="using-the-createmanagedfolder-operation"></a>С помощью операции CreateManagedFolder

Операция CreateManagedFolder добавляет настраиваемой управляемой папки почтового ящика пользователя. Командлет командной консоли Exchange **Get-ManagedFolder** найти доступные управляемые папки для добавления. Несмотря на то, что этот командлет возвращает управляемые настраиваемые папки и управляемые папки по умолчанию, только управляемые настраиваемые папки можно добавить. Управляемые настраиваемые папки, идентифицируются по типу папки ManagedCustomFolder. Пространство имен System.DirectoryServices также содержит типы, которые можно использовать для получения имен доступных управляемых папок. 
  
> [!NOTE]
> Нельзя использовать веб-служб Exchange для поиска имен доступен управляемые папки для добавления к почтовому ящику. 
  
Операции FindFolder и GetFolder можно использовать для доступа к управляемых папок. FindFolder используется для поиска папок в указанной родительской папки. Можно использовать, чтобы управляемые папки для обнаружения в папке, прежде чем пытаться добавить дубликат настраиваемую управляемую папку на том же каталоге. GetFolder используется после операции FindFolder для получения дополнительных сведений о настраиваемой управляемой папки.
  
## <a name="remarks"></a>Замечания

Сведения о настройке политики управления записями обмена сообщениями Узнайте, [как создать политику почтовых ящиков управляемых папок](http://go.microsoft.com/fwlink/?LinkId=100975).
  
Сведения о том, как удалить управляемые настраиваемые папки из почтового ящика можно [Remove-ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976).
  
## <a name="createmanagedfolder-request-example"></a>Пример запроса CreateManagedFolder

### <a name="description"></a>Описание

В следующем примере запрос CreateManagedFolder показано, как для добавления управляемых папок с именем Test управляемых папок для почтового ящика.
  
> [!NOTE]
> Передача прав доступа можно также использовать для добавления настраиваемых управляемых папок. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [FolderNames](foldernames.md)
    
- [Имя папки](foldername.md)
    
Чтобы найти другие параметры для запроса CreateManagedFolder операции, изучите иерархия схемы. Запустите в элементе [CreateManagedFolder](createmanagedfolder.md) . 
  
## <a name="successful-createmanagedfolder-response"></a>Успешного ответа CreateManagedFolder

### <a name="description"></a>Описание

В следующем примере кода показано успешного ответа на запрос CreateManagedFolder.
  
> [!NOTE]
> Значения атрибута **Id** и **ChangeKey** URL-были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы: 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Папки](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Чтобы найти другие параметры сообщений ответа CreateManagedFolder операции, изучите иерархия схемы. Запустите в элементе [CreateManagedFolderResponse](createmanagedfolderresponse.md) . 
  
## <a name="createmanagedfolder-error-response"></a>Ошибка CreateManagedFolder ответа

### <a name="description"></a>Описание

В следующем примере кода показано ошибочный ответ на запрос CreateManagedFolder.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Папки](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также



[GetFolder Operation](getfolder-operation.md)
  
[FindFolder Operation](findfolder-operation.md)


[Поиск папок](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

