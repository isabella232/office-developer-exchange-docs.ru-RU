---
title: Операция ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: Операция ResolveNames разрешает неоднозначные адреса электронной почты и отображаемые имена.
ms.openlocfilehash: 51728addddd2bfb9d35b874ae8c11e83a4c8629b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468280"
---
# <a name="resolvenames-operation"></a>Операция ResolveNames

Операция **ResolveNames** разрешает неоднозначные адреса электронной почты и отображаемые имена. 
  
## <a name="using-the-resolvenames-operation"></a>Использование операции ResolveNames

Эту операцию можно использовать для проверки псевдонимов и разрешения отображаемых имен соответствующему пользователю почтового ящика. Если существуют неоднозначные имена, ответ операции **ResolveNames** предоставляет сведения о каждом пользователе почтового ящика, чтобы клиентское приложение могло разрешить имена. 
  
## <a name="remarks"></a>Примечания

Ответ ResolveNames возвращает не более 100 кандидатов. Возвращаемые кандидаты 100 являются первыми 100, которые встречаются в операции поиска.
  
Адреса электронной почты с предфиксированными типами маршрутизации, такими как SMTP или SIP, сохраняются в массиве с несколькими значениями. Операция **ResolveNames** выполняет частичное соответствие с каждым значением этого массива при добавлении типа маршрутизации в начале неизвестного имени, например "SIP:user1@Contoso.com". Если не указать тип маршрутизации, **ResolveNames** по умолчанию будет иметь тип маршрутизации SMTP, сопоставлять его с основным свойством SMTP-адреса, а не выполнять поиск по многозначному массиву. 
  
В одном запросе можно указать только одно неоднозначное имя. Сначала выполняется поиск в Active Directory, а затем выполняется поиск в папке контактов пользователя. Разрешенные записи из папки контактов пользователя имеют свойство **ItemId** , отличное от NULL, которое затем можно использовать в запросе GetItem. Если это идентификатор частного списка рассылки, его можно использовать в [операции ExpandDL](expanddl-operation.md). Если для атрибута **ретурнфуллконтактдата** задано **значение true**, то записи Active Directory, найденные с помощью операции **ResolveNames** , будут возвращать дополнительные свойства, описывающие [контакт](contact.md). Атрибут **ретурнфуллконтактдата** не влияет на данные, возвращаемые для контактов и частных списков рассылки из папки контактов пользователя. 
  
## <a name="resolvenames-request-example"></a>Пример запроса ResolveNames

### <a name="description"></a>Description

В приведенном ниже примере запроса **ResolveNames** показано, как разрешить запись пользователя.
  
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

Ответ на этот запрос возвратит все записи, начинающиеся с "Петр" или "MI". Возвращенные элементы представляют собой общедоступные почтовые ящики, общедоступные и частные списки рассылки, а также контакты.
  
> [!NOTE]
> Поиск осуществляется только по контактам из папки личных контактов по умолчанию. 
  
Ниже приведены возможные результаты запроса **ResolveNames** . 
  
- Ответы, которые не содержат разрешенных сущностей, возвращают значение атрибута **респонсекласс** , равное **Error**. Элемент **мессажетекст** будет содержать " **результаты не найдены**".
    
- Ответы, содержащие одну разрешенную сущность, возвращают значение атрибута **респонсекласс** , равное **Success**.
    
- Ответы, которые содержат несколько возможных сущностей, будут возвращать значение атрибута **респонсекласс** , равное **warning**. В этом случае сущность не может быть сопоставлена с уникальным идентификатором. Элемент **мессажетекст** будет содержать "несколько результатов поиска". 
    
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [ResolveNames](resolvenames.md)
    
- [унресолведентри](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>Пример успешного ответа операции ResolveNames

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос **ResolveNames** . 
  
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

### <a name="successful-resolvenames-response-elements"></a>Успешные элементы ответа ResolveNames

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [ресолвенамесреспонсе](resolvenamesresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [ресолвенамесреспонсемессаже](resolvenamesresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Авторешение](resolutionset.md)
    
- [Resolution](resolution.md)
    
- [Mailbox](mailbox.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md)
    
- [Раутингтипе (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [контакт](contact.md);
    
- [DisplayName (строка)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Запись (EmailAddress)](entry-emailaddress.md)
    
- [контактсаурце](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>Ответ об ошибке операции ResolveNames

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке для запроса **ResolveNames** . Ошибка возникает при попытке разрешить имя, которое не удается разрешить. 
  
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

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [ресолвенамесреспонсе](resolvenamesresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [ресолвенамесреспонсемессаже](resolvenamesresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также



[Операция ExpandDL](expanddl-operation.md)


[Использование разрешения имен](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

