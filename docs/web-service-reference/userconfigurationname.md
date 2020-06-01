---
title: усерконфигуратионнаме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: Элемент Усерконфигуратионнаме представляет имя объекта пользовательской конфигурации. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.
ms.openlocfilehash: 020b55919f7f81602a5eb072652d82168607d306
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466033"
---
# <a name="userconfigurationname"></a>усерконфигуратионнаме

Элемент **усерконфигуратионнаме** представляет имя объекта пользовательской конфигурации. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя. 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

```XML
<UserConfigurationName Name="">
   <DistinguishedFolderId/> 
</UserConfigurationName>
```

**усерконфигуратионнаметипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Name** <br/> |Содержит строковое значение, представляющее имя объекта конфигурации пользователя. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Представляет идентификатор папки, содержащей объект конфигурации пользователя.  <br/> |
|[дистингуишедфолдерид](distinguishedfolderid.md) <br/> |Представляет имя папки, содержащей объект конфигурации пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DeleteUserConfiguration](deleteuserconfiguration.md) <br/> |Представляет запрос на удаление объекта конфигурации пользователя.  <br/> |
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Представляет запрос на получение объекта конфигурации пользователя.  <br/> |
|[усерконфигуратион](userconfiguration.md) <br/> |Определяет один объект конфигурации пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

