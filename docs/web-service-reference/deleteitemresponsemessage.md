---
title: DeleteItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItemResponseMessage
api_type:
- schema
ms.assetid: c3d34c4d-8d83-4612-aa9e-66f9cc7314df
description: Элемент DeleteItemResponseMessage содержит состояние и результат одного запроса операции DeleteItem.
ms.openlocfilehash: 86a1556ecd6043078b9daa1a98c0c5b8e3c7c386
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545393"
---
# <a name="deleteitemresponsemessage"></a>DeleteItemResponseMessage

Элемент **DeleteItemResponseMessage** содержит состояние и результат одного запроса [операции DeleteItem.](deleteitem-operation.md) 
  
- [DeleteItemResponse](deleteitemresponse.md) 
- [ResponseMessages](responsemessages.md)  
- [DeleteItemResponseMessage](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 **DeleteItemResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ResponseClass** <br/> | Описывает состояние ответа [операции DeleteItem.](deleteitem-operation.md)<br/><br/>Для данного атрибута допустимы следующие значения:<br/><br/>- Успех  <br/>–  Warning  <br/>–  Error  <br/> |
   
#### <a name="responseclass-attribute"></a>Атрибут ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает необработанный запрос. Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов.<br/><br/>Ниже приведены примеры источников предупреждений:<br/><br/>- Exchange магазин выходит из офлайна во время пакета.  <br/>- Службы домена Active Directory (AD DS) отключены.  <br/>– Почтовые ящики перемещены.  <br/>- База данных сообщений (MDB) отключена.  <br/>– Срок действия пароля истек.  <br/>– Превышена квота  <br/> |
|**Error** <br/> | Описывает запрос, который невозможно выполнить.<br/><br/>Ниже приведены примеры источников ошибок:<br/><br/>– Недопустимые атрибуты или элементы  <br/>– Атрибуты или элементы находятся вне диапазона  <br/>– Неизвестный тег  <br/>– Атрибут или элемент недопустим в контексте  <br/>— попытка клиента установить уровень ведения журнала ошибок выше максимального уровня, разрешенного администратором.  <br/>- Попытка клиента установить уровень сбоя серьезности ниже уровня по умолчанию, указанного администратором.  <br/>– Попытка неавторизованного доступа любым клиентом  <br/>– Сбой на стороне сервера в ответ на допустимый клиентский вызов<br/><br/>  Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервирован для последующего применения. Содержит значение 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения отклика для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
### <a name="version-differences"></a>Различия версий

В версиях Exchange, начиная со сборки 15.00.0986.00, элемент **DeleteItemResponseMessage** имеет тип **DeleteItemResponseMessageType**. В предыдущих версиях элемент имеет тип **ResponseMessageType.**
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция DeleteItem](deleteitem-operation.md)
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Удаление элементов (Exchange веб-служб)](https://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

