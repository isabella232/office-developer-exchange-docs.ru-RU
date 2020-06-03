---
title: сетфолдерфиелд
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetFolderField
api_type:
- schema
ms.assetid: 8c69db7b-54b5-4ae2-abca-4d6e0937a790
description: Элемент Сетфолдерфиелд представляет обновление, которое задает значение для одного свойства папки в операции операцию UpdateFolder.
ms.openlocfilehash: ab75a3862801b9a7b3369d9a4116c653b461781c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530319"
---
# <a name="setfolderfield"></a>сетфолдерфиелд

Элемент **сетфолдерфиелд** представляет обновление, которое задает значение для одного свойства папки в операции операцию UpdateFolder. 

```xml
<SetFolderField>
   <FieldURI/>
   <Folder/>
</SetFolderField>
```
  
```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <SearchFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <Folder/> 
</SetFolderField>
```

```xml
<SetFolderField>
    <IndexedFieldURI/> 
    <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <TasksFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <Folder/>
</SetFolderField>
```

```xml
<SetFolderField>
    <FieldURI/> 
    <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <ContactsFolder/> 
</SetFolderField>
```


**сетфолдерфиелдтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фиелдури](fielduri.md) <br/> |Определяет часто упоминаемые свойства по URI.  <br/> |
|[индекседфиелдури](indexedfielduri.md) <br/> |Определяет отдельные элементы словаря.  <br/> |
|[екстендедфиелдури](extendedfielduri.md) <br/> |Определяет расширенные свойства MAPI.  <br/> |
|[Folder](folder.md) <br/> |Определяет папку, которую требуется обновить.  <br/> |
|[календарфолдер](calendarfolder.md) <br/> |Представляет папку, в которой в основном содержатся элементы календаря.  <br/> |
|[контактсфолдер](contactsfolder.md) <br/> |Представляет папку "Контакты" в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, содержащуюся в почтовом ящике.  <br/> |
|[тасксфолдер](tasksfolder.md) <br/> |Представляет папку Tasks, содержащуюся в почтовом ящике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Обновления (папка)](updates-folder.md) <br/> |Содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств папки.  <br/> |
   
## <a name="remarks"></a>Примечания

Если свойство существует, значение свойства задается равным указанному значению. Если свойство не существует, свойство создается с указанным значением.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция UpdateFolder](updatefolder-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

