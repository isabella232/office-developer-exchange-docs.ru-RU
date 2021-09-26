---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: Элемент DeleteFolder определяет запрос на удаление папок из почтового ящика в Exchange магазине.
ms.openlocfilehash: d1d64b84604acec54d9153144e5bfd7abaece94c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542479"
---
# <a name="deletefolder"></a>DeleteFolder

Элемент **DeleteFolder** определяет запрос на удаление папок из почтового ящика в Exchange магазине. 
  
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
|**DeleteType** <br/> |Описывает, как удаляется папка. Этот атрибут является обязательным.  <br/> |
   
#### <a name="deletetype-attribute"></a>Атрибут DeleteType

|**Значение**|**Описание**|
|:-----|:-----|
|HardDelete  <br/> |Папка постоянно удаляется из магазина.  <br/> |
|SoftDelete  <br/> |Если контейнер включен, папка перемещается в контейнер.  <br/> |
|MoveToDeletedItems  <br/> |Папка перемещается в папку "Удаленные элементы".  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Содержит массив идентификаторов папок, используемых для идентификации папок для удаления.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Параметры **MoveToDeletedItems** и **HardDelete** являются транзакциями, что означает, что к моменту завершения вызова веб-службы база данных переместила элемент в папку "Удаленные элементы" или окончательно удалила его из Exchange базы данных. Это поведение одинаково для MicrosoftExchange Server 2007 и Exchange Server 2010. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция DeleteFolder](deletefolder-operation.md)

