---
title: конвертидреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: Элемент Конвертидреспонсемессаже содержит состояние и результат запроса операции ConvertId.
ms.openlocfilehash: cd0154f87390be3516ced4be53f5371d4a348c49
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456222"
---
# <a name="convertidresponsemessage"></a>конвертидреспонсемессаже

Элемент **конвертидреспонсемессаже** содержит состояние и результат запроса [операции ConvertId](convertid-operation.md) . 
  
- [конвертидреспонсе](convertidresponse.md) 
- [респонсемессажес](responsemessages.md)
- [конвертидреспонсемессаже](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 **конвертидреспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**респонсекласс** <br/> | Описывает состояние ответа [операции ConvertId](convertid-operation.md) .<br/><br/>Для этого атрибута допустимы следующие значения:<br/><br/>Успешное выполнение  <br/>— Предупреждение  <br/>— Ошибка  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов Респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает запрос, который не был полностью обработан или для которого возникл нежелательный результат.  <br/> |
|**Error** <br/> | Описывает запрос, который не может быть выполнен.<br/><br/>Ниже приведены примеры источников ошибок.  <br/><br/>— Недопустимые атрибуты или элементы  <br/>— Атрибуты или элементы, которые выходят за пределы допустимого диапазона  <br/>— Неизвестный тег  <br/>— Атрибут или элемент, который не является допустимым в контексте  <br/>— Попытки несанкционированного доступа, выполняемые любым клиентом;  <br/>— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента<br/><br/>Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.  <br/> |
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для будущего использования. Этот элемент содержит значение 0.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
|[AlternateId](alternateid.md) <br/> |Описывает преобразованный идентификатор в отклике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Содержит ответные сообщения для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Возвращается одно ответное сообщение на один преобразованный идентификатор. Элемент [AlternateId](alternateid.md) будет отсутствовать в ответе, если возвращается код ответа об ошибке, 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Exchange 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ConvertId](convertid-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

