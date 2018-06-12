---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: Элемент ParentItemId определяет родительский элемент, ссылки на связанные вложения.
ms.openlocfilehash: 9bd875ee5ead8b87996288a640e1bb14e3a5e8b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834703"
---
# <a name="parentitemid"></a>ParentItemId

Элемент **ParentItemId** определяет родительский элемент, ссылки на связанные вложения. 
  
- [CreateAttachment](createattachment.md)
  
- [ParentItemId](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

**ItemIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|
  **Id** <br/> |Определяет один элемент в хранилище Exchange для связи с вложением. Это значение является строкой. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Определяет не указан версию элемента, который идентифицируется с помощью атрибута **Id** в хранилище Exchange. Здесь указывается убедитесь в том, что текущего элемента используется при обновлении с вложением. Это значение является строкой. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Определяет запрос на создание вложения в элемент в почтовом ящике.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент является обязательным в [CreateAttachment операции](createattachment-operation.md). Этот элемент по сути является то же, что элемент [ItemId](itemid.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |[http://schemas.microsoft.com/exchange/services/2006/messages](http://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция CreateAttachment](createattachment-operation.md)

