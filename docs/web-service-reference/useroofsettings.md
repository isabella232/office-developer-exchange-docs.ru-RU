---
title: UserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserOofSettings
api_type:
- schema
ms.assetid: 0a95ca63-660e-4cc0-82e4-3f74fb4ae21c
description: Элемент UserOofSettings указывает параметры об отсутствии на работе Office (отсутствие на работе).
ms.openlocfilehash: a035fd89387ece632d83f5f72a564e4896bc6753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840433"
---
# <a name="useroofsettings"></a>UserOofSettings

Элемент **UserOofSettings** указывает параметры об отсутствии на работе Office (отсутствие на работе). 
  
[SetUserOofSettingsRequest](setuseroofsettingsrequest.md)
  
[UserOofSettings](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 **UserOofSettings**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Задает состояние пользователя об отсутствии на работе.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Задает или содержит значение, определяющее, которому отправляются внешних сообщений об отсутствии на работе.  <br/> |
|[Продолжительность (UserOofSettings)](duration-useroofsettings.md) <br/> |Указывает, во время выполнения, для которого включен состояние об отсутствии на работе, если элемент [OofState](oofstate.md) задано значение **Запланировано**. Если элемент [OofState](oofstate.md) — это значение **включено** или **отключено**, значение этого элемента игнорируется.  <br/> |
|[InternalReply](internalreply.md) <br/> |Содержит ответа об отсутствии на работе, для других пользователей в домене или доверенных доменов пользователя.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Содержит отправлено адресам за пределами домена или доверенных доменов получателя ответов об отсутствии на работе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Содержит аргументы, используется для задания параметров об отсутствии на работе и сообщения пользователя почтового ящика.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В следующем примере запроса SetUserOofSettings задает OoFState **включена**, задает длительность об отсутствии на работе для 10 дней и задает внешних и внутренних сообщений об отсутствии на работе.
  
```xml
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

