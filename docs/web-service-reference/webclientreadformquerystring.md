---
title: WebClientReadFormQueryString
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- WebClientReadFormQueryString
api_type:
- schema
ms.assetid: 13e8871a-32a6-4bb9-9493-864c4c07efff
description: Элемент WebClientReadFormQueryString представляет URL-адрес, привнося в конечную точку Outlook Web App для чтения элемента в Outlook Web App.
ms.openlocfilehash: 10035aa001c74926ae36e96e09b5b2995844cb68
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538473"
---
# <a name="webclientreadformquerystring"></a>WebClientReadFormQueryString

Элемент **WebClientReadFormQueryString** представляет URL Outlook Web App для чтения элемента в Outlook Web App. 
  
```XML
<WebClientReadFormQueryString/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент столба в Exchange магазине.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если используется этот элемент, требуется текстовое значение, представляю которое представляет строку.
  
## <a name="remarks"></a>Заметки

Идентификатор элемента для url Outlook Web App является идентификатором элемента EWS. Вы можете кодировать URL-адрес идентификатора элемента EWS и примкните его к строке запроса, чтобы получить Outlook Web App URL-адрес элемента.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
### <a name="version-differences"></a>Различия версий

Версии Exchange начиная с основной версии 15 и заканчивая Exchange Server 2013 г. сборкой 15.0.775.38 (CU3) и Exchange Online версии 15.00.0775.009 не возвращают правильный фрагмент строки запроса в **элементе WebClientReadFormQueryString.** 
  
В версиях Exchange версии 15 идентификатор элемента для URL Outlook Web App является идентификатором Outlook Web App. Если вы нацелены на версию Exchange версии 15, для преобразования идентификатора необходимо использовать операцию [ConvertId.](convertid-operation.md) 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

