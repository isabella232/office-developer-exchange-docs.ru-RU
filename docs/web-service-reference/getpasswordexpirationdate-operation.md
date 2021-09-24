---
title: Операция GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: Операция GetPasswordExpirationDate предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя.
ms.openlocfilehash: 07928fd3e6fca410a292d6cd74f1240d8e81c42f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524240"
---
# <a name="getpasswordexpirationdate-operation"></a>Операция GetPasswordExpirationDate

Операция **GetPasswordExpirationDate** предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя. 
  
Эта операция была введена в Exchange Server 2010 Пакет обновления 1 (SP1).
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>Заголовки операции SOAP GetPasswordExpirationDate

В **операции GetPasswordExpirationDate** можно использовать заголовки SOAP, перечисленные в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет культуру, определяемую в RFC 3066 , "Теги для идентификации языков", которая будет использоваться для доступа к почтовому ящику. Это применимо к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет схему запроса на операцию. Это применимо к запросу. Это применимо к запросу.  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>Пример запроса на операцию GetPasswordExpirationDate

### <a name="description"></a>Описание

В следующем примере запроса **операции GetPasswordExpirationDate** показано, как получить дату истечения срока действия пароля для учетной записи электронной почты. 
  
### <a name="code"></a>Код

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>Успешный ответ операции GetPasswordExpirationDate

В ответе используются следующие элементы:
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    

