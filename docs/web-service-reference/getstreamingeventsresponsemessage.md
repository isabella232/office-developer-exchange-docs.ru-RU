---
title: жетстреаминжевентсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: Элемент Жетстреаминжевентсреспонсемессаже содержит состояние и результат одного запроса операции GetStreamingEvents.
ms.openlocfilehash: 055fb7eeb12e241739eb860cecbe398b8a322bd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459148"
---
# <a name="getstreamingeventsresponsemessage"></a>жетстреаминжевентсреспонсемессаже

Элемент **жетстреаминжевентсреспонсемессаже** содержит состояние и результат одного запроса [операции GetStreamingEvents](getstreamingevents-operation.md) . 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 **жетстреаминжевентсреспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**респонсекласс** <br/> | Описывает состояние ответа [операции GetStreamingEvents](getstreamingevents-operation.md) . <br/><br/>Для этого атрибута допустимы следующие значения:  <br/><br/>Успешное выполнение  <br/>— Предупреждение  <br/>— Ошибка  <br/> |
   
#### <a name="responseclass-attribute"></a>Атрибут Респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|Успешно  <br/> |Описывает выполненный запрос.  <br/> |
|Предупреждение  <br/> | Описывает запрос, который не был обработан. Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение. <br/><br/>Ниже приведены примеры источников предупреждений.  <br/><br/>— Хранилище Exchange находится в автономном режиме во время выполнения пакета.  <br/>-Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>— Почтовые ящики были перемещены.  <br/>— База данных почтовых ящиков (MDB) находится в автономном режиме.  <br/>— Срок действия пароля истек.  <br/>— Превышена квота.  <br/> |
|Ошибка  <br/> | Описывает запрос, который не может быть выполнен. <br/><br/>Ниже приведены примеры источников ошибок.  <br/><br/>— Недопустимые атрибуты или элементы  <br/>— Атрибуты или элементы, которые выходят за пределы допустимого диапазона  <br/>— Неизвестный тег  <br/>— Атрибут или элемент, который не является допустимым в контексте  <br/>— Попытки несанкционированного доступа, выполняемые любым клиентом;  <br/>— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента  <br/><br/>  Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.  <br/> |
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для последующего использования. Он содержит значение 0.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
|[Уведомления](notifications.md) <br/> |Содержит список сведений о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
|[еррорсубскриптионидс](errorsubscriptionids.md) <br/> |Содержит список недопустимых идентификаторов подписки.  <br/> |
|[ConnectionStatus](connectionstatus.md) <br/> |Предоставляет текстовое описание состояния попотоковой подписки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Содержит ответные сообщения для запроса веб-служб Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [GetStreamingEvents](getstreamingevents.md) 
- [жетстреаминжевентсреспонсе](getstreamingeventsresponse.md)
- [Операция GetStreamingEvents](getstreamingevents-operation.md)

