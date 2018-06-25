---
title: WebClientReadFormQueryString
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
description: Элемент WebClientReadFormQueryString представляет URL-адрес для объединения в конечную точку Outlook Web App для чтения элемента в Outlook Web App.
ms.openlocfilehash: 8096c14956d132a631b0ade6f2eae12a2bff9c06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840495"
---
# <a name="webclientreadformquerystring"></a>WebClientReadFormQueryString

Элемент **WebClientReadFormQueryString** представляет URL-адрес для объединения в конечную точку Outlook Web App для чтения элемента в Outlook Web App. 
  
```XML
<WebClientReadFormQueryString/>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент post в хранилище Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее строку является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Идентификатор элемента для URL-адрес Outlook Web App — это веб-служб Exchange идентификатор элемента. Можно кодировать URL-адрес идентификатор элемента веб-служб Exchange и добавить его в строку запроса, чтобы получить URL-адрес Outlook Web App для элемента.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
### <a name="version-differences"></a>Различия версий

Версии Exchange, начиная с версии 15 и Exchange Server 2013 построения 15.0.775.38 (CU3) и Exchange Online версии 15.00.0775.009 не возвращают фрагмента строка правильный запроса в элементе **WebClientReadFormQueryString** . 
  
В версиях Exchange до 15 основной номер версии идентификатор элемента для URL-адреса Outlook Web App — это идентификатор Outlook Web App. Если вы используете версия Exchange более ранних чем основной номер версии 15, необходимо преобразовать идентификатор с помощью [операции ConvertId](convertid-operation.md) . 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

