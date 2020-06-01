---
title: саведитемфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: Элемент Саведитемфолдерид определяет целевую папку для операций обновления, отправки и создания элементов в почтовом ящике.
ms.openlocfilehash: 8e18b8863a54aa4e9d6e65f7a54e20904f5a9599
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465277"
---
# <a name="saveditemfolderid"></a>саведитемфолдерид

Элемент **саведитемфолдерид** определяет целевую папку для операций обновления, отправки и создания элементов в почтовом ящике. 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

```xml
<SavedItemFolderId>
   <DistinguishedFolderId/>
</SavedItemFolderId>
```

**таржетфолдеридтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения целевой папки для операций, которые обновляют, отправляют и создают элементы в хранилище Exchange.  <br/> |
|[дистингуишедфолдерид](distinguishedfolderid.md) <br/> |Определяет целевую папку с помощью именованного идентификатора для операций, которые обновляют, отправляют и создают элементы в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Определяет запрос на создание элемента в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Определяет запрос на обновление элемента в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Определяет запрос на отправку элемента в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

