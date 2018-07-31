---
title: UserConfigurationName
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
description: Элемент UserConfigurationName представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.
ms.openlocfilehash: 33b3fc316a06b8088eb20a71788a9e6a3394d0d4
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354304"
---
# <a name="userconfigurationname"></a>UserConfigurationName

Элемент **UserConfigurationName** представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя. 
  
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

**UserConfigurationNameType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Name** <br/> |Содержит строковое значение, представляющее имя объекта конфигурации пользователя. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Представляет идентификатор папки папку, содержащую объект конфигурации пользователя.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Представляет имя различающегося папки папку, содержащую объект конфигурации пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DeleteUserConfiguration](deleteuserconfiguration.md) <br/> |Представляет запрос на удаление объекта конфигурации пользователя.  <br/> |
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Представляет запрос на получение объекта конфигурации пользователя.  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |Определяет объект конфигурации одного пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

