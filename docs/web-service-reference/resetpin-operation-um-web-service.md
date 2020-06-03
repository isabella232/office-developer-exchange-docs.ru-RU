---
title: Операция ResetPIN (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: Операция ResetPIN изменяет ПИН-код (ТЕЛЕФОННОГО интерфейса пользователя пароль) на новое случайное значение.
ms.openlocfilehash: 8de64ce7a47e9c426f8eb9298e1ca00508fb616c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465494"
---
# <a name="resetpin-operation-um-web-service"></a><span data-ttu-id="8fa40-103">Операция ResetPIN (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="8fa40-103">ResetPIN operation (UM web service)</span></span>

<span data-ttu-id="8fa40-104">Операция ResetPIN изменяет ПИН-код (ТЕЛЕФОННОГО интерфейса пользователя пароль) на новое случайное значение.</span><span class="sxs-lookup"><span data-stu-id="8fa40-104">The ResetPIN operation changes the PIN (TUI password) to a new random value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fa40-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="8fa40-105">Remarks</span></span>

<span data-ttu-id="8fa40-106">Операция ResetPIN создает новый ПИН-код на основе политик ПИН-кодов.</span><span class="sxs-lookup"><span data-stu-id="8fa40-106">The ResetPIN operation creates a new PIN based on the PIN policies.</span></span> <span data-ttu-id="8fa40-107">Если операция выполнена успешно, в почтовый ящик пользователя отправляется сообщение электронной почты, содержащее новый ПИН-код.</span><span class="sxs-lookup"><span data-stu-id="8fa40-107">If the operation is successful, an e-mail message that contains the new PIN is sent to the mailbox of the user.</span></span> <span data-ttu-id="8fa40-108">Если операция завершается с ошибкой, возникает исключение, содержащее сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="8fa40-108">If the operation fails, it will throw an exception that contains information about the failure.</span></span>
  
## <a name="resetpin-request-example"></a><span data-ttu-id="8fa40-109">Пример запроса ResetPIN</span><span class="sxs-lookup"><span data-stu-id="8fa40-109">ResetPIN request example</span></span>

### <a name="description"></a><span data-ttu-id="8fa40-110">Description</span><span class="sxs-lookup"><span data-stu-id="8fa40-110">Description</span></span>

<span data-ttu-id="8fa40-111">В приведенном ниже примере запроса ResetPIN показано, как сформировать запрос на сброс ПИН-кода для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8fa40-111">The following example of a ResetPIN request shows how to form a request to reset the PIN for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="8fa40-112">Код</span><span class="sxs-lookup"><span data-stu-id="8fa40-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a><span data-ttu-id="8fa40-113">Пример успешного ответа ResetPIN</span><span class="sxs-lookup"><span data-stu-id="8fa40-113">Successful ResetPIN response example</span></span>

### <a name="description"></a><span data-ttu-id="8fa40-114">Description</span><span class="sxs-lookup"><span data-stu-id="8fa40-114">Description</span></span>

<span data-ttu-id="8fa40-115">В приведенном ниже примере ответа ResetPIN показан ответ на запрос ResetPIN.</span><span class="sxs-lookup"><span data-stu-id="8fa40-115">The following example of a ResetPIN response shows a response to the ResetPIN request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8fa40-116">Код</span><span class="sxs-lookup"><span data-stu-id="8fa40-116">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="8fa40-117">См. также</span><span class="sxs-lookup"><span data-stu-id="8fa40-117">See also</span></span>



[<span data-ttu-id="8fa40-118">ResetPIN (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="8fa40-118">ResetPIN (UM web service)</span></span>](resetpin-um-web-service.md)
  
[<span data-ttu-id="8fa40-119">Ресетпинреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="8fa40-119">ResetPINResponse (UM web service)</span></span>](resetpinresponse-um-web-service.md)

