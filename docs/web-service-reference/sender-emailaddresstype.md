---
title: Отправитель (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 717eb6d0-d167-4b20-92e2-5d08b96186c4
description: Элемент sender представляет адрес электронной почты отправителя сообщения.
ms.openlocfilehash: 23a487f216a110796d40f3d3e86224c691acc004
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455326"
---
# <a name="sender-emailaddresstype"></a>Отправитель (EmailAddressType)

Элемент **sender** представляет адрес электронной почты отправителя сообщения. 
  
```XML
<Sender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Sender>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (EmailAddressType)](name-emailaddresstype.md) <br/> |Представляет имя пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md) <br/> |Определяет основной SMTP-адрес пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[Раутингтипе (EmailAddress)](routingtype-emailaddress.md) <br/> |Представляет протокол маршрутизации для получателя. По умолчанию используется значение SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Представляет тип почтового ящика, представленного адресом электронной почты. Этот элемент является необязательным.  <br/> |
|[Идентификатор](itemid.md) <br/> |Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Задает условия для типов сообщений, которые требуется найти.  <br/> |
|[мессажетраккингсеарчресулт](messagetrackingsearchresult.md) <br/> |Содержит один результат одного сообщения для элемента [финдмессажетраккингрепортреспонсе](findmessagetrackingreportresponse.md) .  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

