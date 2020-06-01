---
title: Продолжительность (Усеруфсеттингс)
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
description: Элемент duration указывает длительность включения состояния "нет на месте" (отсутствие на работе), если для элемента Уфстате задано значение "запланировано".
ms.openlocfilehash: 0ba0f1ea7498781c0cccb072c7ea0fa05414764c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457300"
---
# <a name="duration-useroofsettings"></a>Продолжительность (Усеруфсеттингс)

Элемент **Duration** указывает длительность включения состояния "нет на месте" (отсутствие на работе), если для элемента [уфстате](oofstate.md) задано значение " **запланировано**".
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 **Duration**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Представляет начало временного интервала, установленного со статусом "отсутствие на работе". Этот элемент обязательный.  <br/> |
|[EndTime](endtime.md) <br/> |Представляет конец интервала времени, установленного со статусом "отсутствие на работе". Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[усеруфсеттингс](useroofsettings.md) <br/> |Задает параметры отсутствия на работе.  <br/><br/>Ниже приведено выражение XPath для этого элемента:<br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[уфсеттингс](oofsettings.md) <br/> |Содержит параметры отсутствия на работе.<br/><br/>Ниже приведено выражение XPath для этого элемента:<br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[аутофоффице](outofoffice.md) <br/> |Определяет ответ об отсутствии на работе (отсутствие на работе) и время для отправки ответного сообщения для почтового ящика.  <br/> |
   
## <a name="remarks"></a>Примечания

Тип **Duration** также является типом для элементов [детаиледсугжестионсвиндов](detailedsuggestionswindow.md), [TimeWindow](timewindow.md)и [аутофоффице](outofoffice.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

Следующий пример запроса [операции SetUserOofSettings](setuseroofsettings-operation.md) устанавливает для параметра [уфстате](oofstate.md) значение **Enabled**, внутренние и внешние сообщения об отсутствии на работе, а также задает длительность бездействия в течение 10 дней.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserOofSettings](getuseroofsettings-operation.md)  
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

