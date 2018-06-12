---
title: Отображаемое имя (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisplayName
api_type:
- schema
ms.assetid: e7efbbe1-6629-4d11-bed1-ed899e3f9d77
description: Элемент DisplayName определяет отображаемое имя папки, контактов, список рассылки, делегата, расположение или правило.
ms.openlocfilehash: 53f4e083d9e6617206e383d4408e08ed7ea0fe08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762164"
---
# <a name="displayname-string"></a>Отображаемое имя (строка)

Элемент **DisplayName** определяет отображаемое имя папки, контактов, список рассылки, делегата, расположение или правило. 
  
```XML
<DisplayName/>
```

 **Строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку Календарь в почтовом ящике.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папке контактов в почтовом ящике.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[Правило (RuleType)](rule-ruletype.md) <br/> |Представляет правило в почтовом ящике пользователя.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
|[Идентификатор пользователя](userid.md) <br/> |Идентифицирует пользователя делегатом или пользователь, имеющий права доступа к папкам.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее отображаемое имя является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере показано, как создать новую папку и задавать DisplayName папки «TestFolder».
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

