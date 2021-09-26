---
title: ExternalAudience
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: Элемент ExternalAudience задает или содержит значение, определяющие, кому отправляются внешние сообщения Office (OOF).
ms.openlocfilehash: da318bfcf4a43d880b86379364c6e40aa9861f83
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545141"
---
# <a name="externalaudience"></a>ExternalAudience

Элемент **ExternalAudience** задает или содержит значение, определяющие, кому отправляются внешние сообщения Office (OOF). 
  
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
|[UserOofSettings](useroofsettings.md) <br/> |Указывает параметры OOF.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Содержит параметры OOF.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|**Нет** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправившие сообщения пользователю, не получат внешнего ответа на сообщение OOF.  <br/> |
|**Известные** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправившие сообщения пользователю, получат внешний ответ на сообщение OOF только в том случае, если отправитель находится в списке контактов Exchange магазина пользователя.  <br/> |
|**Все** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, отправившие сообщения пользователю, получат внешний ответ на сообщение OOF.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент имеет тот же тип, что и [элемент AllowExternalOof.](allowexternaloof.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

Следующий пример запроса SetUserOofSettings задает включенную OoFState, задает внешнюю аудиторию для **всех,** задает продолжительность OOF до 10 дней и задает внутренние и внешние сообщения OOF.
  
```
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



[Операция GetUserOofSettings](getuseroofsettings-operation.md)
  
[Операция SetUserOofSettings](setuseroofsettings-operation.md)

