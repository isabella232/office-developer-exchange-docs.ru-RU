---
title: исреадрецеиптрекуестед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceiptRequested
api_type:
- schema
ms.assetid: 7ab6edd5-c7ed-4701-8de3-d7dc7ecfa9c2
description: Элемент Исреадрецеиптрекуестед указывает, запрашивает ли отправитель элемента уведомление о прочтении.
ms.openlocfilehash: e3db685fc4e72e4332eab4a95afb5f844d04c35e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834097"
---
# <a name="isreadreceiptrequested"></a>исреадрецеиптрекуестед

Элемент **исреадрецеиптрекуестед** указывает, запрашивает ли отправитель элемента уведомление о прочтении. 
  
```xml
<IsReadReceiptRequested/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[акцептитем](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[тентативелякцептитем](tentativelyacceptitem.md) <br/> |Представляет под вопросом ответ на приглашения на собрание.  <br/> |
|[деклинеитем](declineitem.md) <br/> |Представляет отклонить ответ на приглашения на собрание.  <br/> |
|[реплитоитем](replytoitem.md) <br/> |Содержит ответ создателем элемента в хранилище Exchange.  <br/> |
|[репляллтоитем](replyalltoitem.md) <br/> |Содержит ответить всем получателям определенного элемента в хранилище Exchange.  <br/> |
|[форвардитем](forwarditem.md) <br/> |Содержит элемент хранилища Exchange переадресация получателям.  <br/> |
|[канцелкалендаритем](cancelcalendaritem.md) <br/> |Представляет объект ответа, используемый для отмены собрания.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** указывает, что уведомление о прочтении запрашивается у получателя элемента. 
  
## <a name="remarks"></a>Примечания

Если **исреадрецеиптрекуестед** имеет **значение true**, параметру [Read](isread.md) to **true** отправляется уведомление о прочтении. Получатель может отключить уведомления о прочтении, отправив объект ответа [суппрессреадрецеипт](suppressreadreceipt.md) , прежде чем устанавливать свойство- **Read** . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

