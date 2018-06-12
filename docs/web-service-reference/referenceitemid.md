---
title: ReferenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReferenceItemId
api_type:
- schema
ms.assetid: 8fd4bb12-a94b-43f5-be3b-f435684e311d
description: Элемент ReferenceItemId определяет элемент, к которому относится объект ответа.
ms.openlocfilehash: d29f2dfec8f2c23fe0ac8c84d2bb9029fce613d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835032"
---
# <a name="referenceitemid"></a>ReferenceItemId

Элемент **ReferenceItemId** определяет элемент, к которому относится объект ответа. 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|
  **Id** <br/> |Идентифицирует определенного элемента в хранилище Exchange.  <br/> |
|**ChangeKey** <br/> |Идентифицирует определенной версии элемента.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[AcceptSharingInvitation](acceptsharinginvitation.md) <br/> |Представляет ответ на Accept для приглашения на общий доступ.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Представляет объект ответа, которая используется для отмены собрания.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Представляет отклонить ответ на приглашения на собрание.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Содержит элемент хранилища Exchange переадресация получателям.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Содержит ответить всем получателям определенного элемента в хранилище Exchange.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Содержит ответ создателем элемента в хранилище Exchange.  <br/> |
|[SuppressReadReceipt](suppressreadreceipt.md) <br/> |Используется для ответа на чтение запросов уведомлений.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Представляет под вопросом ответ на приглашения на собрание.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

