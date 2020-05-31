---
title: рецеиведби
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceivedBy
api_type:
- schema
ms.assetid: ac84c9c5-d2fe-4b6f-bf4d-0444131d835b
description: Элемент Рецеиведби идентифицирует делегат в сценарии доступа делегата.
ms.openlocfilehash: 7918fa3320223e5cf02dd225912adfae3181e29c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834969"
---
# <a name="receivedby"></a>рецеиведби

Элемент **рецеиведби** идентифицирует делегат в сценарии доступа делегата. 
  
```xml
<ReceivedBy>
   <Mailbox/>
</ReceivedBy>
```

 **синглереЦипиенттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
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
|[канцелкалендаритем](cancelcalendaritem.md) <br/> |Представляет объект ответа, которая используется для отмены собрания.  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **рецеиведрепресентинг** используется вместе с элементами **from** и **рецеиведби** в сценариях доступа делегата. В следующей таблице перечислены сущности, которые представляют эти элементы в сценарии доступа делегата. 
  
**Элементы в сценарии доступа делегата**

|**Элемент**|**Объект, который представляет элемент**|
|:-----|:-----|
|[From](from.md) <br/> |ThirdParty  <br/> |
|[рецеиведби](receivedby.md) <br/> |Делегат  <br/> |
|[рецеиведрепресентинг](receivedrepresenting.md) <br/> |Principal  <br/> |
   
Если в сценарии доступа делегата ThirdParty отправляет приглашение на собрание участнику с представителем, он увидит новое приглашение на собрание. Эти элементы позволяют представителям различать сообщения, отправленные непосредственно им, и сообщения, отправленные им из-за правила пересылки делегата.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

