---
title: делетеаттачментреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachmentResponseMessage
api_type:
- schema
ms.assetid: 1edb085f-1674-48e5-8ec3-42351adeac7d
description: Элемент Делетеаттачментреспонсемессаже содержит состояние и результат одного запроса операции DeleteAttachment.
ms.openlocfilehash: 3ff253a5c2b6cbd69b7b976f7f41ca8b83814a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464261"
---
# <a name="deleteattachmentresponsemessage"></a>делетеаттачментреспонсемессаже

Элемент **делетеаттачментреспонсемессаже** содержит состояние и результат одного запроса [операции DeleteAttachment](deleteattachment-operation.md) . 
  
- [делетеаттачментреспонсе](deleteattachmentresponse.md)  
- [респонсемессажес](responsemessages.md)  
- [делетеаттачментреспонсемессаже](deleteattachmentresponsemessage.md)
  
```xml
<DeleteAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootItemId/>
</DeleteAttachmentResponseMessage>
```

**делетеаттачментреспонсемессажетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**респонсекласс** <br/> | Описывает состояние ответа [операции DeleteAttachment](deleteattachment-operation.md) .<br/><br/>Для этого атрибута допустимы следующие значения:<br/><br/>Успешное выполнение  <br/>— Предупреждение  <br/>— Ошибка  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов Респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает запрос, который не был обработан. Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.<br/><br/>Ниже приведены примеры источников предупреждений.<br/><br/>— Хранилище Exchange находится в автономном режиме во время выполнения пакета.  <br/>-Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>— Почтовые ящики перемещаются.  <br/>— База данных сообщений (MDB) находится в автономном режиме.  <br/>— Срок действия пароля истек.  <br/>— Превышена квота.  <br/> |
|**Error** <br/> | Описывает запрос, который не может быть выполнен.<br/><br/>Ниже приведены примеры источников ошибок.<br/><br/>— Недопустимые атрибуты или элементы  <br/>— Атрибуты или элементы выходят за пределы допустимого диапазона  <br/>— Неизвестный тег  <br/>— Атрибут или элемент не является допустимым в контексте  <br/>— Попытки несанкционированного доступа, выполняемые любым клиентом;  <br/>Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента<br/><br/>  Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.  <br/> |
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для последующего использования. Он содержит значение 0.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
|[рутитемид](rootitemid.md) <br/> |Определяет родительский элемент удаленного вложения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Содержит ответные сообщения для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [DeleteAttachment](deleteattachment.md) 
- [Операция DeleteAttachment](deleteattachment-operation.md)
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md) 
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

