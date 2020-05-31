---
title: Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 2c92d914-bdee-4337-b3ea-0655fdb658e9
description: Операция SetTelephoneAccessFolderEmail задает папку, из которой единая система обмена сообщениями будет читать сообщения пользователю по телефону.
ms.openlocfilehash: 9497e58f66b8efcf7e358aa529223942298a3bed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835459"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a>Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)

Операция SetTelephoneAccessFolderEmail задает папку, из которой единая система обмена сообщениями будет читать сообщения пользователю по телефону.
  
## <a name="settelephoneaccessfolderemail-request-example"></a>Пример запроса SetTelephoneAccessFolderEmail

### <a name="description"></a>Описание

В приведенном ниже примере запроса SetTelephoneAccessFolderEmail показано, как сформировать запрос на установку папки, из которой единая система обмена сообщениями будет прочитана пользователю по телефону.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a>Пример успешного ответа SetTelephoneAccessFolderEmail

### <a name="description"></a>Описание

В приведенном ниже примере ответа SetTelephoneAccessFolderEmail показан ответ на запрос SetTelephoneAccessFolderEmail.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-um-web-service.md)
  
[Сеттелефонеакцессфолдеремаилреспонсе (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[base64FolderId (веб-служба единой системы обмена сообщениями)](base64folderid-um-web-service.md)

