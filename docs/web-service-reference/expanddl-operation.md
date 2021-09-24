---
title: Операция ExpandDL
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: Операция ExpandDL предоставляет полное членство в списках рассылки.
ms.openlocfilehash: 9878ecff0eeee1ef386c7bb26a092eec47f471de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513782"
---
# <a name="expanddl-operation"></a>Операция ExpandDL

Операция ExpandDL предоставляет полное членство в списках рассылки.
  
## <a name="using-the-expanddl-web-method"></a>Использование веб-метода ExpandDL

Операция ExpandDL использует веб-службу, расположенную в Exchange.asmx. Этот метод веб-службы принимает элемент почтовых ящиков, который может содержать детский элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) для расширения общего списка рассылки или детский элемент [ItemId](itemid.md) для расширения частного списка рассылки. [](mailbox.md) 
  
Общедоступные списки рассылки можно расширить с помощью одного из следующих:
  
1. Псевдоним списка рассылки
    
2. SMTP-адрес
    
3. X400
    
4. X500
    
5. Exchange Устаревший адрес
    
6. Имя списка рассылки
    
7. Имя отображения
    
> [!IMPORTANT]
> Имена отображения не являются уникальными. Несколько учетных записей могут иметь одно и то же имя отображения. 
  
## <a name="remarks"></a>Заметки

Рекурсивное расширение не поддерживается. В одном вызове можно расширить только один список рассылки. Если несколько списков рассылки соответствуют критериям, веб-служба сообщает об ошибке. Клиентские приложения могут использовать неоднозначное разрешение имен (ANR), чтобы найти неоднозначные списки рассылки, а затем выбрать правильный адрес электронной почты необходимого списка рассылки в качестве параметра для операции [ExpandDL](expanddl-operation.md). Дополнительные сведения см. в операции [ResolveNames.](resolvenames-operation.md)
  
Общедоступные списки рассылки расположены в Active Directory. Они могут быть любой группой рассылки с поддержкой почты или динамической рассылкой. Группа не должна быть скрыта из списка адресов, и каждый член должен иметь непустый адрес электронной почты. Членами списка рассылки могут быть пользователи и контакты с поддержкой почты, общедоступные папки, списки рассылки с поддержкой почты и динамические группы.
  
Частные списки рассылки находятся в папке Контакты почтового ящика пользователя. Частные списки рассылки не имеют адресов электронной почты, поэтому идентификаторы элементов магазина используются в запросе ExpandDL. Членами частного списка рассылки могут быть любой пользователь с включенной почтой, контакты или списки рассылки из Active Directory, а также контакты или частные списки рассылки из папки контакты пользователя.
  
Для контактов или частных списков рассылки идентификаторы элементов возвращаются в ответе. Это можно использовать для получения сведений об объекте или расширения членства в частном списке рассылки.
  
## <a name="expanddl-private-distribution-list-request-example"></a>Пример запроса на расширенный частный список рассылки

### <a name="description"></a>Описание

В следующем примере запроса ExpandDL показано, как сформировать запрос на расширение частного списка рассылки.
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

### <a name="comments"></a>Комментарии

Чтобы расширить частный список рассылки, элемент [почтовых](mailbox.md) ящиков будет содержать элемент [ItemId,](itemid.md) который идентифицирует частный список рассылки в почтовом ящике пользователя. 
  
## <a name="expanddl-public-distribution-list-request-example"></a>Пример запроса на расширенный список общедоступных рассылки

### <a name="description"></a>Описание

В следующем примере запроса ExpandDL показано, как сформировать запрос на расширение общего списка рассылки. В примере показано использование имени отображения для расширения списка рассылки.
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Ответ на этот запрос будет содержать **элементы почтовых ящиков,** идентифицирующие каждый почтовый ящик в списке рассылки. Если список рассылки содержится в списке рассылки, в встроенном списке рассылки необходимо выполнить отдельное расширение списка рассылки. Если в списке рассылки нет участников или отсутствует запрашиваемая рассылка, атрибут **ResponseClass** будет содержать значение, равное успеху. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [ExpandDL](expanddl.md)
    
- [Mailbox](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) используется для определения общедоступных списков рассылки. Элемент [ItemId](itemid.md) используется для определения частных списков рассылки. 
    
> [!NOTE]
> Схема, описываемая этими элементами, расположена в виртуальном каталоге EWS компьютера под управлением MicrosoftExchange Server 2007, где установлена роль сервера клиентского доступа. 
  
## <a name="successful-expanddl-response-example"></a>Пример успешного ответа ExpandDL

### <a name="description"></a>Описание

В следующем примере ответа ExpandDL показан ответ на описанный выше запрос. Расширение списка рассылки описывает следующее: 
  
- Количество участников списка рассылки, возвращаемого в ответе.
    
- Содержит ли ответ все участники списка рассылки.
    
- Имя почтового ящика.
    
- Адрес электронной почты почтового ящика.
    
- Тип маршрутивки для почтового ящика.
    
- Тип почтового ящика.
    
> [!NOTE]
> Имя списка рассылки не включено в ответ; Поэтому необходимо отслеживать имя из запроса. 
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
Чтобы найти другие параметры ответного сообщения операции ExpandDL, ознакомьтесь с иерархией схемы. Начните с [элемента ExpandDLResponse.](expanddlresponse.md) 
  
## <a name="expanddl-error-response"></a>Ответ на ошибки ExpandDL

### <a name="description"></a>Описание

В следующем примере показан ответ на ошибку на запрос ExpandDL.
  
### <a name="code"></a>Код

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>Элементы ответа на ошибки

В ответе на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Чтобы найти другие параметры ответного сообщения операции ExpandDL, ознакомьтесь с иерархией схемы. Начните с [элемента ExpandDLResponse.](expanddlresponse.md) 
  
## <a name="see-also"></a>См. также

- [Операция ResolveNames](resolvenames-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

