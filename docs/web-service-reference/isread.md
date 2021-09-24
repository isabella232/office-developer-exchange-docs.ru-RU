---
title: IsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsRead
api_type:
- schema
ms.assetid: 161455d5-a870-4c99-b2eb-c759c538f1bc
description: Элемент IsRead указывает, было ли прочитано сообщение.
ms.openlocfilehash: cbd2fb90a413e1ec700cf07a11e0082a985545b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539397"
---
# <a name="isread"></a>IsRead

Элемент **IsRead** указывает, было ли прочитано сообщение. 
  
```XML
<IsRead/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент столба в Exchange магазине. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[ConversationAction](conversationaction.md) <br/> |Содержит одно действие, которое необходимо применить к одному разговору.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true указывает,** что сообщение было прочитано. Ложное **текстовое** значение указывает на то, что сообщение не было прочитано. 
  
## <a name="remarks"></a>Заметки

Если [isReadReceiptRequested](isreadreceiptrequested.md) является **верным,** параметр **IsRead** для **true** отправляет квитанцию о прочтение. Получатель может подавлять получение чтения, перед тем как установить свойство **IsRead,** перед отправкой объекта [ответа SuppressReadReceipt.](suppressreadreceipt.md) 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

