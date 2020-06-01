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
description: Элемент DeleteFolder определяет запрос на удаление папок из почтового ящика в хранилище Exchange.
ms.openlocfilehash: eb705a47b78b19c79b2e87561ba3696ed40e09cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458770"
---
# <a name="deletefolder"></a>DeleteFolder

Элемент **DeleteFolder** определяет запрос на удаление папок из почтового ящика в хранилище Exchange. 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 **делетефолдертипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**делететипе** <br/> |Описывает, как удаляется папка. Этот атрибут является обязательным.  <br/> |
   
#### <a name="deletetype-attribute"></a>Атрибут Делететипе

|**Значение**|**Описание**|
|:-----|:-----|
|HardDelete  <br/> |Папка безвозвратно удаляется из хранилища.  <br/> |
|SoftDelete  <br/> |При включенной корзине папка перемещается в корзину.  <br/> |
|MoveToDeletedItems  <br/> |Папка перемещается в папку "Удаленные".  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдеридс](folderids.md) <br/> |Содержит массив идентификаторов папок, которые используются для идентификации папок, которые необходимо удалить.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Параметры **MoveToDeletedItems** и **HardDelete** являются транзакционными, что означает, что по завершении вызова веб-службы база данных переместит элемент в папку "Удаленные" или окончательно удалил его из базы данных Exchange. Это одно и то же поведение для Майкрософт Exchange Server 2007 и Exchange Server 2010. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция DeleteFolder](deletefolder-operation.md)

