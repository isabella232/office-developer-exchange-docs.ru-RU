---
title: TimeZoneContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZoneContext
api_type:
- schema
ms.assetid: 573c462b-aa1d-4ba0-8852-e3f48b26873b
description: Элемент TimeZoneContext используется в загонах Протокол SOAP (SOAP) для указания определения часового пояса, которое будет использоваться по умолчанию при назначении часового пояса для свойств DateTime объектов, которые создаются, обновляются и извлекаются с помощью Exchange Web Services (EWS).
ms.openlocfilehash: a628d4a094e70f1190f2cc0eda8cc4416bc37860
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515175"
---
# <a name="timezonecontext"></a>TimeZoneContext

Элемент **TimeZoneContext** используется в загонах Протокол SOAP (SOAP) для указания определения часового пояса, которое будет использоваться по умолчанию при назначении часового пояса для свойств DateTime объектов, которые создаются, обновляются и извлекаются с помощью Exchange Web Services (EWS). 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 **TimeZoneContextType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TimeZoneDefinition](timezonedefinition.md) <br/> |Указывает периоды и переходы, которые определяют часовой пояс.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, на Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

