---
title: Идентификация учетной записи для олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Узнайте, как приложения-службы с помощью веб-служб Exchange для идентификации пользователя для олицетворения.
ms.openlocfilehash: 78df4b511a9947d4d815b2802a53ab178b14622b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761015"
---
# <a name="identify-the-account-to-impersonate"></a>Идентификация учетной записи для олицетворения

Узнайте, как приложения-службы с помощью веб-служб Exchange для идентификации пользователя для олицетворения.
  
Приложение службы указываются учетной записи пользователя для олицетворения, используя один из следующих трех идентификаторов:
  
- Основной SMTP-адрес.
    
- Имя участника пользователя (UPN).
    
- Идентификатор безопасности (SID).
    
Идентификатор, который можно использовать зависит от того, конечно, сведения, в приложении есть недоступны.
  
## <a name="identifying-the-user-account-to-impersonate"></a>Определение учетной записи пользователя для олицетворения

Приложение может использовать управляемый API EWS или веб-служб Exchange SOAP запросов для идентификации учетной записи пользователя, который олицетворении. Управляемый API EWS использует свойство [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) для идентификации олицетворения пользователя. Веб-служб Exchange используется элемент [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , как показано в следующем фрагменте XML. 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

Каждой из следующих разделах показано, как использовать один из идентификаторов. Пример идентификатор олицетворения в действии в разделе [Добавление встреч с помощью олицетворения Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a>Используйте адрес электронной почты SMTP для учетной записи пользователя

Адрес электронной почты SMTP — это основной адрес электронной почты, связанный с учетной записью пользователя.
  
В приложении, управляемый API веб-служб Exchange укажите адрес электронной почты SMTP, а также значение перечисления [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

В запрос SOAP веб-служб Exchange элемент [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) содержит адрес электронной почты для учетной записи пользователя. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a>Используйте имя участника-пользователя для учетной записи пользователя

Имя участника-пользователя содержит полное доменное имя (FQDN) для расположения учетной записи пользователя. Это не обязательно домен почтового ящика пользователя. Атрибут **UserPrincipleName** необходимо правильно задать для учетной записи пользователя в доменных службах Active Directory (AD DS) для успешного завершения поиска пользователя. 
  
В приложении, управляемый API веб-служб Exchange укажите имя участника-пользователя, а также значение перечисления [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

В запрос SOAP веб-служб Exchange [элемент PrincipalName (ConnectingSIDType complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) элемент содержит имя участника-пользователя для учетной записи пользователя. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a>Используйте идентификатор безопасности для учетной записи пользователя

Идентификатор безопасности — это идентификатор учетной записи для олицетворения в виде языке SDDL определения дескриптора безопасности.
  
В приложении, управляемый API веб-служб Exchange укажите идентификатор безопасности, а также значение перечисления [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

В запрос SOAP веб-служб Exchange элемент [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) содержит идентификатор безопасности для учетной записи пользователя. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a>См. также


- [Олицетворение и EWS в Exchange](impersonation-and-ews-in-exchange.md)
    
- [Добавление встреч с использованием олицетворения Exchange](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [Класс ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

