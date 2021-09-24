---
title: Операция MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: c7233966-6c87-4a14-8156-b1610760176d
description: Операция MoveFolder перемещает папки из указанной папки и помещает их в другую папку.
ms.openlocfilehash: e0b0e93bd070354d03c511382b6096f2d3a07508
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523861"
---
# <a name="movefolder-operation"></a>Операция MoveFolder

Операция MoveFolder перемещает папки из указанной папки и помещает их в другую папку.
  
## <a name="remarks"></a>Заметки

Операция MoveFolder похожа на операцию CopyFolder. Нельзя перемещать различаемую папку. Вы можете переместить несколько папок одновременно в папку назначения.
  
## <a name="movefolder-request-example"></a>Пример запроса MoveFolder

### <a name="description"></a>Описание

В следующем примере запроса MoveFolder показано, как сформировать запрос на перемещение папки, идентифицированной папкой [FolderId,](folderid.md) и поместить ее в отличимую папку нежелательной почты. 
  
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
> Значение атрибута ID элемента [FolderId](folderid.md) было сокращено для читаемости. 
  
### <a name="request-elements"></a>Элементы запроса

Этот запрос MoveFolder включает в себя следующие элементы:
  
- [MoveFolder](movefolder.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
См. схему дополнительных элементов, которые можно использовать для формирования запроса MoveFolder.
  
> [!NOTE]
> Расположение схемы по умолчанию находится в виртуальном каталоге EWS на компьютере с установленной ролью сервера клиентского доступа. 
  
## <a name="successful-movefolder-response-example"></a>Пример успешного ответа MoveFolder

### <a name="description"></a>Описание

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
> ID папки и ключ изменения были сокращены для сохранения читаемости. 
  
Папка, возвращаемая в ответе, представляет папку, перемещенную в новое расположение папки.
  
### <a name="response-elements"></a>Элементы ответа

Ответ MoveFolder включает в себя следующие элементы:
  
- [MoveFolderResponse](movefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MoveFolderResponseMessage](movefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
## <a name="movefolder-error-response-example"></a>Пример ответа на ошибку MoveFolder

### <a name="description"></a>Описание

В следующем примере показан ответ на ошибку, который возникает при попытке перемещения различной папки.
  
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

### <a name="error-response-elements"></a>Элементы ответа на ошибки

Ответ на ошибку MoveFolder включает следующие элементы:
  
- [MoveFolderResponse](movefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MoveFolderResponseMessage](movefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Folders](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>См. также



[Операция CopyFolder](copyfolder-operation.md)

