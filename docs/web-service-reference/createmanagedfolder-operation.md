---
title: Операция CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: Операция CreateManagedFolder создает управляемые папки в Exchange магазине.
ms.openlocfilehash: 2b00691fbaba294950a091d5caafb8054f3e2073
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536426"
---
# <a name="createmanagedfolder-operation"></a>Операция CreateManagedFolder

Операция CreateManagedFolder создает управляемые папки в Exchange магазине.
  
## <a name="using-the-createmanagedfolder-operation"></a>Использование операции CreateManagedFolder

Операция CreateManagedFolder добавляет управляемые пользовательские папки в почтовый ящик пользователя. Для поиска доступных управляемых папок можно использовать Exchange управления Shell **Get-ManagedFolder** для добавления доступных управляемых папок. Хотя этот комлет возвращает как управляемые пользовательские папки, так и управляемые папки по умолчанию, можно добавить только управляемые пользовательские папки. Управляемые пользовательские папки идентифицированы типом папки ManagedCustomFolder. Пространство имен System.DirectoryServices также включает типы, которые можно использовать для обнаружения имен доступных управляемых папок. 
  
> [!NOTE]
> Вы не Exchange веб-службы, чтобы найти имена доступных управляемых папок для добавления в почтовый ящик. 
  
Операции FindFolder и GetFolder можно использовать для доступа к управляемым папкам. FindFolder используется для поиска папок в указанной родительской папке. Это можно использовать для обнаружения управляемых папок в папке перед попыткой добавить дубликат управляемой пользовательской папки в тот же каталог. GetFolder используется после операции FindFolder для получения дополнительных сведений о управляемой пользовательской папке.
  
## <a name="remarks"></a>Заметки

Сведения о том, как настроить политику управления записями сообщений (MRM), см. в руб. Как создать политику управляемых папок [почтовых ящиков.](https://go.microsoft.com/fwlink/?LinkId=100975)
  
Сведения о том, как удалить управляемые пользовательские папки из почтового ящика, см. в сообщении [Remove-ManagedFolder.](https://go.microsoft.com/fwlink/?LinkId=100976)
  
## <a name="createmanagedfolder-request-example"></a>Пример запроса CreateManagedFolder

### <a name="description"></a>Описание

В следующем примере запроса CreateManagedFolder показано, как добавить в почтовый ящик управляемые папки с именем Test Managed Folder.
  
> [!NOTE]
> Вы также можете использовать делегатский доступ для добавления управляемых пользовательских папок. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
- [FolderName](foldername.md)
    
Чтобы найти другие варианты сообщения запроса операции CreateManagedFolder, ознакомьтесь с иерархией схемы. Начните с [элемента CreateManagedFolder.](createmanagedfolder.md) 
  
## <a name="successful-createmanagedfolder-response"></a>Успешный ответ CreateManagedFolder

### <a name="description"></a>Описание

В следующем примере кода показан успешный ответ на запрос CreateManagedFolder.
  
> [!NOTE]
> Значения **атрибутов Id** и **ChangeKey** были сокращены для сохранения читаемости. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Чтобы найти другие варианты ответных сообщений операции CreateManagedFolder, ознакомьтесь с иерархией схемы. Начните с [элемента CreateManagedFolderResponse.](createmanagedfolderresponse.md) 
  
## <a name="createmanagedfolder-error-response"></a>Ответ на ошибку CreateManagedFolder

### <a name="description"></a>Описание

В следующем примере кода показан ответ на ошибку на запрос CreateManagedFolder.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>Элементы ответа на ошибки

В ответе на ошибку используются следующие элементы:
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также



[Операция GetFolder](getfolder-operation.md)
  
[Операция FindFolder](findfolder-operation.md)


[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

