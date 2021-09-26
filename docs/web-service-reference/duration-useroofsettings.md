---
title: Duration (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: Элемент Duration указывает продолжительность включения состояния вне офиса (OOF), если элемент OofState задан в Scheduled.
ms.openlocfilehash: cb6529bfe3799ff41550d7fe3ce2c79b8a4197e2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544159"
---
# <a name="duration-useroofsettings"></a>Duration (UserOofSettings)

Элемент **Duration** указывает продолжительность включения состояния вне офиса (OOF), если элемент [OofState](oofstate.md) задан **в Scheduled**.
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 **Duration**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Представляет начало набора времени со статусом OOF. Этот элемент обязательный.  <br/> |
|[EndTime](endtime.md) <br/> |Представляет конец набора времени со статусом OOF. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Указывает параметры OOF.  <br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Содержит параметры OOF.<br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[OutOfOffice](outofoffice.md) <br/> |Определяет сообщение ответа Office (OOF) и продолжительность отправки сообщения ответа для почтового ящика.  <br/> |
   
## <a name="remarks"></a>Заметки

Тип **Duration** — это также тип элементов [DetailedSuggestionsWindow,](detailedsuggestionswindow.md) [TimeWindow](timewindow.md)и [OutOfOffice.](outofoffice.md) 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

Следующий пример запроса операции [SetUserOofSettings](setuseroofsettings-operation.md) задает [OofState](oofstate.md) для включения **внутренних** и внешних сообщений OOF и задает продолжительность OOF в течение 10 дней.
  
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
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserOofSettings](getuseroofsettings-operation.md)  
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

