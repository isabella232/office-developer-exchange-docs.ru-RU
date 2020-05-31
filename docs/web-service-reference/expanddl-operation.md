---
title: Операция ExpandDL
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: Операция ExpandDL предоставляет полное членство в списках рассылки.
ms.openlocfilehash: 4af6198ff15407b7fb71cdb4010ff6ce035460d0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353744"
---
# <a name="expanddl-operation"></a>Операция ExpandDL

Операция ExpandDL предоставляет полное членство в списках рассылки.
  
## <a name="using-the-expanddl-web-method"></a>Использование веб-метода ExpandDL

Операция ExpandDL использует веб-службу, размещенную в Exchange. asmx. Этот метод веб-службы принимает элемент [почтового ящика](mailbox.md) , который может содержать дочерний элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) для расширения общедоступного списка рассылки или дочернего элемента [ItemId](itemid.md) для расширения частного списка рассылки. 
  
Общедоступные списки рассылки можно развернуть с помощью одного из следующих компонентов:
  
1. Псевдоним списка рассылки
    
2. SMTP-адрес
    
3. X400
    
4. Х
    
5. Устаревший адрес Exchange
    
6. Имя списка рассылки
    
7. Отображаемое имя
    
> [!IMPORTANT]
> Отображаемые имена не являются уникальными. Несколько учетных записей могут иметь одно и то же отображаемое имя. 
  
## <a name="remarks"></a>Примечания

Рекурсивное расширение не поддерживается. В одном вызове можно развернуть только один список рассылки. Если критерию отвечает несколько списков рассылки, веб-служба сообщает об ошибке. Клиентское приложение может использовать разрешение неоднозначных имен, чтобы найти неоднозначные списки рассылки, а затем выбрать правильный адрес электронной почты требуемого списка рассылки в качестве параметра для [операции ExpandDL](expanddl-operation.md). Дополнительные сведения см. в разделе [Operation ResolveNames Operation](resolvenames-operation.md).
  
Общедоступные списки рассылки находятся в Active Directory. Можно использовать любую группу рассылки с поддержкой почты или динамическую группу рассылки. Группу не следует скрывать из списка адресов, а у каждого участника должен быть непустой адрес электронной почты. Членами этого списка рассылки могут быть пользователи и контакты, общедоступные папки и списки рассылки с поддержкой почты и динамические группы.
  
Частные списки рассылки находятся в папке "Контакты" в почтовом ящике пользователя. Частные списки рассылки не имеют адресов электронной почты, поэтому их идентификаторы элементов хранилища используются в запросе ExpandDL. Членами частного списка рассылки может быть любой пользователь с включенной поддержкой почты, контакты или списки рассылки из Active Directory, а также списки контактов или частных рассылки из папки "Контакты" пользователя.
  
Для контактов или частных списков рассылки в ответе возвращаются идентификаторы элементов. Этот параметр можно использовать для получения сведений о объекте или для расширения членства в частном списке рассылки.
  
## <a name="expanddl-private-distribution-list-request-example"></a>Пример запроса частного списка рассылки ExpandDL

### <a name="description"></a>Описание

В приведенном ниже примере запроса ExpandDL показано, как сформировать запрос на развертывание частного списка рассылки.
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExpandDL>
      <m:Mailbox>
       <t:EmailAddress>test</t:EmailAddress>
      </m:Mailbox>
    </m:ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Чтобы развернуть частный список рассылки, элемент [Mailbox](mailbox.md) будет содержать элемент [ItemId](itemid.md) , определяющий частный список рассылки в почтовом ящике пользователя. 
  
## <a name="expanddl-public-distribution-list-request-example"></a>Пример общего списка рассылки ExpandDL

### <a name="description"></a>Описание

В приведенном ниже примере запроса ExpandDL показано, как создать запрос для развертывания общедоступного списка рассылки. В этом примере показано использование отображаемого имени для развертывания списка рассылки.
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Ответ на этот запрос будет содержать элементы **почтовых ящиков** , которые определяют каждый почтовый ящик в списке рассылки. Если список рассылки находится в списке рассылки, для внедренного списка рассылки должно выполняться отдельное расширение списка рассылки. Если в списке рассылки нет участников или запрошенный список рассылки не существует, атрибут **респонсекласс** будет содержать значение Success. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [ExpandDL](expanddl.md)
    
- [Mailbox](mailbox.md)
    
- [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) используется для идентификации общедоступных списков рассылки. Элемент [ItemId](itemid.md) используется для идентификации частных списков рассылки. 
    
> [!NOTE]
> Схема, описывающая эти элементы, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Майкрософт Exchange Server 2007, на котором установлена роль сервера клиентского доступа. 
  
## <a name="successful-expanddl-response-example"></a>Пример успешного ответа ExpandDL

### <a name="description"></a>Описание

В приведенном ниже примере ответа ExpandDL показан ответ на запрос, описанный выше. Раскрытие списка рассылки содержит следующие сведения: 
  
- Количество членов списка рассылки, возвращаемых в ответе.
    
- Содержит ли ответ все члены списка рассылки.
    
- Имя почтового ящика.
    
- Адрес электронной почты почтового ящика.
    
- Тип маршрутизации для почтового ящика.
    
- Тип почтового ящика.
    
> [!NOTE]
> Имя списка рассылки не включается в ответ; Поэтому необходимо следить за именем в запросе. 
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DLExpansion TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Mailbox>
              <t:Name>Dan Park</t:Name>
              <t:EmailAddress>dpark@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Jeff Price</t:Name>
              <t:EmailAddress>jprice@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Tanja Plate</t:Name>
              <t:EmailAddress>tplate@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
          </m:DLExpansion>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [експанддлреспонсе](expanddlresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [експанддлреспонсемессаже](expanddlresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [длекспансион](dlexpansion.md)
    
- [Mailbox](mailbox.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md)
    
- [Раутингтипе (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
Чтобы найти другие параметры для ответного сообщения операции ExpandDL, изучите иерархию схемы. Начните с элемента [експанддлреспонсе](expanddlresponse.md) . 
  
## <a name="expanddl-error-response"></a>Ответ об ошибке ExpandDL

### <a name="description"></a>Описание

В следующем примере показан ответ об ошибке для запроса ExpandDL.
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Error">
          <m:MessageText>No results are found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [експанддлреспонсе](expanddlresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [експанддлреспонсемессаже](expanddlresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Чтобы найти другие параметры для ответного сообщения операции ExpandDL, изучите иерархию схемы. Начните с элемента [експанддлреспонсе](expanddlresponse.md) . 
  
## <a name="see-also"></a>См. также

- [Операция ResolveNames](resolvenames-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

