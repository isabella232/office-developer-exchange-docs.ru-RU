---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: Элемент EmptyFolder определяет запрос на пустой папку в почтовом ящике в Exchange магазине. Необязательно, подмостки также могут быть удалены, когда папка опустеет.
ms.openlocfilehash: c1b0e953f677c1fe5ae0958b35f85f3f5c4fb973
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519676"
---
# <a name="emptyfolder"></a>EmptyFolder

Элемент **EmptyFolder** определяет запрос на пустой папку в почтовом ящике в Exchange магазине. Необязательно, подмостки также могут быть удалены, когда папка опустеет. 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 **EmptyFolderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**DeleteType** <br/> |Указывает, как опустошает папку. Этот атрибут является обязательным.  <br/> |
|**DeleteSubFolders** <br/> |Указывает, следует ли удалять подмостки. Этот атрибут является обязательным.  <br/> |
   
#### <a name="deletetype-attribute"></a>Атрибут DeleteType

|**Значение**|**Описание**|
|:-----|:-----|
|HardDelete  <br/> |Сообщения и папки удаляются из магазина навсегда.  <br/> |
|SoftDelete  <br/> |Если контейнер включен, сообщения и папки перемещаются в контейнер.  <br/> |
|MoveToDeletedItems  <br/> |Сообщения и папки перемещаются в папку "Удаленные элементы".  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Содержит массив идентификаторов папок, используемых для идентификации папок для удаления.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция EmptyFolder](emptyfolder-operation.md)

