---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: Элемент GetServerTimeZones является корневым элементом запроса для получения определений часовых поясов с сервера Exchange.
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762920"
---
# <a name="getservertimezones"></a>GetServerTimeZones

Элемент **GetServerTimeZones** является корневым элементом запроса для получения определений часовых поясов с сервера Exchange. 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **жетсервертимезонестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ретурнфуллтимезонедата** <br/> |Указывает, возвращает ли [Операция GetServerTimeZones](getservertimezones-operation.md) полное определение или только имя и идентификатор для каждого часового пояса. Этот атрибут является необязательным. Значение по умолчанию  **true**.  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>Атрибут Ретурнфуллтимезонедата

|**Значение**|**Описание**|
|:-----|:-----|
|**относится** <br/> |Получение полных определений для каждого часового пояса.  <br/> |
|**значения** <br/> |Возвращает только имя и идентификатор для каждого часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификаторы](ids.md) <br/> |Содержит массив идентификаторов определения часовых поясов, которые задают запрошенные определения часовых поясов. Этот элемент является необязательным. Если этот элемент не включен в запрос [операции GetServerTimeZones](getservertimezones-operation.md) , все определения часовых поясов, доступные на сервере, возвращаются в ответе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetServerTimeZones](getservertimezones-operation.md)
  
[жетсервертимезонесреспонсе](getservertimezonesresponse.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

