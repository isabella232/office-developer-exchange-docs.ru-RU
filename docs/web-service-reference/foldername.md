---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: Элемент FolderName определяет единую настраиваемую папку для добавления в почтовый ящик.
ms.openlocfilehash: 76263d56c423411a58ea45d691ce93e2b3202571
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511567"
---
# <a name="foldername"></a>FolderName

Элемент **FolderName** определяет единую настраиваемую папку для добавления в почтовый ящик. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[FolderNames](foldernames.md)
  
[FolderName](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |Содержит массив именных управляемых пользовательских папок для добавления в почтовый ящик.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение представляет имя папки.
  
## <a name="remarks"></a>Заметки

Несмотря на то Exchange веб-службы можно использовать для добавления управляемых пользовательских папок в почтовый ящик, вы не можете использовать ту же технологию для доступа к списку доступных управляемых пользовательских папок. Список управляемых пользовательских папок можно получить с помощью команды Exchange management Shell или С помощью API, который взаимодействует со службой каталогов Active Directory. Имя папки — это имя соответствующего объекта Active Directory.
  
Вы можете использовать операцию [FindFolder для](findfolder-operation.md) поиска управляемых пользовательских папок. Используйте операцию [DeleteFolder для](deletefolder-operation.md) удаления управляемых пользовательских папок. 
  
Важно отметить, что **folderName** — это имя существующей управляемой пользовательской папки в организации. Попытка добавить папку, не вложенную в организацию, приведет к ошибке. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindFolder](findfolder-operation.md)


[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

