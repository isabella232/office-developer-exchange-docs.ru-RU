---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: Элемент ParentItemId определяет родительский элемент, который связывается с связанным вложением.
ms.openlocfilehash: d8072e86d8bd989d4baf6b0f29385dc955b83de8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515364"
---
# <a name="parentitemid"></a>ParentItemId

Элемент **ParentItemId** определяет родительский элемент, который связывается с связанным вложением. 
  
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
|**Id** <br/> |Определяет один элемент в Exchange для связи с вложением. Это значение — строка. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Определяет неустановленную версию элемента, определяемого атрибутом **Id** в Exchange магазине. Это используется для того, чтобы убедиться, что текущий элемент используется при обновлении с помощью вложения. Это значение — строка. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Определяет запрос на создание вложения к элементу в почтовом ящике.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент необходим в операции [CreateAttachment.](createattachment-operation.md) Этот элемент в основном такой же, как элемент [ItemId.](itemid.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция CreateAttachment](createattachment-operation.md)

