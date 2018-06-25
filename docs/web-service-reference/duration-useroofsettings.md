---
title: Продолжительность (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: Элемент длительность указывает продолжительность ожидания сообщения об отсутствии на состояние доступен, если элемент OofState задано значение запланировано.
ms.openlocfilehash: 62a5492372fd80173d58e965376b7c8c466825a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762235"
---
# <a name="duration-useroofsettings"></a>Продолжительность (UserOofSettings)

Элемент **длительность** указывает продолжительность ожидания сообщения об отсутствии на состояние доступен, если элемент [OofState](oofstate.md) задано значение **Запланировано**.
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 **Срок действия**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Время начала](starttime.md) <br/> |Представляет начало интервала времени задайте со статусом об отсутствии на работе. Этот элемент обязательный.  <br/> |
|[Время окончания](endtime.md) <br/> |Представляет окончания интервала времени задайте со статусом об отсутствии на работе. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Задает параметры об отсутствии на работе.  <br/><br/>Ниже приведен выражение XPath для этого элемента.<br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Содержит параметры об отсутствии на работе.<br/><br/>Ниже приведен выражение XPath для этого элемента.<br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[Нет на месте](outofoffice.md) <br/> |Определяет ответное сообщение об отсутствии на работе Office (OOF) и время для отправки сообщения ответа для почтового ящика.  <br/> |
   
## <a name="remarks"></a>Замечания

Тип **длительность** также является типом элементов [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [значение TimeWindow](timewindow.md)и [Нет на месте](outofoffice.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере [SetUserOofSettings операция](setuseroofsettings-operation.md) запроса задает [OofState](oofstate.md) **включено**, внешних и внутренних сообщений об отсутствии на работе и задает длительность об отсутствии на работе для 10 дней.
  
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
        <SetByLegacyClient>false</SetByLegacyClient>
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

- [Операция GetUserOofSettings](getuseroofsettings-operation.md)  
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

