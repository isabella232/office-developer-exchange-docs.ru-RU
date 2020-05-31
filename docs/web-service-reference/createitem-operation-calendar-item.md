---
title: Операция CreateItem (элемент календаря)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: aa4a7c94-f668-4bd2-8079-c855f6ab17e1
description: Операция CreateItem создает элементы календаря в хранилище Exchange.
ms.openlocfilehash: c2174dd806b922e640ef7afcab32b98c67c65b41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761891"
---
# <a name="createitem-operation-calendar-item"></a>Операция CreateItem (элемент календаря)

Операция CreateItem создает элементы календаря в хранилище Exchange.
  
## <a name="remarks"></a>Примечания

Операция CreateItem создает встречи, собрания и приглашения на собрания. Если элемент календаря создан без участников, он считается встречей. Если указаны участники, элемент календаря является собранием. При создании собрания с помощью операции CreateItem приглашения на собрания автоматически отправляются определенным участникам, если для атрибута Сендмитингинвитатионс задано значение отправки приглашений на собрание.
  
## <a name="createitem-calendar-item-request-example"></a>Пример запроса CreateItem (элемента календаря)

### <a name="description"></a>Описание

В приведенном ниже примере запроса CreateItem показано, как создать собрание с двумя обязательными участниками. Этот запрос отправляет приглашения на собрание двум участникам.
  
### <a name="code"></a>Код

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                SendMeetingInvitations="SendToAllAndSaveCopy" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar"/>
      </SavedItemFolderId>
      <Items>
        <t:CalendarItem xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Planning Meeting</Subject>
          <Body BodyType="Text">Plan the agenda for next week's meeting.</Body>
          <ReminderIsSet>true</ReminderIsSet>
          <ReminderMinutesBeforeStart>60</ReminderMinutesBeforeStart>
          <Start>2006-11-02T14:00:00</Start>
          <End>2006-11-02T15:00:00</End>
          <IsAllDayEvent>false</IsAllDayEvent>
          <LegacyFreeBusyStatus>Busy</LegacyFreeBusyStatus>
          <Location>Conference Room 721</Location>
          <RequiredAttendees>
            <Attendee>
              <Mailbox>
                <EmailAddress>User1@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
            <Attendee>
              <Mailbox>
                <EmailAddress>User2@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
          </RequiredAttendees>
        </t:CalendarItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Пример ответа на приглашение на собрание представлен в разделе [Операция CreateItem (приглашение на собрание)](createitem-operation-meeting-request.md) . 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [CreateItem](createitem.md)
    
- [саведитемфолдерид](saveditemfolderid.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md)
    
- [календаритем](calendaritem.md)
    
- [Тема](subject.md)
    
- [Основной текст](body.md)
    
- [реминдериссет](reminderisset.md)
    
- [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)
    
- [Начало](start.md)
    
- [Оканчиваться](end-ex15websvcsotherref.md)
    
- [исаллдайевент](isalldayevent.md)
    
- [легацифрибусистатус](legacyfreebusystatus.md)
    
- [Location](location.md)
    
- [RequiredAttendees](requiredattendees.md)
    
- [Attendee](attendee.md)
    
- [Mailbox](mailbox.md)
    
- [EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a>Успешный отклик CreateItem (элемент календаря)

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос CreateItem.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAAlAFV" ChangeKey="DwAAABYA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Атрибуты **ID** и **чанжекэй** элемента [ItemId](itemid.md) были сокращены для сохранения удобочитаемости. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатеитемреспонсе](createitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеитемреспонсемессаже](createitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Items](items.md)
    
- [календаритем](calendaritem.md)
    
- [Идентификатор](itemid.md)
    
## <a name="see-also"></a>См. также



[Операция CreateItem](createitem-operation.md)

