---
title: Операция ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: Операция ResolveNames устраняет неоднозначные адреса электронной почты и отображает имена.
ms.openlocfilehash: f5ab0e3ee23cc085d8aa425c6eeb0ac7c392b9bb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509450"
---
# <a name="resolvenames-operation"></a>Операция ResolveNames

Операция **ResolveNames** устраняет неоднозначные адреса электронной почты и отображает имена. 
  
## <a name="using-the-resolvenames-operation"></a>Использование операции ResolveNames

Эта операция может использоваться для проверки псевдонимов и разрешения имен отображения соответствующему пользователю почтового ящика. Если существуют неоднозначные имена, ответ операции **ResolveNames** предоставляет сведения о каждом пользователе почтового ящика, чтобы клиентские приложения могли разрешить имена. 
  
## <a name="remarks"></a>Заметки

Ответ ResolveNames возвращает максимум 100 кандидатов. Возвращаемые 100 кандидатов являются первыми 100, которые встречаются в операции lookup.
  
Адреса электронной почты с префиксными типами маршрутиза, такими как smtp или sip, сохраняются в многоценном массиве. Операция **ResolveNames** выполняет частичное соответствие каждому значению этого массива при добавлении типа маршрутизов в начале неурегулированного имени, например "sip:User1@Contoso.com". Если не указать тип маршрутизования, **ResolveNames** по умолчанию будет соответствовать типу smtp маршрутики, соизменить его с основным свойством адресов smtp, а не искать многоценный массив. 
  
Только одно неоднозначное имя может быть указано в одном запросе. Сначала ведется поиск active Directory, а затем поиск в папке контактов пользователя. Разрешенные записи из контактной папки пользователя имеют свойство Non-null **ItemId,** которое затем можно использовать в запросе GetItem. Если это ID частного списка рассылки, его можно использовать в операции [ExpandDL.](expanddl-operation.md) Если атрибут **ReturnFullContactData** настроен на верность, то записи Active Directory, найденные с помощью операции **ResolveNames,** возвращают дополнительные свойства, описывая [контакт.](contact.md) Атрибут **ReturnFullContactData** не влияет на данные, возвращаемые для контактов и частные списки рассылки из папки контактов пользователя. 
  
## <a name="resolvenames-request-example"></a>Пример запроса resolveNames

### <a name="description"></a>Описание

В следующем примере **запроса ResolveNames** показано, как разрешить запись Пользователя.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Ответ на этот запрос возвращает все записи, которые начинаются с "Jo" или "Mi". Возвращенные элементы — это общедоступные почтовые ящики, общедоступные и частные списки рассылки и контакты.
  
> [!NOTE]
> Поиск ведутся только с контактами в папке личных контактов по умолчанию. 
  
Ниже возможен результат запроса **ResolveNames:** 
  
- Ответы, не содержащие разрешенную сущность, возвращают значение **атрибута ResponseClass,** равное **ошибке.** Элемент **MessageText будет** содержать **"Результатов не обнаружено".**
    
- Ответы, содержащие одну разрешенную сущность, возвращают значение **атрибута ResponseClass,** равное **успеху.**
    
- Ответы, содержащие несколько возможных сущностями, возвращают значение **атрибута ResponseClass,** равное **предупреждению.** В этом случае сущность не может быть разрешена к уникальному удостоверению. Элемент **MessageText будет** содержать "Найдено несколько результатов". 
    
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>Пример успешного ответа на операции ResolveNames

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос **ResolveNames.** 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>User2</t:Name>
                <t:EmailAddress>User2@example.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>User2</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:User2@example.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-resolvenames-response-elements"></a>Элементы успешного ответа ResolveNames

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [Решение](resolution.md)
    
- [Mailbox](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Contact](contact.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entry (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>Ответ на ошибку операции ResolveNames

### <a name="description"></a>Описание

В следующем примере показан ответ на ошибку **запроса ResolveNames.** Ошибка вызвана попыткой устранить имя, которое невозможно устранить. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа на ошибки

В ответе на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также



[Операция ExpandDL](expanddl-operation.md)


[Использование разрешения имен](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

