---
title: усеруфсеттингс
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
description: Элемент Усеруфсеттингс указывает параметры заместителя (отсутствие на работе).
ms.openlocfilehash: 417c3d5061a6229d41eb57f72e89f03213acf460
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461907"
---
# <a name="useroofsettings"></a>усеруфсеттингс

Элемент **усеруфсеттингс** указывает параметры заместителя (отсутствие на работе). 
  
[сетусеруфсеттингсрекуест](setuseroofsettingsrequest.md)
  
[усеруфсеттингс](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 **усеруфсеттингс**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[уфстате](oofstate.md) <br/> |Задает состояние отсутствия на работе пользователя.  <br/> |
|[екстерналаудиенце](externalaudience.md) <br/> |Задает или содержит значение, которое определяет, кому отправляются внешние сообщения об отсутствии на работе.  <br/> |
|[Продолжительность (Усеруфсеттингс)](duration-useroofsettings.md) <br/> |Указывает срок, в течение которого состояние отсутствия на работе включено, если для элемента [уфстате](oofstate.md) задано значение " **запланировано**". Если для элемента [уфстате](oofstate.md) задано значение **Enabled** или **disabled**, значение этого элемента игнорируется.  <br/> |
|[интерналрепли](internalreply.md) <br/> |Содержит ответ о нерабочем месте, отправленный другим пользователям в домене пользователя или доверенных доменах.  <br/> |
|[екстерналрепли](externalreply.md) <br/> |Содержит ответ о нерабочем месте, отправленный на адреса, не входящие в домен получателя или доверенные домены.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[сетусеруфсеттингсрекуест](setuseroofsettingsrequest.md) <br/> |Содержит аргументы, используемые для задания параметров и сообщений о нежелательных пользователя почтового ящика.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В следующем примере запроса SetUserOofSettings задается для Уфстате значение **Enabled**, устанавливается длительность бездействия в течение 10 дней, а также задаются внутренние и внешние сообщения об отсутствии на работе.
  
```xml
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |схема сообщений  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция SetUserOofSettings](setuseroofsettings-operation.md)

