---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: Элемент DeleteFolder определяет запрос на удаление папки из почтового ящика в хранилище Exchange.
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762036"
---
# <a name="deletefolder"></a>DeleteFolder

Элемент **DeleteFolder** определяет запрос на удаление папки из почтового ящика в хранилище Exchange. 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 **DeleteFolderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**DeleteType** <br/> |Описывает, как удалить папку. Этот атрибут является обязательным.  <br/> |
   
#### <a name="deletetype-attribute"></a>Атрибут DeleteType

|**Значение**|**Описание**|
|:-----|:-----|
|HardDelete  <br/> |Папка окончательно удалить из хранилища.  <br/> |
|SoftDelete  <br/> |Папка перемещается в корзину Если корзины включена.  <br/> |
|MoveToDeletedItems  <br/> |Папка переносится для папки «Удаленные».  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Содержит массив идентификаторов папок, которые используются для определения папок, которые следует удалить.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Параметры **MoveToDeletedItems** и **HardDelete** являются транзакций, это означает, что с на время завершения вызова веб-службы, базы данных переместить элемент папки «Удаленные» или окончательно удалить элемент из базы данных Exchange. Это поведение не зависит от MicrosoftExchange Server 2007 и Exchange Server 2010. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция DeleteFolder](deletefolder-operation.md)

