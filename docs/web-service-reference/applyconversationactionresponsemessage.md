---
title: аппликонверсатионактионреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: Элемент Аппликонверсатионактионреспонсемессаже содержит состояние и результаты запроса операции ApplyConversationAction.
ms.openlocfilehash: 377aee12d8cc7d6b4aff8d6fc2a6cb67b3bcd10b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464695"
---
# <a name="applyconversationactionresponsemessage"></a>аппликонверсатионактионреспонсемессаже

Элемент **аппликонверсатионактионреспонсемессаже** содержит состояние и результаты запроса [операции ApplyConversationAction](applyconversationaction-operation.md) .  
  
- [аппликонверсатионактионреспонсе](applyconversationactionresponse.md)
- [респонсемессажес](responsemessages.md)
- [аппликонверсатионактионреспонсемессаже](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 **аппликонверсатионактионреспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**респонсекласс** <br/> | Описывает состояние ответа.<br/><br/>Для этого атрибута допустимы следующие значения:<ul><li>Успешно</li><li>Предупреждение</li><li>Ошибка</li></ul> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов Респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает запрос, который не был обработан. Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.<br/><br/>Ниже приведены примеры источников предупреждений.<ul><li>Хранилище Exchange находится в автономном режиме во время выполнения пакета.</li><li>Доменные службы Active Directory (AD DS) находятся в автономном режиме.</li><li>Почтовые ящики были перемещены.</li><li>База данных сообщений (MDB) находится в автономном режиме.</li><li>Истек срок действия пароля.</li><li>Превышена квота.</li></ul> |
|**Error** <br/> | Описывает запрос, который не может быть выполнен.<br/><br/>Ниже приведены примеры источников ошибок.  <ul><li>Недопустимые атрибуты или элементы</li><li>Атрибуты или элементы, которые выходят за пределы диапазона</li><li>Неизвестный тег  </li><li>Атрибут или элемент, который не является допустимым в контексте</li><li>Попытки несанкционированного доступа, выполняемые любым клиентом</li><li>Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</li></ul>Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.  <br/> |
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для будущего использования. Этот элемент содержит значение 0.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Содержит ответные сообщения для запроса веб-служб Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
### <a name="version-differences"></a>Различия версий

В версиях Exchange, начиная с сборки 15.00.0986.00, элемент **аппликонверсатионактионреспонсемессаже** имеет тип **аппликонверсатионактионреспонсемессажетипе**. В предыдущих версиях элемент относится к типу **респонсемессажетипе**.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ApplyConversationAction](applyconversationaction-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

