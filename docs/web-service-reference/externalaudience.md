---
title: екстерналаудиенце
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
description: Элемент Екстерналаудиенце задает или содержит значение, определяющее отправку внешних сообщений об отсутствии на работе (отсутствие на работе).
ms.openlocfilehash: b3fcebd9042b07bb9a8294196799ef2a13d78bdd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530602"
---
# <a name="externalaudience"></a>екстерналаудиенце

Элемент **екстерналаудиенце** задает или содержит значение, определяющее отправку внешних сообщений об отсутствии на работе (отсутствие на работе). 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 **екстерналаудиенце**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[усеруфсеттингс](useroofsettings.md) <br/> |Задает параметры отсутствия на работе.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[уфсеттингс](oofsettings.md) <br/> |Содержит параметры отсутствия на работе.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|**Нет** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, не будут получать ответ об отсутствии внешних сообщений об отсутствии на работе.  <br/> |
|**Стандартных** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, будут получать ответ о внешнем ответе на отсутствие ответа, если отправитель находится в списке контактов хранилища Exchange пользователя.  <br/> |
|**All** <br/> |Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, получат сообщение о внешнем ответе на отсутствие.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент использует тот же тип, что и элемент [алловекстерналуф](allowexternaloof.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В приведенном ниже примере запроса SetUserOofSettings задается для параметра Уфстате значение **Enabled**, устанавливается для внешней аудитории значение " **все**", устанавливается время бездействия в 10 дней и задаются внутренние и внешние сообщения об отсутствии на работе.
  
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
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserOofSettings](getuseroofsettings-operation.md)
  
[Операция SetUserOofSettings](setuseroofsettings-operation.md)

