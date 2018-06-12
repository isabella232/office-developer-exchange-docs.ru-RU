---
title: ExternalAudience
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: Элемент ExternalAudience устанавливает или содержит значение, определяющее, которому отправляются внешних сообщений об отсутствии на работе Office (отсутствие на работе).
ms.openlocfilehash: 836b0f6a5140a37e1584f571cb8e26534fe7a25f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762484"
---
# <a name="externalaudience"></a>ExternalAudience

Элемент **ExternalAudience** устанавливает или содержит значение, определяющее, которому отправляются внешних сообщений об отсутствии на работе Office (отсутствие на работе). 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Задает параметры об отсутствии на работе.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Содержит параметры об отсутствии на работе.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|**None** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправлять сообщения пользователю, не получат внешнего ответа сообщение об отсутствии на работе.  <br/> |
|**Известные** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, которые отправляют сообщения, чтобы пользователь получит только внешние ответа сообщение об отсутствии на работе Если отправитель входит в Exchange пользователя хранить список контактов.  <br/> |
|**All** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправлять сообщения для пользователя будет получать внешние ответа сообщение об отсутствии на работе.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент использует совместно с типом элемента [AllowExternalOof](allowexternaloof.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

Приведенный ниже запрос SetUserOofSettings задает OoFState **включена**, наборы данных для **всех**внешних аудитории, задает длительность об отсутствии на работе на 10 дней и задает внешних и внутренних сообщений об отсутствии на работе.
  
```
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



[Операция GetUserOofSettings](getuseroofsettings-operation.md)
  
[Операция SetUserOofSettings](setuseroofsettings-operation.md)

