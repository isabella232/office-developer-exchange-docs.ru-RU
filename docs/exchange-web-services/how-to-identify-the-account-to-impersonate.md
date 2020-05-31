---
title: Идентификация учетной записи для олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Узнайте, как приложение службы использует EWS для идентификации пользователя, который будет олицетворять.
ms.openlocfilehash: 01c6ee797359c38c8539257003a2f110fdf253cf
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354297"
---
# <a name="identify-the-account-to-impersonate"></a>Идентификация учетной записи для олицетворения

Узнайте, как приложение службы использует EWS для идентификации пользователя, который будет олицетворять.
  
Приложение службы определяет учетную запись пользователя для олицетворения с помощью одного из следующих трех идентификаторов:
  
- Основной SMTP-адрес.
    
- Имя участника-пользователя (UPN).
    
- Идентификатор безопасности (SID).
    
Используемый идентификатор зависит от сведений, доступных в приложении.
  
## <a name="identifying-the-user-account-to-impersonate"></a>Идентификация учетной записи пользователя для олицетворения

Приложение может использовать управляемый API EWS или запросы SOAP для идентификации учетной записи пользователя, которая является олицетворенной. Управляемый API EWS использует свойство [ExchangeService. имперсонатедусерид](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) для идентификации олицетворяемого пользователя. В веб-службах EWS используется элемент [ексчанжеимперсонатион](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , как показано в следующем фрагменте XML. 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

В каждом из следующих разделов показано, как использовать один из идентификаторов. Пример кода олицетворения в действии представлен в статье [Добавление встреч с помощью олицетворения Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a>Использование SMTP-адреса электронной почты для идентификации учетной записи пользователя

SMTP-адрес электронной почты это основной адрес электронной почты, связанный с учетной записью пользователя.
  
В приложении управляемого API EWS вы указываете адрес электронной почты SMTP вместе со значением перечисления [коннектингидтипе. SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

В запросе SOAP в EWS элемент [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) содержит адрес электронной почты для учетной записи пользователя. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a>Определение учетной записи пользователя с помощью имени участника-пользователя

Имя участника-пользователя содержит полное доменное имя (FQDN) для расположения учетной записи пользователя. Он не обязательно является доменом почтовых ящиков пользователя. Для успешного выполнения поиска пользователя атрибут **усерпринЦипленаме** должен быть правильно задан для учетной записи пользователя в доменных службах Active Directory (AD DS). 
  
В приложении управляемого API EWS указывается имя участника-пользователя вместе со значением перечисления [коннектингидтипе. принЦипленаме](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

В запросе SOAP для EWS элемент [имя участника-(Коннектингсидтипе complexType) (EWS)](../web-service-reference/principalname.md) содержит имя участника-пользователя для учетной записи пользователя. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a>Определение учетной записи пользователя с помощью идентификатора безопасности (SID)

SID это идентификатор учетной записи, которая должна быть олицетворена в форме языка определения дескрипторов безопасности (SDDL).
  
В приложении управляемого API EWS укажите идентификатор безопасности вместе со значением перечисления [коннектингидтипе. SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

В запросе SOAP для EWS элемент [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) содержит идентификатор SID учетной записи пользователя. 
  
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
    
- [Добавление встреч с помощью олицетворения Exchange](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [Класс ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [ексчанжеимперсонатион](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

