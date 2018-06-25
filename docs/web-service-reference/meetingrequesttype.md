---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: Элемент MeetingRequestType описывает тип запроса на проведение собрания.
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834432"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

Элемент **MeetingRequestType** описывает тип запроса на проведение собрания. 
  
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

Текстовое значение является обязательным. В следующей таблице перечислены возможные значения для этого элемента.
  
|**Значение**|**Описание**|
|:-----|:-----|
|FullUpdate  <br/> |Определяет запрос на собрание как полное обновление для существующего запроса. Полное обновление обновил времени и информационного контента.  <br/> |
|InformationalUpdate  <br/> |Определяет запрос на собрание, содержащее обновления информационного контента.  <br/> |
|NewMeetingRequest  <br/> |Указывает запрос на собрание в качестве нового приглашения на собрание.  <br/> |
|Нет  <br/> |Указывает, что собрание тип не определен.  <br/> |
|Устаревшие  <br/> |Определяет запрос на собрание считается устаревшим.  <br/> |
|PrincipalWantsCopy  <br/> |Показывает, что запрос на собрание принадлежит участника, кто имеет свой копии, помеченные как информационные и перенаправление сообщений о собрании делегат.  <br/> |
|SilentUpdate  <br/> |Указывает запрос на собрание в качестве автоматической обновление для существующего собрания.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

