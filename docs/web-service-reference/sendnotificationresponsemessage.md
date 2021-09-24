---
title: SendNotificationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SendNotificationResponseMessage
api_type:
- schema
ms.assetid: 2c6d681b-67ac-4331-bc6b-a2e709b638e3
description: Элемент SendNotificationResponseMessage содержит состояние и результат одного запроса операции SendNotification.
ms.openlocfilehash: 8e6b54a1afa046f7bd318fb8eca7d1cbeb6c4c8b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521615"
---
# <a name="sendnotificationresponsemessage"></a>SendNotificationResponseMessage

Элемент **SendNotificationResponseMessage** содержит состояние и результат одного запроса операции **SendNotification.** 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 **SendNotificationResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа операции **SendNotification.** <br/><br/>Для данного атрибута допустимы следующие значения:  <br/><br/>–  Success  <br/>–  Warning  <br/>–  Error  <br/> |
   
#### <a name="responseclass-attribute"></a>Атрибут ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает необработанный запрос. Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов.<br/><br/> Ниже приведены примеры источников предупреждений:  <br/><br/>– Хранилище Exchange находится в автономном режиме при обработке пакета.  <br/>– Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>– Почтовые ящики перемещены.  <br/>– База данных сообщений (MDB) находится в автономном режиме.  <br/>- Срок действия пароля истек.  <br/>- Квота была превышена.  <br/> |
|**Error** <br/> | Описывает запрос, который невозможно выполнить. <br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>– Недопустимые атрибуты или элементы  <br/>- Атрибуты или элементы, которые находятся вне диапазона  <br/>- Неизвестный тег  <br/>- Атрибут или элемент, не допустимый в контексте  <br/>- Несанкционированная попытка доступа любого клиента  <br/>- Сбой на стороне сервера в ответ на допустимый клиентский вызов  <br/><br/>  Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения отклика для запроса веб-служб Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [SendNotification](sendnotification.md)
- [Операции подписки](subscribe-operation.md)
- [Операция Unsubscribe](unsubscribe-operation.md)

