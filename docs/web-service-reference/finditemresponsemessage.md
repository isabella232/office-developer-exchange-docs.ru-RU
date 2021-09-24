---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: Элемент FindItemResponseMessage содержит состояние и результат одного запроса операции FindItem.
ms.openlocfilehash: 8a736f6782b6901a2b41ea8c602832614a331a06
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518416"
---
# <a name="finditemresponsemessage"></a>FindItemResponseMessage

Элемент **FindItemResponseMessage** содержит состояние и результат одного запроса [операции FindItem.](finditem-operation.md) 
  
- [FindItemResponse](finditemresponse.md) 
- [ResponseMessages](responsemessages.md)
- [FindItemResponseMessage](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 **FindItemResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа операции [FindItem.](finditem-operation.md)<br/><br/> Для данного атрибута допустимы следующие значения: <br/> <br/>–  Success  <br/>–  Warning  <br/>–  Error  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибута ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает необработанный запрос. Предупреждение может быть возвращено, если ошибка произошла во время обработки элемента в запросе и последующие элементы не могут быть обработаны. <br/><br/>Ниже приведены примеры источников предупреждений: <br/> <br/>- Exchange магазин выходит из офлайна во время пакета.  <br/>- Службы домена Active Directory (AD DS) отключены.  <br/>– Почтовые ящики перемещены.  <br/>- База данных сообщений (MDB) отключена.  <br/>– Срок действия пароля истек.  <br/>- Квота была превышена.  <br/> |
|**Error** <br/> | Описывает запрос, который невозможно выполнить. <br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>– Недопустимые атрибуты или элементы  <br/>- Атрибуты или элементы, которые находятся вне диапазона  <br/>- Неизвестный тег  <br/>— атрибут или элемент, не допустимый в контексте  <br/>- Несанкционированная попытка доступа любого клиента  <br/>- Сбой на стороне сервера в ответ на допустимый клиентский вызов  <br/><br/>  Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Содержит результаты поиска одной корневой папки во время операции [FindItem.](finditem-operation.md)  <br/> |
   
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

- [Операция FindItem](finditem-operation.md)
- [Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

