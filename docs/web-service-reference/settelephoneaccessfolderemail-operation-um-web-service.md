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
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a><span data-ttu-id="21cdc-103">Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="21cdc-103">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>

<span data-ttu-id="21cdc-104">Операция SetTelephoneAccessFolderEmail задает папку, из которой единая система обмена сообщениями будет читать сообщения пользователю по телефону.</span><span class="sxs-lookup"><span data-stu-id="21cdc-104">The SetTelephoneAccessFolderEmail operation sets the folder from which Unified Messaging will read back messages to the user over the telephone.</span></span>
  
## <a name="settelephoneaccessfolderemail-request-example"></a><span data-ttu-id="21cdc-105">Пример запроса SetTelephoneAccessFolderEmail</span><span class="sxs-lookup"><span data-stu-id="21cdc-105">SetTelephoneAccessFolderEmail request example</span></span>

### <a name="description"></a><span data-ttu-id="21cdc-106">Описание</span><span class="sxs-lookup"><span data-stu-id="21cdc-106">Description</span></span>

<span data-ttu-id="21cdc-107">В приведенном ниже примере запроса SetTelephoneAccessFolderEmail показано, как сформировать запрос на установку папки, из которой единая система обмена сообщениями будет прочитана пользователю по телефону.</span><span class="sxs-lookup"><span data-stu-id="21cdc-107">The following example of a SetTelephoneAccessFolderEmail request shows how to form a request to set the folder from which Unified Messaging will read back to the user over the telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="21cdc-108">Код</span><span class="sxs-lookup"><span data-stu-id="21cdc-108">Code</span></span>

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

## <a name="successful-settelephoneaccessfolderemail-response-example"></a><span data-ttu-id="21cdc-109">Пример успешного ответа SetTelephoneAccessFolderEmail</span><span class="sxs-lookup"><span data-stu-id="21cdc-109">Successful SetTelephoneAccessFolderEmail response example</span></span>

### <a name="description"></a><span data-ttu-id="21cdc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="21cdc-110">Description</span></span>

<span data-ttu-id="21cdc-111">В приведенном ниже примере ответа SetTelephoneAccessFolderEmail показан ответ на запрос SetTelephoneAccessFolderEmail.</span><span class="sxs-lookup"><span data-stu-id="21cdc-111">The following example of a SetTelephoneAccessFolderEmail response shows a response to the SetTelephoneAccessFolderEmail request.</span></span>
  
### <a name="code"></a><span data-ttu-id="21cdc-112">Код</span><span class="sxs-lookup"><span data-stu-id="21cdc-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="21cdc-113">См. также</span><span class="sxs-lookup"><span data-stu-id="21cdc-113">See also</span></span>



[<span data-ttu-id="21cdc-114">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="21cdc-114">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="21cdc-115">Сеттелефонеакцессфолдеремаилреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="21cdc-115">SetTelephoneAccessFolderEmailResponse (UM web service)</span></span>](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[<span data-ttu-id="21cdc-116">base64FolderId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="21cdc-116">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)

