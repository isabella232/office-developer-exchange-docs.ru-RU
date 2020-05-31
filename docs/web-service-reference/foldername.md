---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: Элемент имя_папки определяет отдельную управляемую настраиваемую папку, добавляемую к почтовому ящику.
ms.openlocfilehash: 56a7a7d256624c5103c88a333222807519d21501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762629"
---
# <a name="foldername"></a>FolderName

Элемент **имя_папки** определяет отдельную управляемую настраиваемую папку, добавляемую к почтовому ящику. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[фолдернамес](foldernames.md)
  
[FolderName](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдернамес](foldernames.md) <br/> |Содержит массив именованных управляемых настраиваемых папок для добавления к почтовому ящику.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Текстовое значение представляет имя папки.
  
## <a name="remarks"></a>Примечания

Несмотря на то, что вы можете использовать веб-службы Exchange для добавления управляемых настраиваемых папок в почтовый ящик, вы не можете использовать одну и ту же технологию для доступа к списку доступных управляемых настраиваемых папок. Список управляемых настраиваемых папок можно получить с помощью команды командной консоли Exchange или API, с помощью которого выполняется взаимодействие с службой каталогов Active Directory. Имя папки — это имя соответствующего объекта Active Directory.
  
Для поиска управляемых настраиваемых папок можно использовать [операцию FindFolder](findfolder-operation.md) . Используйте [операцию DeleteFolder](deletefolder-operation.md) для удаления управляемых пользовательских папок. 
  
Важно отметить, что параметр **имя_папки** — это имя существующей управляемой настраиваемой папки в Организации. При попытке добавить папку, которой нет в Организации, будет получено сообщение об ошибке. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindFolder](findfolder-operation.md)


[Поиск папок](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

