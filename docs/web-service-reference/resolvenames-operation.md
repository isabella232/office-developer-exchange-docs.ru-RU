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
description: Адреса ResolveNames операция переносов неоднозначные электронной почты и отображаемые имена.
ms.openlocfilehash: 8443cf834dfdf104daeaaa92fdee3742c3fa3719
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835162"
---
# <a name="resolvenames-operation"></a>Операция ResolveNames

Адреса **ResolveNames** операция переносов неоднозначные электронной почты и отображаемые имена. 
  
## <a name="using-the-resolvenames-operation"></a>С помощью операции ResolveNames

Эту операцию можно использовать для проверки псевдонимы и разрешения отображаемые имена в соответствующий почтовый ящик пользователя. Если существует неоднозначные имена ответа операции **ResolveNames** сведения о каждого почтового ящика пользователя, чтобы клиентское приложение может разрешения имен. 
  
## <a name="remarks"></a>Замечания

Ответ ResolveNames возвращает не более 100 кандидатов. 100 кандидатов, возвращенных — это первый 100 обнаружения в операции поиска.
  
Адреса электронной почты с с префиксами типов маршрутизации, например smtp или sip, сохраняются в нескольких значений массива. Операция **ResolveNames** выполняет частичное соответствие каждого значения этого массива, при добавлении типа маршрутизации в начале неизвестное имя, например «sip:User1@Contoso.com». Если не указать тип маршрутизации, **ResolveNames** по умолчанию для типа маршрутизации smtp, соответствует свойству основной адрес smtp и поиск нескольких значений массива. 
  
В одном запросе можно указать только один неоднозначное имя. Сначала выполняется поиск Active Directory, а затем осуществляется в папке контактов пользователя. Записей в папке контактов пользователя имеют свойство **ItemId** ненулевое, которую можно использовать в запросе GetItem. Если идентификатор списка рассылки частный, его можно использовать в рамках одной [операции ExpandDL](expanddl-operation.md). Если атрибут **ReturnFullContactData** имеет значение **true**, найдено Active Directory с помощью операции **ResolveNames** возвращает дополнительные свойства, описывающие [контакт](contact.md). Атрибут **ReturnFullContactData** не влияет на данные, возвращаемые для контактов и частных списки рассылки из папки контактов пользователя. 
  
## <a name="resolvenames-request-example"></a>Пример запроса ResolveNames

### <a name="description"></a>Описание

В следующем примере запрос **ResolveNames** показано, как разрешить запись пользователя.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Ответ на этот запрос будет возвращать все записи, начинающиеся с «Петр» или «Mi». Возвращенные элементы, общих почтовых ящиков, списки рассылки общедоступных и частных и контакты.
  
> [!NOTE]
> Поиск осуществляется только контактов в папке личных контактов по умолчанию. 
  
Ниже приведены возможные результаты запроса **ResolveNames** . 
  
- Ответы, которые не содержат разрешения сущности возвращает значение атрибута **ResponseClass** равно **ошибки**. Элемент **MessageText** будет содержать « **Нет результатов**».
    
- Ответы, которые содержат одного объекта разрешения возвращает значение атрибута **ResponseClass** равно **успеха**.
    
- Ответы, которые содержат несколько возможных сущностей возвращает значение атрибута **ResponseClass** равно **предупреждения**. В этом случае сущность не удалось разрешить уникальное удостоверение. Элемент **MessageText** будет содержать «находятся несколько результатов». 
    
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>Пример ответа операция успешно ResolveNames

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **ResolveNames** . 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-resolvenames-response-elements"></a>Элементы ответов успешно ResolveNames

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [Решение](resolution.md)
    
- [Mailbox](mailbox.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Контакт](contact.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Запись (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>Ошибка операции ResolveNames ответа

### <a name="description"></a>Описание

В следующем примере показано ошибочный ответ на запрос **ResolveNames** . Ошибки, возникающие при попытке определить имя, которое не может быть разрешен. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также



[Операция ExpandDL](expanddl-operation.md)


[С помощью разрешения имен](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

