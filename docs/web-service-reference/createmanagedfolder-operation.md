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
description: Операция CreateManagedFolder создает управляемую папку в хранилище Exchange.
ms.openlocfilehash: 779c730b55b9b441644108a6837f9e22d39cc2f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44444595"
---
# <a name="createmanagedfolder-operation"></a>Операция CreateManagedFolder

Операция CreateManagedFolder создает управляемую папку в хранилище Exchange.
  
## <a name="using-the-createmanagedfolder-operation"></a>Использование операции CreateManagedFolder

Операция CreateManagedFolder добавляет настраиваемую управляемую папку в почтовый ящик пользователя. С помощью командлета **Get – ManagedFolder** в командной консоли Exchange можно найти доступные управляемые папки для добавления. Несмотря на то, что этот командлет возвращает как управляемые настраиваемые папки, так и управляемые папки по умолчанию, можно добавлять только настраиваемые папки с управляемыми папками. Управляемые настраиваемые папки определяются типом папки Манажедкустомфолдер. Пространство имен System. DirectoryServices также включает типы, которые можно использовать для обнаружения имен доступных управляемых папок. 
  
> [!NOTE]
> Веб-службы Exchange невозможно использовать для поиска имен доступных управляемых папок, добавляемых в почтовый ящик. 
  
Вы можете использовать операции FindFolder и a Folder для доступа к управляемым папкам. FindFolder используется для поиска папок в указанной родительской папке. Это можно использовать для обнаружения управляемых папок в папке перед попыткой добавить дублирующую управляемую настраиваемую папку в тот же каталог. "-Папка" используется после операции FindFolder для получения дополнительных сведений об управляемой настраиваемой папке.
  
## <a name="remarks"></a>Примечания

Сведения о том, как настроить политику управления записями сообщений (управления ЗАПИСЯМИ сообщений), приведены [в статье Создание политики почтовых ящиков управляемых папок](https://go.microsoft.com/fwlink/?LinkId=100975).
  
Сведения об удалении управляемых настраиваемых папок из почтового ящика можно найти в статье [Remove – ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).
  
## <a name="createmanagedfolder-request-example"></a>Пример запроса CreateManagedFolder

### <a name="description"></a>Description

В приведенном ниже примере запроса CreateManagedFolder показано, как добавить управляемую папку с именем Test Managed Folder в почтовый ящик.
  
> [!NOTE]
> Вы также можете использовать делегированный доступ для добавления настраиваемых управляемых папок. 
  
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

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [фолдернамес](foldernames.md)
    
- [FolderName](foldername.md)
    
Чтобы найти другие параметры сообщения Request операции CreateManagedFolder, изучите иерархию схемы. Начните с элемента [CreateManagedFolder](createmanagedfolder.md) . 
  
## <a name="successful-createmanagedfolder-response"></a>Успешный ответ CreateManagedFolder

### <a name="description"></a>Description

В следующем примере кода показан успешный ответ на запрос CreateManagedFolder.
  
> [!NOTE]
> Значения атрибута **ID** и **чанжекэй** были сокращены для сохранения удобочитаемости. 
  
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

В отклике используются следующие элементы: 
  
- [креатеманажедфолдерреспонсе](createmanagedfolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеманажедфолдерреспонсемессаже](createmanagedfolderresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Чтобы найти другие параметры для ответных сообщений операции CreateManagedFolder, изучите иерархию схемы. Начните с элемента [креатеманажедфолдерреспонсе](createmanagedfolderresponse.md) . 
  
## <a name="createmanagedfolder-error-response"></a>Ответ об ошибке CreateManagedFolder

### <a name="description"></a>Description

В следующем примере кода показан ответ об ошибке для запроса CreateManagedFolder.
  
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

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [креатеманажедфолдерреспонсе](createmanagedfolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеманажедфолдерреспонсемессаже](createmanagedfolderresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также



[Операция GetFolder](getfolder-operation.md)
  
[Операция FindFolder](findfolder-operation.md)


[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

