---
title: GetEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetEventsResponseMessage
api_type:
- schema
ms.assetid: d433977f-b86a-499e-b9c3-f405ac229358
description: Элемент GetEventsResponseMessage содержит состояние и результат одного запроса на операцию GetEvents.
ms.openlocfilehash: d35b3f3dd3ff3cfe914b425d6e490d778922a342
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542283"
---
# <a name="geteventsresponsemessage"></a>GetEventsResponseMessage

Элемент **GetEventsResponseMessage** содержит состояние и результат одного запроса на операцию [GetEvents.](getevents-operation.md) 
  
```xml
<GetEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</GetEventsResponseMessage>
```

 **GetEventsResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа на операцию [GetEvents.](getevents-operation.md) <br/><br/>Для данного атрибута допустимы следующие значения: <br/> <br/>–  Success  <br/>–  Warning  <br/>–  Error  <br/> |
   
#### <a name="responseclass-attribute"></a>Атрибут ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|Успешно  <br/> |Описывает выполненный запрос.  <br/> |
|Предупреждение  <br/> | Описывает необработанный запрос. Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов. <br/><br/>Ниже приведены примеры источников предупреждений: <br/> <br/>– Хранилище Exchange находится в автономном режиме при обработке пакета.  <br/>– Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>- Почтовые ящики были перемещены.  <br/>- База данных почтовых ящиков (MDB) отключена.  <br/>- Срок действия пароля истек.  <br/>- Квота была превышена.  <br/> |
|Error  <br/> | Описывает запрос, который невозможно выполнить. <br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>– Недопустимые атрибуты или элементы  <br/>- Атрибуты или элементы, которые находятся вне диапазона  <br/>- Неизвестный тег  <br/>— атрибут или элемент, не допустимый в контексте  <br/>- Несанкционированная попытка доступа любого клиента  <br/>- Сбой на стороне сервера в ответ на допустимый клиентский вызов  <br/><br/>  Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
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

- [GetEvents](getevents.md) 
- [GetEventsResponse](geteventsresponse.md)
- [Операция GetEvents](getevents-operation.md)

