---
title: Сообщение (доступность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 1eec24dd-c981-41f4-a2f0-c51d43f1d7c0
description: Элемент сообщение содержит ожидания ответа Office (OOF).
ms.openlocfilehash: 9facd04767fdcc0fd9dfd84fc6badb1a7633d2b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834452"
---
# <a name="message-availability"></a>Сообщение (доступность)

Элемент **сообщение** содержит ожидания ответа Office (OOF). 
  
```xml
<Message/> 
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[InternalReply](internalreply.md) <br/> | Содержит сообщения об отсутствии на работе, для других пользователей в домен отправителя. <br/> <br/>  Ниже приведены возможные выражения XPath для этого элемента. <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/InternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/InternalReply` <br/> |
|[ExternalReply](externalreply.md) <br/> | Содержит сообщение об отсутствии на работе, которое отправляется адресам за пределами домена отправителя.  <br/> <br/> Ниже приведены возможные выражения XPath для этого элемента.  <br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/ExternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/ExternalReply` <br/> |
|[ReplyBody](replybody.md) <br/> |Содержит сообщение об отсутствии на работе и язык, используемый для сообщения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение необходимо задать для сообщения об отсутствии на работе.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере [SetUserOofSettings операция](setuseroofsettings-operation.md) запроса задает [OofState](oofstate.md) **включена**, задает длительность об отсутствии на работе на 10 дней и задает внешних и внутренних сообщений об отсутствии на работе.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция SetUserOofSettings](setuseroofsettings-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

