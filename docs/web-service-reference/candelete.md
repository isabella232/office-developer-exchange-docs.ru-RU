---
title: CanDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanDelete
api_type:
- schema
ms.assetid: 55e17121-aad0-4f90-889f-2c3512e9579c
description: Элемент CanDelete указывает, можно ли удалить управляемой папки клиентом.
ms.openlocfilehash: b70b28bd6b3c9452f5d7f249f453218d555754da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761665"
---
# <a name="candelete"></a>CanDelete

Элемент **CanDelete** указывает, можно ли удалить управляемой папки клиентом. 
  
```xml
<CanDelete/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Содержит сведения об управляемых папок.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее логическое значение является обязательным, если присутствует этого элемента. Значение **true** указывает, что можно удалить папку; значение **false** означает, что папка не может быть удален. 
  
## <a name="remarks"></a>Замечания

Чтобы удалить управляемых папок, с помощью [операции DeleteFolder](deletefolder-operation.md).
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateManagedFolder](createmanagedfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Удаление папок](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

