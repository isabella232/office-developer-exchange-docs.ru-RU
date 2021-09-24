---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: Элемент GetServerTimeZones является корневым элементом запроса на извлечение определений часовой зоны с Exchange сервера.
ms.openlocfilehash: b710334e5778f8bc27ba7ac07c6bf9c2e2d3392e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533541"
---
# <a name="getservertimezones"></a>GetServerTimeZones

Элемент **GetServerTimeZones** является корневым элементом запроса на извлечение определений часовой зоны с Exchange сервера. 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |Указывает, возвращает ли операция [GetServerTimeZones](getservertimezones-operation.md) полное определение или только имя и идентификатор для каждого часового пояса. Этот атрибут является необязательным. Значение по умолчанию  **true**.  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>Атрибут ReturnFullTimeZoneData

|**Значение**|**Описание**|
|:-----|:-----|
|**true** <br/> |Возвращаем полные определения для каждого часовой пояс.  <br/> |
|**false** <br/> |Возвращаем только имя и идентификатор для каждого часовой пояс.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ids](ids.md) <br/> |Содержит массив идентификаторов определений часового пояса, который указывает запрашиваемую определения часового пояса. Этот элемент является необязательным. Если этот элемент не включен в запрос на операцию [GetServerTimeZones,](getservertimezones-operation.md) все определения часовой зоны, доступные на сервере, возвращаются в ответ.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, на Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetServerTimeZones](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

