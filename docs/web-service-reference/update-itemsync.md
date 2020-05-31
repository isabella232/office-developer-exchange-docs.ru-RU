---
title: Обновление (Итемсинк)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: Элемент Update определяет один элемент для обновления в локальном хранилище клиента.
ms.openlocfilehash: bf560f18184151a3f17d7016d05cdb725db934ae
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353632"
---
# <a name="update-itemsync"></a>Обновление (Итемсинк)

Элемент **Update** определяет один элемент для обновления в локальном хранилище клиента. 
  
- [синкфолдеритемсреспонсе](syncfolderitemsresponse.md) 
- [респонсемессажес](responsemessages.md)  
- [синкфолдеритемсреспонсемессаже](syncfolderitemsresponsemessage.md)  
- [Изменения (элементы)](changes-items.md)  
- [Обновление (Итемсинк)](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

```xml
<Update>
   <MeetingRequest/>
</Update>
```

```xml
<Update>
   <MeetingCancellation/>
</Update>
```

```xml
<Update>
   <Task/>
</Update>
```

```xml
<Update>
   <CalendarItem/>
</Update>
```

```xml
<Update>
   <MeetingResponse/>
</Update>
```

```xml
<Update>
   <Message/>
</Update>
```

```xml
<Update>
   <DistributionList/>
</Update>
```

```xml
<Update>
   <MeetingMessage/>
</Update>
```

```xml
<Update>
   <Contact/> 
</Update>
```

**синкфолдеритемскреатеорупдатетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент](item.md) <br/> |Представляет универсальный элемент Exchange, который необходимо обновить.  <br/> |
|[Сообщение](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange, которое требуется обновить.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange, который необходимо обновить.  <br/> |
|[контакт](contact.md); <br/> |Представляет элемент контакта Exchange, который необходимо обновить.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки, который необходимо обновить.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет сообщение о собрании, которое необходимо обновить.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание, которое требуется обновить.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание, который необходимо обновить.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания, которое необходимо обновить.  <br/> |
|[Task](task.md) <br/> |Представляет задачу, которую необходимо обновить.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Изменения (элементы)](changes-items.md) <br/> |Содержит массив последовательности типов изменений, представляющих тип различий между элементами на клиенте и элементами на сервере Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция SyncFolderItems](syncfolderitems-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

