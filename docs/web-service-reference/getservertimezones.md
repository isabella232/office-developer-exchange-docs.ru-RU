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
description: Элемент GetServerTimeZones является корневым элементом в запросе на получение определений часовых поясов из Exchange server.
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762920"
---
# <a name="getservertimezones"></a>GetServerTimeZones

Элемент **GetServerTimeZones** является корневым элементом в запросе на получение определений часовых поясов из Exchange server. 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |Указывает, возвращает ли [операция GetServerTimeZones](getservertimezones-operation.md) полное определение или только имя и идентификатор для каждого часового пояса. Этот атрибут является необязательным. Значение по умолчанию — **true**.  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>Атрибут ReturnFullTimeZoneData

|**Значение**|**Описание**|
|:-----|:-----|
|**значение true** <br/> |Возвращает полный определения для каждого часового пояса.  <br/> |
|**false** <br/> |Возвращает имя и идентификатор для каждого часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификаторы](ids.md) <br/> |Содержит массив идентификаторов определения часового пояса, который задает определения запрошенный часового пояса. Этот элемент является необязательным. Если этот элемент не включен в запрос [GetServerTimeZones операции](getservertimezones-operation.md) , все определения часового пояса, доступных на сервере возвращаемого в ответе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetServerTimeZones](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

