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
ms.openlocfilehash: 4184092cf98161e4c2f74446cef5439722ae71a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457895"
---
# <a name="getpasswordexpirationdate-operation"></a>Операция GetPasswordExpirationDate

Операция **GetPasswordExpirationDate** предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя. 
  
Эта операция появилась в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>Заголовки SOAP операции GetPasswordExpirationDate

Операция **GetPasswordExpirationDate** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Это относится к запросу.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет схему запроса операции. Это относится к запросу. Это относится к запросу.  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>Пример запроса операции GetPasswordExpirationDate

### <a name="description"></a>Описание

В приведенном ниже примере запроса операции **GetPasswordExpirationDate** показано, как получить срок действия пароля для учетной записи электронной почты. 
  
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

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [маилбокссмтпаддресс](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>Успешный отклик операции GetPasswordExpirationDate

В отклике используются следующие элементы:
  
- [жетпассвордекспиратиондатереспонсе](getpasswordexpirationdateresponse.md)
    
- [пассвордекспиратиондате](passwordexpirationdate.md)
    

