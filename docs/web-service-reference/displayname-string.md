---
title: DisplayName (строка)
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
description: Элемент DisplayName определяет отображаемое имя папки, контакта, списка рассылки, пользователя, расположения или правила.
ms.openlocfilehash: 9b566ec1938ec206e45cddf9c7f00083af2d8a9c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463618"
---
# <a name="displayname-string"></a>DisplayName (строка)

Элемент **DisplayName** определяет отображаемое имя папки, контакта, списка рассылки, пользователя, расположения или правила. 
  
```XML
<DisplayName/>
```

 **String**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календарфолдер](calendarfolder.md) <br/> |Представляет папку "Календарь" в почтовом ящике.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[контактсфолдер](contactsfolder.md) <br/> |Представляет папку контактов в почтовом ящике.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[Правило (RuleType)](rule-ruletype.md) <br/> |Представляет правило в почтовом ящике пользователя.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[тасксфолдер](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
|[UserId](userid.md) <br/> |Определяет делегата или пользователя с разрешениями на доступ к папке.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

При использовании этого элемента необходимо указать текстовое значение, представляющее отображаемое имя.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере показано, как создать новую папку и задать для нее значение "Тестфолдер".
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

