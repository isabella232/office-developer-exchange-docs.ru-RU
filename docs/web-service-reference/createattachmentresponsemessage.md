---
title: CreateAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateAttachmentResponseMessage
api_type:
- schema
ms.assetid: b326e616-3ce0-4dcb-ba75-4ce4b9867211
description: Элемент CreateAttachmentResponseMessage содержит состояние и результат одного запроса операции CreateAttachment.
ms.openlocfilehash: da4183c8d81fbcf5abe6b46321e9bff50ad96f2a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536544"
---
# <a name="createattachmentresponsemessage"></a>CreateAttachmentResponseMessage

Элемент **CreateAttachmentResponseMessage** содержит состояние и результат одного запроса операции [CreateAttachment.](createattachment-operation.md) 
  
- [CreateAttachmentResponse](createattachmentresponse.md)
- [ResponseMessages](responsemessages.md)
- [CreateAttachmentResponseMessage](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

**AttachmentInfoResponseMessageType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа операции [CreateAttachment.](createattachment-operation.md) <br/><br/>Для данного атрибута допустимы следующие значения:<br/><br/>–  Success  <br/>–  Warning  <br/>–  Error  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибута ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает необработанный запрос. Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов.<br/><br/>Ниже приведены примеры источников предупреждений:<br/><br/>– Хранилище Exchange находится в автономном режиме при обработке пакета.  <br/>– Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>– Почтовые ящики перемещены.  <br/>– База данных сообщений (MDB) находится в автономном режиме.  <br/>– Срок действия пароля истек.  <br/>– Превышена квота  <br/> |
|**Error** <br/> | Описывает запрос, который невозможно выполнить.<br/><br/>Ниже приведены примеры источников ошибок:  <br/><br/>- Недействительные атрибуты или элементы  <br/>– Атрибуты или элементы находятся вне диапазона  <br/>– Неизвестный тег  <br/>– Атрибут или элемент недопустим в контексте  <br/>– Попытка неавторизованного доступа любым клиентом  <br/>– Сбой на стороне сервера в ответ на допустимый клиентский вызов<br/><br/>  Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, присоединенные к элементу в Exchange магазине.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения отклика для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
> [!NOTE]
> Если к элементу в одном круговом путешествии прикреплено несколько вложений, атрибут **RootItemChangeKey** в последнем сообщении отклика представляет новый ключ изменения элемента с вложениями. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция CreateAttachment](createattachment-operation.md) 
- [CreateAttachment](createattachment.md)
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md) 
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

