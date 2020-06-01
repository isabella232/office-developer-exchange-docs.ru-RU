---
title: Create (Итемсинк)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: Элемент create определяет отдельный элемент для создания в локальном хранилище клиента.
ms.openlocfilehash: b9c0f28333594a6c17ee9581a227fc4773874fd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460801"
---
# <a name="create-itemsync"></a>Create (Итемсинк)

Элемент **CREATE** определяет отдельный элемент для создания в локальном хранилище клиента. 
  
- [синкфолдеритемсреспонсе](syncfolderitemsresponse.md) 
- [респонсемессажес](responsemessages.md) 
- [синкфолдеритемсреспонсемессаже](syncfolderitemsresponsemessage.md) 
- [Изменения (элементы)](changes-items.md) 
- [Create (Итемсинк)](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

```xml
<Create>
   <Task/> 
</Create>
```

```xml
<Create>
   <MeetingResponse/>
</Create>
```

```xml
<Create>
   <CalendarItem/>
</Create>
```

```xml
<Create>
   <MeetingMessage/>
</Create>
```

```xml
<Create>
   <DistributionList/>
</Create>
```

```xml
<Create>
   <MeetingCancellation/>
</Create>
```

```xml
<Create>
   <MeetingRequest/> 
</Create>
```

```xml
<Create>
   <Message/> 
</Create>
```

```xml
<Create>
   <Contact/> 
</Create>
```

**синкфолдеритемскреатеорупдатетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ресурс](item.md) <br/> |Представляет общий элемент Exchange для создания.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет создаваемое сообщение электронной почты Exchange.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange, который необходимо создать.  <br/> |
|[контакт](contact.md); <br/> |Представляет элемент контакта Exchange, который необходимо создать.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет создаваемый список рассылки.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет создаваемое сообщение о собрании.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание, которое требуется создать.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание, который требуется создать.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания, которое необходимо создать.  <br/> |
|[Task](task.md) <br/> |Представляет задачу, которую необходимо создать.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Изменения (элементы)](changes-items.md) <br/> |Содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция SyncFolderItems](syncfolderitems-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

