---
title: ResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseType
api_type:
- schema
ms.assetid: cdc09dda-ce20-4504-880d-9da6025ca812
description: Элемент ResponseType представляет тип ответа получателя, полученный для собрания.
ms.openlocfilehash: ef8183b71e267a20427873ca44b269b828686cbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465396"
---
# <a name="responsetype"></a>ResponseType

Элемент **ResponseType** представляет тип ответа получателя, полученный для собрания. 
  
```xml
<ResponseType/>
```

 **респонсетипетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Участник](attendee.md) <br/> |Представляет участников и ресурсы собрания.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет сообщение о собрании в хранилище Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Ниже приведены возможные текстовые значения для этого элемента:
  
- Неизвестно
    
- Организатор
    
- Занят
    
- Accept
    
- Отклоня
    
- нореспонсерецеивед
    
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

