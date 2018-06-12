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
description: Элемент FolderName определяет один настраиваемой управляемой папки для добавления к почтовому ящику.
ms.openlocfilehash: 56a7a7d256624c5103c88a333222807519d21501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762629"
---
# <a name="foldername"></a>FolderName

Элемент **FolderName** определяет один настраиваемой управляемой папки для добавления к почтовому ящику. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[FolderNames](foldernames.md)
  
[Имя папки](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |Содержит массив именованных управляемые настраиваемые папки для добавления к почтовому ящику.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение представляет имя папки.
  
## <a name="remarks"></a>Замечания

Несмотря на то, что веб-служб Exchange можно использовать для добавления настраиваемых управляемых папок для почтового ящика, та же технология нельзя использовать для доступа к списку доступных настраиваемых управляемых папок. Список настраиваемых управляемых папок можно получить с помощью командной консоли Exchange или с помощью интерфейса API, связанный со службой каталогов Active Directory. Имя папки — это имя соответствующего объекта Active Directory.
  
[Операция FindFolder](findfolder-operation.md) можно использовать для поиска настраиваемых управляемых папок. Используйте [операцию DeleteFolder](deletefolder-operation.md) для удаления настраиваемые управляемые папки. 
  
Важно Обратите внимание на то, что **имя папки** — это имя существующей управляемые настраиваемые папки в организации. При попытке добавить в папку, которая не находится в организации приведет к возврату ошибки. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindFolder Operation](findfolder-operation.md)


[Поиск папок](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

