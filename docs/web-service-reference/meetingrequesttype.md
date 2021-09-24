---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: Элемент MeetingRequestType описывает тип запроса собрания.
ms.openlocfilehash: 1a8371331691bb9dee5595b0130ec0c3c75c47c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539376"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

Элемент **MeetingRequestType** описывает тип запроса собрания. 
  
```xml
<MeetingRequestType/>
```

 **MeetingRequestTypeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. В следующей таблице перечислены возможные текстовые значения для этого элемента.
  
|**Значение**|**Описание**|
|:-----|:-----|
|FullUpdate  <br/> |Определяет запрос собрания как полное обновление существующего запроса. Полное обновление обновило время и информационный контент.  <br/> |
|InformationalUpdate  <br/> |Определяет запрос собрания только как содержащий обновленный информационный контент.  <br/> |
|NewMeetingRequest  <br/> |Определяет запрос собрания в качестве нового запроса на собрание.  <br/> |
|Нет  <br/> |Указывает, что тип запроса собрания не определен.  <br/> |
|Устаревшие  <br/> |Определяет запрос собрания как устаревший.  <br/> |
|PrincipalWantsCopy  <br/> |Указывает, что запрос на собрание принадлежит директору, который переназначил сообщения собрания делегату и его копии помечены как информационные.  <br/> |
|SilentUpdate  <br/> |Определяет запрос собрания как тихое обновление существующего собрания.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

