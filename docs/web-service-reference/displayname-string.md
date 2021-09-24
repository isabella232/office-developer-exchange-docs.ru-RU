---
title: DisplayName (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DisplayName
api_type:
- schema
ms.assetid: e7efbbe1-6629-4d11-bed1-ed899e3f9d77
description: Элемент DisplayName определяет имя отображения папки, контакта, списка рассылки, делегирования пользователя, расположения или правила.
ms.openlocfilehash: 3fc0faca0425bc6de3f71c154926991d922c8a79
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520865"
---
# <a name="displayname-string"></a>DisplayName (строка)

Элемент **DisplayName** определяет имя отображения папки, контакта, списка рассылки, делегирования пользователя, расположения или правила. 
  
```XML
<DisplayName/>
```

 **String**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку календаря в почтовом ящике.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку контактов в почтовом ящике.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[Правило (RuleType)](rule-ruletype.md) <br/> |Представляет правило в почтовом ящике пользователя.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
|[UserId](userid.md) <br/> |Определяет пользователя-делегата или пользователя, у которого есть разрешения на доступ к папкам.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если используется этот элемент, требуется текстовое значение, представляю которое представляет имя отображения.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере показано, как создать новую папку и установить имя displayname папки на "TestFolder".
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

