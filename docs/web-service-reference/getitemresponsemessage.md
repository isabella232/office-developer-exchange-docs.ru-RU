---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: Элемент GetItemResponseMessage содержит состояние и результат одного запроса на операцию GetItem.
ms.openlocfilehash: 3c931a6d7df91e4e90bfd0a69dc4816ee71a0aad
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521964"
---
# <a name="getitemresponsemessage"></a>GetItemResponseMessage

Элемент **GetItemResponseMessage** содержит состояние и результат одного запроса на операцию [GetItem.](getitem-operation.md) 
  
- [GetItemResponse](getitemresponse.md) 
- [ResponseMessages](responsemessages.md)
- [GetItemResponseMessage](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

**ItemInfoResponseMessageType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа [на операцию GetItem.](getitem-operation.md) <br/><br/>Для данного атрибута допустимы следующие значения:<br/><br/>- Успех<br/>- Предупреждение<br/>- Ошибка |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибута ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает необработанный запрос. Предупреждение может быть возвращено, если произошла ошибка во время обработки элемента запроса и не удалось обработать последующие элементы.<br/><br/>Ниже приводится пример источников предупреждений:<br/><br/>- Exchange в автономном режиме во время пакета.<br/>- Служба домена Active Directory (AD DS) отключена.<br/>- Почтовые ящики перемещаются.<br/>- MDB находится в автономном режиме.<br/>- Срок действия пароля истек.  <br/>- Квота превышена. |
|**Error** <br/> | Описывает запрос, который невозможно выполнить.<br/><br/>Ниже приводится пример источников ошибок:<br/><br/>- Недействительные атрибуты или элементы<br/>- Атрибуты или элементы вне диапазона<br/>- Неизвестный тег<br/>- Атрибут или элемент, не допустимый в контексте<br/>- Несанкционированный доступ, который пытается получить любой клиент<br/>- Сбой на стороне сервера в ответ на допустимый клиентский вызов<br/><br/>Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md). |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
|[Items](items.md) <br/> |Содержит массив возвращенных элементов.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения отклика для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [GetItem](getitem.md)
- [Операция GetItem](getitem-operation.md)

