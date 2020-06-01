---
title: вебклиентреадформкуеристринг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WebClientReadFormQueryString
api_type:
- schema
ms.assetid: 13e8871a-32a6-4bb9-9493-864c4c07efff
description: Элемент Вебклиентреадформкуеристринг представляет URL-адрес для сцепления с конечной точкой Outlook Web App для чтения элемента в Outlook Web App.
ms.openlocfilehash: d7102ef288c0aafa6cdada09eda321b546edddb7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464982"
---
# <a name="webclientreadformquerystring"></a>вебклиентреадформкуеристринг

Элемент **вебклиентреадформкуеристринг** представляет URL-адрес для сцепления с конечной точкой Outlook Web App для чтения элемента в Outlook Web App. 
  
```XML
<WebClientReadFormQueryString/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент POST в хранилище Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

При использовании этого элемента необходимо указать текстовое значение, представляющее строку.
  
## <a name="remarks"></a>Примечания

Идентификатор элемента для URL-адреса Outlook Web App — это идентификатор EWS элемента. Можно использовать URL-кодирование идентификатора элемента EWS и добавить его в строку запроса, чтобы получить URL-адрес Outlook Web App для элемента.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
### <a name="version-differences"></a>Различия версий

Версии Exchange, начинающиеся с основной версии 15 и заканчивающейся на сервере Exchange Server 2013 Build 15.0.775.38 (CU3) и Exchange Online версии 15.00.0775.009, не возвращают соответствующий фрагмент строки запроса в элементе **вебклиентреадформкуеристринг** . 
  
В более ранних версиях Exchange идентификатор элемента для URL-адресов Outlook Web App — это идентификатор Outlook Web App. Если вы нацелены на более раннюю версию Exchange, чем основная версия 15, необходимо использовать [операцию ConvertId](convertid-operation.md) для преобразования идентификатора. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

