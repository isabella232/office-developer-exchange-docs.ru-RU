---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: Элемент AttendeeType обозначает тип участника, указанного в элементе Электронной почты (EmailAddressType). Этот элемент используется в запросах, которые содержат предложения о собраниях.
ms.openlocfilehash: a08532ed78296102ee252c1e0c40beee7ca8ea5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761520"
---
# <a name="attendeetype"></a>AttendeeType

Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **AttendeeType** обозначает тип участника, указанного в элементе [Электронной почты (EmailAddressType)](email-emailaddresstype.md). Этот элемент используется в запросах, которые содержат предложения о собраниях. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
- [AttendeeType](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 **MeetingAttendeeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.
  
|**Значение**|**Описание**|
|:-----|:-----|
|Organizer  <br/> |Пользователь почтового ящика и участник, который создал элемент календаря.  <br/> |
|Required  <br/> |Пользователь почтового ящика, который входит в число обязательных участников собрания.  <br/> |
|Optional  <br/> |Пользователь почтового ящика, который не входит в число обязательных участников собрания.  <br/> |
|Room  <br/> |Объект почтового ящика, который указывает на помещение для проведения собрания.  <br/> |
|Resource  <br/> |Оборудование, которое будет использоваться во время собрания, например, телевизор или проектор.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент относится к обязательным дочерним элементам элемента [MailboxData](mailboxdata.md). Он упоминается в [MailboxData](mailboxdata.md) только один раз. Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа. 
  
> [!NOTE]
> [!Примечание] Тип схемы AttendeeType используется для включения сведений об участниках в элемент календаря. Не путайте этот элемент с элементами типа схемы AttendeeType. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

