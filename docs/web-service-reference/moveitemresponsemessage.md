---
title: MoveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoveItemResponseMessage
api_type:
- schema
ms.assetid: 1efacb2c-cb76-44ad-b0be-bb47bf2553be
description: Элемент MoveItemResponseMessage содержит состояние и результат одного запроса на операцию MoveItem.
ms.openlocfilehash: 7ede208e5bba09827f505401bc1221bd78e15d25
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515539"
---
# <a name="moveitemresponsemessage"></a>MoveItemResponseMessage

Элемент **MoveItemResponseMessage** содержит состояние и результат одного запроса на операцию [MoveItem.](moveitem-operation.md) 
  
```xml
<MoveItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</MoveItemResponseMessage>
```

 **ItemInfoResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа на [операцию MoveItem.](moveitem-operation.md) <br/><br/>Для данного атрибута допустимы следующие значения:  <br/><br/>–  Success  <br/>–  Warning  <br/>–  Error  <br/> |
   
#### <a name="responseclass-attribute"></a>Атрибут ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает необработанный запрос. Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов. <br/><br/>Ниже приведены примеры источников предупреждений:  <br/><br/>– Хранилище Exchange находится в автономном режиме при обработке пакета.  <br/>– Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>– Почтовые ящики перемещены.  <br/>– База данных сообщений (MDB) находится в автономном режиме.  <br/>– Срок действия пароля истек.  <br/>- Квота была превышена.  <br/> |
|**Error** <br/> | Описывает запрос, который невозможно выполнить. <br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>– Недопустимые атрибуты или элементы  <br/>– Атрибуты или элементы находятся вне диапазона  <br/>– Неизвестный тег  <br/>– Атрибут или элемент недопустим в контексте  <br/>- Любой несанкционированный доступ, который пытается получить любой клиент  <br/>- Любой сбой на стороне сервера в ответ на допустимый клиентский вызов.  <br/><br/>  Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
|[Items](items.md) <br/> |Содержит массив перемещенных элементов.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения отклика для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, который Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция MoveItem](moveitem-operation.md)
- [MoveItem](moveitem.md)

