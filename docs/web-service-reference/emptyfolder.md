---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: Элемент EmptyFolder определяет запрос на очистку папки в почтовом ящике в хранилище Exchange. Кроме того, при очистке папки также можно удалить вложенные папки.
ms.openlocfilehash: a42e4e3f25741a96ee65fe6f87fc3236b68f4dc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457279"
---
# <a name="emptyfolder"></a>EmptyFolder

Элемент **EmptyFolder** определяет запрос на очистку папки в почтовом ящике в хранилище Exchange. Кроме того, при очистке папки также можно удалить вложенные папки. 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 **емптифолдертипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**делететипе** <br/> |Указывает, как очищается папка. Этот атрибут является обязательным.  <br/> |
|**делетесубфолдерс** <br/> |Указывает, следует ли удалять подпапки. Этот атрибут является обязательным.  <br/> |
   
#### <a name="deletetype-attribute"></a>Атрибут Делететипе

|**Значение**|**Описание**|
|:-----|:-----|
|HardDelete  <br/> |Сообщения и папки безвозвратно удаляются из хранилища.  <br/> |
|SoftDelete  <br/> |При включенной корзине сообщения и папки перемещаются в корзину.  <br/> |
|MoveToDeletedItems  <br/> |Сообщения и папки перемещаются в папку "Удаленные".  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдеридс](folderids.md) <br/> |Содержит массив идентификаторов папок, которые используются для идентификации папок, которые необходимо удалить.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция EmptyFolder](emptyfolder-operation.md)

