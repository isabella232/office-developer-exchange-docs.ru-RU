---
title: DeleteFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteFolderResponseMessage
api_type:
- schema
ms.assetid: de4c63ff-80b2-40c2-bc06-ef0c23beacd4
description: Элемент DeleteFolderResponseMessage содержит состояние и результат одного запроса операции DeleteFolder.
ms.openlocfilehash: 9002764f55981d7bb24a18c41312393b24a075d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542458"
---
# <a name="deletefolderresponsemessage"></a>DeleteFolderResponseMessage

Элемент **DeleteFolderResponseMessage** содержит состояние и результат одного запроса операции [DeleteFolder.](deletefolder-operation.md) 
  
- [DeleteFolderResponse](deletefolderresponse.md)  
- [ResponseMessages](responsemessages.md)  
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
  
```xml
<DeleteFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteFolderResponseMessage>
```

 **ResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа операции [DeleteFolder.](deletefolder-operation.md)<br/><br/>Для данного атрибута допустимы следующие значения:<br/><br/>–  Success  <br/>–  Warning  <br/>–  Error  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибута ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает необработанный запрос. Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов.<br/><br/>Ниже приведены примеры источников предупреждений:<br/><br/>- Exchange магазин выходит из офлайна во время пакета.<br/>- Службы домена Active Directory (AD DS) отключены.<br/>- Почтовые ящики перемещаются.<br/>- База данных сообщений (MDB) отключена.<br/>- Истек срок действия пароля.<br/>- Квота превышена.  <br/> |
|**Error** <br/> | Описывает запрос, который невозможно выполнить.<br/><br/>Ниже приведены примеры источников ошибок:<br/><br/>- Недействительные атрибуты или элементы<br/>- Атрибуты или элементы вне диапазона<br/>- Неизвестный тег<br/>- Атрибут или элемент, не допустимый в контексте<br/>- Попытка несанкционированного доступа любого клиента<br/>- Сбой на стороне сервера в ответ на допустимый клиентский вызов  <br/><br/>  Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Текстовое описание состояния ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Он содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
   
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

- [Операция DeleteFolder](deletefolder-operation.md)
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Удаление папок](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

