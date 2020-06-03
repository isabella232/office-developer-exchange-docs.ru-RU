---
title: Операция MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: c7233966-6c87-4a14-8156-b1610760176d
description: Операция MoveFolder перемещает папки из указанной папки и размещает их в другой папке.
ms.openlocfilehash: dc572130ca3b2f2b152abbb4a8b68cc6f67790e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460584"
---
# <a name="movefolder-operation"></a>Операция MoveFolder

Операция MoveFolder перемещает папки из указанной папки и размещает их в другой папке.
  
## <a name="remarks"></a>Примечания

Операция MoveFolder подобна операции CopyFolder. Невозможно переместить папки "различающиеся папки". В целевую папку можно переместить сразу несколько папок.
  
## <a name="movefolder-request-example"></a>Пример запроса MoveFolder

### <a name="description"></a>Description

В приведенном ниже примере запроса MoveFolder показано, как создать запрос на перемещение папки, определенной [FolderId](folderid.md) , и поместить ее в папку нежелательной почты. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="junkemail"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AScAc"/>
      </FolderIds>
    </MoveFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

> [!NOTE]
> Значение атрибута ID элемента [FolderId](folderid.md) было сокращено для удобочитаемости. 
  
### <a name="request-elements"></a>Элементы Request

Этот запрос MoveFolder включает следующие элементы:
  
- [MoveFolder](movefolder.md)
    
- [тофолдерид](tofolderid.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [фолдеридс](folderids.md)
    
- [FolderId](folderid.md)
    
В схеме представлены дополнительные элементы, которые можно использовать для формирования запроса MoveFolder.
  
> [!NOTE]
> Расположение схемы по умолчанию находится в виртуальном каталоге EWS на компьютере, на котором установлена роль сервера клиентского доступа. 
  
## <a name="successful-movefolder-response-example"></a>Пример успешного ответа MoveFolder

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос MoveFolder. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFV" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

> [!NOTE]
> Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость. 
  
FolderId, возвращаемый в ответе, представляет папку, которая была перемещена в новое расположение папки.
  
### <a name="response-elements"></a>Элементы Response

Ответ MoveFolder включает следующие элементы:
  
- [мовефолдерреспонсе](movefolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [мовефолдерреспонсемессаже](movefolderresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
## <a name="movefolder-error-response-example"></a>Пример ответа на сообщение об ошибке MoveFolder

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке, возникающий при попытке переместить различающиеся папки.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot move distinguished folder.</m:MessageText>
          <m:ResponseCode>ErrorMoveDistinguishedFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ошибочного ответа

Ответ об ошибке MoveFolder включает следующие элементы:
  
- [мовефолдерреспонсе](movefolderresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [мовефолдерреспонсемессаже](movefolderresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также



[Операция CopyFolder](copyfolder-operation.md)

