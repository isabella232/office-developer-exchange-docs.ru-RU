---
title: Операция ResetPIN (веб-служба единой системы обмена СООБЩЕНИЯМИ)
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
description: Операция ResetPIN изменений ПИН-кода (телефонного интерфейса пароль) в новое значение в случайном порядке.
ms.openlocfilehash: e6417b86ce17c0d34fe857cf1209a18972cbef63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835146"
---
# <a name="resetpin-operation-um-web-service"></a><span data-ttu-id="1551c-103">Операция ResetPIN (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="1551c-103">ResetPIN operation (UM web service)</span></span>

<span data-ttu-id="1551c-104">Операция ResetPIN изменений ПИН-кода (телефонного интерфейса пароль) в новое значение в случайном порядке.</span><span class="sxs-lookup"><span data-stu-id="1551c-104">The ResetPIN operation changes the PIN (TUI password) to a new random value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1551c-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="1551c-105">Remarks</span></span>

<span data-ttu-id="1551c-106">Операция ResetPIN создает новый ПИН-код на основе политик ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="1551c-106">The ResetPIN operation creates a new PIN based on the PIN policies.</span></span> <span data-ttu-id="1551c-107">Если операция выполнена успешно, в почтовый ящик пользователя, отправляется сообщение электронной почты, содержащее новый ПИН-код.</span><span class="sxs-lookup"><span data-stu-id="1551c-107">If the operation is successful, an e-mail message that contains the new PIN is sent to the mailbox of the user.</span></span> <span data-ttu-id="1551c-108">В случае сбоя операции, он будет исключение, который содержит сведения о сбое.</span><span class="sxs-lookup"><span data-stu-id="1551c-108">If the operation fails, it will throw an exception that contains information about the failure.</span></span>
  
## <a name="resetpin-request-example"></a><span data-ttu-id="1551c-109">Пример запроса ResetPIN</span><span class="sxs-lookup"><span data-stu-id="1551c-109">ResetPIN request example</span></span>

### <a name="description"></a><span data-ttu-id="1551c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1551c-110">Description</span></span>

<span data-ttu-id="1551c-111">В следующем примере запрос ResetPIN показано, как для формирования запроса для сброса ПИН-код для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1551c-111">The following example of a ResetPIN request shows how to form a request to reset the PIN for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="1551c-112">Программа</span><span class="sxs-lookup"><span data-stu-id="1551c-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a><span data-ttu-id="1551c-113">Пример успешного ответа ResetPIN</span><span class="sxs-lookup"><span data-stu-id="1551c-113">Successful ResetPIN response example</span></span>

### <a name="description"></a><span data-ttu-id="1551c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="1551c-114">Description</span></span>

<span data-ttu-id="1551c-115">В следующем примере ответа ResetPIN показано ответа на запрос ResetPIN.</span><span class="sxs-lookup"><span data-stu-id="1551c-115">The following example of a ResetPIN response shows a response to the ResetPIN request.</span></span>
  
### <a name="code"></a><span data-ttu-id="1551c-116">Программа</span><span class="sxs-lookup"><span data-stu-id="1551c-116">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="1551c-117">См. также</span><span class="sxs-lookup"><span data-stu-id="1551c-117">See also</span></span>



[<span data-ttu-id="1551c-118">ResetPIN (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="1551c-118">ResetPIN (UM web service)</span></span>](resetpin-um-web-service.md)
  
[<span data-ttu-id="1551c-119">ResetPINResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="1551c-119">ResetPINResponse (UM web service)</span></span>](resetpinresponse-um-web-service.md)

