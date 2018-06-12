---
title: Операция GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: Операция GetPasswordExpirationDate предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя.
ms.openlocfilehash: c57942c88b09a910e2d529a12ea279bb2da5d693
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762874"
---
# <a name="getpasswordexpirationdate-operation"></a>Операция GetPasswordExpirationDate

Операция **GetPasswordExpirationDate** предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя. 
  
Эта операция была введена в пакете обновления 1 (SP1) для Exchange Server 2010.
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>Заголовки SOAP GetPasswordExpirationDate операции

Операция **GetPasswordExpirationDate** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику. Это применимо к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет схему для операции запроса. Это применимо к запросу. Это применимо к запросу.  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>Пример запроса GetPasswordExpirationDate операции

### <a name="description"></a>Описание

В следующем примере запрос операции **GetPasswordExpirationDate** показано, как получить срок действия пароля для учетной записи электронной почты. 
  
### <a name="code"></a>Программа

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>Успешные операции ответа GetPasswordExpirationDate

В ответе используются следующие элементы:
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    

