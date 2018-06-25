---
title: Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)
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
description: Операция SetTelephoneAccessFolderEmail задает папку, из которой единой системы обмена сообщениями будет читать обратная сообщения для пользователя по телефону.
ms.openlocfilehash: 9497e58f66b8efcf7e358aa529223942298a3bed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835459"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a><span data-ttu-id="b9ced-103">Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="b9ced-103">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>

<span data-ttu-id="b9ced-104">Операция SetTelephoneAccessFolderEmail задает папку, из которой единой системы обмена сообщениями будет читать обратная сообщения для пользователя по телефону.</span><span class="sxs-lookup"><span data-stu-id="b9ced-104">The SetTelephoneAccessFolderEmail operation sets the folder from which Unified Messaging will read back messages to the user over the telephone.</span></span>
  
## <a name="settelephoneaccessfolderemail-request-example"></a><span data-ttu-id="b9ced-105">Пример запроса SetTelephoneAccessFolderEmail</span><span class="sxs-lookup"><span data-stu-id="b9ced-105">SetTelephoneAccessFolderEmail request example</span></span>

### <a name="description"></a><span data-ttu-id="b9ced-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b9ced-106">Description</span></span>

<span data-ttu-id="b9ced-107">В следующем примере запрос SetTelephoneAccessFolderEmail показано, как для формирования запроса, чтобы задать папку, из которой единой системы обмена сообщениями будет выполнять чтение для пользователя по телефону.</span><span class="sxs-lookup"><span data-stu-id="b9ced-107">The following example of a SetTelephoneAccessFolderEmail request shows how to form a request to set the folder from which Unified Messaging will read back to the user over the telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="b9ced-108">Программа</span><span class="sxs-lookup"><span data-stu-id="b9ced-108">Code</span></span>

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

## <a name="successful-settelephoneaccessfolderemail-response-example"></a><span data-ttu-id="b9ced-109">Пример успешного ответа SetTelephoneAccessFolderEmail</span><span class="sxs-lookup"><span data-stu-id="b9ced-109">Successful SetTelephoneAccessFolderEmail response example</span></span>

### <a name="description"></a><span data-ttu-id="b9ced-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9ced-110">Description</span></span>

<span data-ttu-id="b9ced-111">В следующем примере ответа SetTelephoneAccessFolderEmail показано ответа на запрос SetTelephoneAccessFolderEmail.</span><span class="sxs-lookup"><span data-stu-id="b9ced-111">The following example of a SetTelephoneAccessFolderEmail response shows a response to the SetTelephoneAccessFolderEmail request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b9ced-112">Программа</span><span class="sxs-lookup"><span data-stu-id="b9ced-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="b9ced-113">См. также</span><span class="sxs-lookup"><span data-stu-id="b9ced-113">See also</span></span>



[<span data-ttu-id="b9ced-114">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="b9ced-114">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="b9ced-115">SetTelephoneAccessFolderEmailResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="b9ced-115">SetTelephoneAccessFolderEmailResponse (UM web service)</span></span>](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[<span data-ttu-id="b9ced-116">base64FolderId (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="b9ced-116">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)

