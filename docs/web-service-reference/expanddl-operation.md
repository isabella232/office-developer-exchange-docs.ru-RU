---
title: Операция ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: Операция ExpandDL предоставляет полного контроля членства списков рассылки.
ms.openlocfilehash: e4654120881f81a79358e0e7c0ab016f94db3288
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762437"
---
# <a name="expanddl-operation"></a>Операция ExpandDL

Операция ExpandDL предоставляет полного контроля членства списков рассылки.
  
## <a name="using-the-expanddl-web-method"></a>С помощью ExpandDL веб-метода

Операция ExpandDL использует веб-службы, размещенной в Exchange.asmx. Этот метод веб-службы принимает элемент [почтового ящика](mailbox.md) , который может содержать дочерний элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) расширения открытый список рассылки либо [ItemId](itemid.md) дочернего элемента для расширения частной список рассылки. 
  
Открытые списки рассылки могут быть развернуты с помощью одного из следующих:
  
1. Псевдоним списка рассылки
    
2. Адрес Simple Mail Transfer Protocol (SMTP)
    
3. X400
    
4. X500
    
5. Адрес прежних версий Exchange
    
6. Имя списка рассылки
    
7. Отображаемое имя
    
> [!IMPORTANT]
> Отображаемые имена не являются уникальными. Несколько учетных записей могут совместно использовать же отображаемое имя. 
  
## <a name="remarks"></a>Замечания

Расширения рекурсивный не поддерживается. Можно развернуть только один список, в одном вызове. Если более одного списка рассылки соответствующие критериям, веб-службы отчетов об ошибке. Клиентское приложение может использовать разрешения неоднозначных имен (ANR) для поиска неоднозначные рассылки список, а затем выбрать правильный адрес электронной почты из списка рассылки необходимые как параметр [ExpandDL операции](expanddl-operation.md). Для получения дополнительных сведений см [ResolveNames операции](resolvenames-operation.md).
  
Открытые списки рассылки, находятся в Active Directory. Они могут быть любая группа рассылки с включенной поддержкой почты или динамической. Группы не должен быть скрыт из списка адресов и каждый элемент должен иметь адрес электронной почты не пуста. Члены списка рассылки могут быть пользователи с включенной поддержкой почты и контакты, общих папок и списков рассылки с включенной поддержкой почты и динамические группы.
  
Частные списки рассылки, находятся в папке «Контакты» из почтового ящика пользователя. Частные списки рассылки не имеют адреса электронной почты, поэтому их идентификаторы элемента хранилища используются в запросе ExpandDL. Члены списка рассылки закрытый может быть любого пользователя с включенной поддержкой почты, контакты или списки рассылки из службы каталогов Active Directory или контактов или частные списки рассылки из папки Контакты.
  
Для контактов или частные списки рассылки идентификаторы элементов возвращаемого в ответе. Можно использовать для получения сведений об объекте или чтобы развернуть членство в списке рассылки закрытый.
  
## <a name="expanddl-private-distribution-list-request-example"></a>Пример запроса ExpandDL Private списка рассылки

### <a name="description"></a>Описание

В следующем примере запрос ExpandDL показано, как для формирования запроса разверните список рассылки закрытый.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:ItemId Id="xASUAd==" ChangeKey="AAts0Q=="/>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Разверните список рассылки закрытый элемент [почтового ящика](mailbox.md) будет содержать элемент [ItemId](itemid.md) , определяющий список рассылки закрытый в почтовом ящике пользователя. 
  
## <a name="expanddl-public-distribution-list-request-example"></a>Пример запроса ExpandDL общедоступных списка рассылки

### <a name="description"></a>Описание

В следующем примере запрос ExpandDL показано, как для формирования запроса, чтобы развернуть открытый список рассылки. В примере показано использование отображаемое имя, чтобы развернуть список рассылки.
  
### <a name="code"></a>Программа

```XML
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

### <a name="comments"></a>Комментарии

Ответ на этот запрос будет содержать элементы **почтового ящика** , чтобы указать каждого почтового ящика в списке рассылки. Если список рассылки содержится в список рассылки, раскрытие списков рассылки отдельные необходимо выполнить на список внедренных рассылки. Если этот список рассылки не имеет членов или список рассылки запрошенные не существует, атрибут **ResponseClass** будет содержать значение, равное успеха. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [ExpandDL](expanddl.md)
    
- [Mailbox](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) используется для идентификации открытые списки рассылки. Элемент [ItemId](itemid.md) используется для идентификации частные списки рассылки. 
    
> [!NOTE]
> Схема, описывающая эти элементы находится в виртуальном каталоге EWS компьютера, на котором работает MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа. 
  
## <a name="successful-expanddl-response-example"></a>Пример успешного ответа ExpandDL

### <a name="description"></a>Описание

В следующем примере ответа ExpandDL показано ответа на запрос, описанных выше. Раскрытие списка рассылки описываются следующие: 
  
- Количество членов списка рассылки, возвращаемого в ответе.
    
- Содержит ли ответ всех членов списка рассылки.
    
- Имя почтового ящика.
    
- Адрес электронной почты для почтового ящика.
    
- Тип маршрутизации для почтового ящика.
    
- Тип почтового ящика.
    
> [!NOTE]
> Имя списка рассылки не включенных в ответ; Таким образом вы должны отслеживать связи имя запроса. 
  
### <a name="code"></a>Программа

```XML
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

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [DLExpansion](dlexpansion.md)
    
- [Mailbox](mailbox.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
Чтобы найти другие параметры в сообщении ответа операция ExpandDL, изучите иерархия схемы. Запустите в элементе [ExpandDLResponse](expanddlresponse.md) . 
  
## <a name="expanddl-error-response"></a>Ошибка ExpandDL ответа

### <a name="description"></a>Описание

В следующем примере показано ошибочный ответ на запрос ExpandDL.
  
### <a name="code"></a>Программа

```XML
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

### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Чтобы найти другие параметры в сообщении ответа операция ExpandDL, изучите иерархия схемы. Запустите в элементе [ExpandDLResponse](expanddlresponse.md) . 
  
## <a name="see-also"></a>См. также

- [Операция ResolveNames](resolvenames-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

