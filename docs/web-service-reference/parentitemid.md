---
title: парентитемид
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
description: Элемент Парентитемид определяет родительский элемент, ссылающийся на связанное вложение.
ms.openlocfilehash: 4f3e33da0af2438948313f0e335cd03e076d135a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465746"
---
# <a name="parentitemid"></a>парентитемид

Элемент **парентитемид** определяет родительский элемент, ссылающийся на связанное вложение. 
  
- [CreateAttachment](createattachment.md)
  
- [парентитемид](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

**итемидтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Определяет один элемент в хранилище Exchange, связываемый с вложением. Это значение является строкой. Этот атрибут является обязательным.  <br/> |
|**чанжекэй** <br/> |Определяет неопределенную версию элемента, определяемого атрибутом **ID** в хранилище Exchange. Это используется, чтобы убедиться, что текущий элемент используется при обновлении с вложением. Это значение является строкой. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Определяет запрос на создание вложения для элемента в почтовом ящике.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент является обязательным в [операции CreateAttachment](createattachment-operation.md). Этот элемент в основном совпадает с элементом [ItemId](itemid.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция CreateAttachment](createattachment-operation.md)

