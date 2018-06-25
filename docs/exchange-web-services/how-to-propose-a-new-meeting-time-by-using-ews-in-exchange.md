---
title: Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Узнайте, как предложение нового времени из клиентского приложения Exchange с помощью веб-служб Exchange в Exchange.
ms.openlocfilehash: f9edd8511332474a728635a6aa369a772da24786
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761097"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a>Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange

Узнайте, как предложение нового времени из клиентского приложения Exchange с помощью веб-служб Exchange в Exchange.
  
Новая функция время предложить позволяет участникам предложение нового времени для организатора собрания в рамках процесса календаря Exchange. При участником предлагает нового собрания, организатором можно использовать предлагаемого нового собрания для обновления собрания и отправить обновления всем участникам. Прежде чем можно будет включить участникам предлагать другое время собрания, необходимо определить, позволяет ли организатора для новых предложений по времени. В этой статье описывается, как определить, является ли может предложить новый времени и использование веб-служб Exchange для предложение нового времени.
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a>Определить, является ли может предложить новое время собрания с помощью веб-служб Exchange
<a name="bk_Determine"> </a>

Прежде чем предлагать новые времени проведения собрания, необходимо найти ссылки на эти собрания и определить, настроен ли Организатор собрания для поддержки новых предложений по времени. Можно получить ссылку на собрание, выполните одно из следующих: 
  
- Поиск приглашения на собрание в папке "Входящие"
    
- Поиск встречи в календаре
    
Чтобы найти ссылки на собрания, выполните следующие действия:
  
1. Используйте операции EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (или метод [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) управляемый API EWS) для нахождения цели собрания элемента календаря или запроса. Кроме того можно использовать операцию [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS для получения идентификатора конечного, элемента календаря или запрос на собрания. 
    
2. Синтаксический анализ результаты операции **FindItem** (или метод **Folder.FindItems** ) для получения элемента идентификатор элемента собрания. 
    
3. Получение объектов ответа для собрания с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) веб-служб Exchange. 
    
В следующем XML показывается, что отправляется запрос объекты ответа на элемент.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ResponseObjects"/>
          <t:FieldURI FieldURI="item:Subject"/>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

Ответа операции **GetItem** будет выглядеть следующий XML-код, если запрос идентификатор элемента, собрания начала и время окончания, коллекции объектов ответа и организатора обеспечивает предложенного изменения во время собрания. Коллекцию объектов ответа, которая представляется элемент [ResponseObjects](http://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) , содержит набор ответов, подходящие для элемента календаря. Элемент **ProposeNewTime** — это объект ответа, которое указывает, что пользователь может предложить новое время собрания. Элементы [AcceptItem](http://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](http://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)и [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) представляют объекты ответа, которые можно использовать для предложение нового времени проведения собрания для организатора собрания. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
              <t:Subject>Competitive analysis: kick off meeting</t:Subject>
              <t:ResponseObjects>
                <t:AcceptItem/>
                <t:TentativelyAcceptItem/>
                <t:DeclineItem/>
                <t:ProposeNewTime/>
                <t:ReplyToItem/>
                <t:ReplyAllToItem/>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2013-11-09T17:00:00Z</t:Start>
              <t:End>2013-11-09T17:30:00Z</t:End>
            </t:MeetingRequest>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="propose-a-new-meeting-time-by-using-ews"></a>Предложение нового времени проведения собрания с помощью веб-служб Exchange
<a name="bk_Propose"> </a>

Если объект ответа **ProposeNewTime** полученные при использовании операции **GetItem** для получения элемента календаря или приглашения на собрание, он может ответить с предлагаемого нового собрания. Если вы не получите объект ответа **ProposeNewTime** , не будут иметь возможность предложить новое время собрания в рамках процесса календаря. Тем не менее, можно ответить Организатор для запроса нового времени проведения собрания. Если вы получите объект ответа **ProposeNewTime** , ответ на приглашение на собрание с учетом его идентификатор и предложение нового времени проведения собрания организатора. Это, где объект ответа **ProposeNewTime** отличается от шаблона объекта типичного ответа, то есть не отвечает с объектом ответа **ProposeNewTime** . Используйте один из другой собрания объекты ответа, например **AcceptItem**, **TentativelyAcceptItem**или **DeclineItem**предложение нового собрания. В этом примере используется объект ответа **AcceptItem** . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:CreateItem>
      <m:Items>
        <t:AcceptItem>
          <t:Body BodyType="Text">This time works better for the HiPPO.</t:Body>
          <t:ReferenceItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
          <t:ProposedStart>2013-11-28T04:00:00Z</t:ProposedStart>
          <t:ProposedEnd>2013-11-28T04:30:00Z</t:ProposedEnd>
        </t:AcceptItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Ответ на этот запрос содержит идентификатор элемента календаря, который был добавлен в календаре участника и копию приглашения на собрание, помещенные в папку Deleted Items участника. Сообщение ответа с помощью нового предложения времени также был сохранен в папке "Отправленные" участника (требуется найти собрания ответное сообщение для получения дескриптора на нем).
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAGRmOWE2OWAAA=" ChangeKey="DwAAJsmU"/>
            </t:CalendarItem>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkAGRmOWE2AAABB=" ChangeKey="AAAGJu1A"/>
            </t:MeetingRequest>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

Организатор будет [MeetingResponse](http://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) при сообщение участника отвечает предлагаемого нового собрания. Сообщение **MeetingResponse** содержит предлагаемого нового собрания время начала и время окончания и идентификатор элемента связанного календаря в календарь организатора. Организатор можно использовать эти сведения для обновления их существующего элемента календаря для собрания. Далее представлен рабочий процесс для организатора ответ на сообщение **MeetingResponse** , которая предлагает собрание: 
  
1. Определите, будет ли **ProposedStart** или **ProposedEnd** элементов были установлены в **MeetingResponse**. Если это так, перейдите к шагу 2. В противном случае сообщение **MeetingResponse** только указывает, ли участником принято, под вопросом или отклонил приглашение на собрание. 
    
2. Получите существующего элемента календаря организатора собрания с помощью идентификатора веб-служб Exchange, возвращаемых в элементе **AssociatedCalendarItemId** . 
    
3. Сравнение исходного начала и время окончания предложенного новое время собрания. Если предложенные новые собрания допустима организатора, перейдите к шагу 4. В противном случае Организатор собрания можно игнорировать назначенное время собрания, или отправить ответ по электронной почте участника, предложенное новое время собрания.
    
4. (Необязательно) Выполните вызов операции веб-служб Exchange [GetUserAvailability](http://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) , чтобы узнать, совместимо ли предложенного времени будут работать для всех участников, включая почтовые ящики оборудования и ресурсов. (Вы можно также использовать метод [ExchangeService.GetUserAvailability](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) управляемый API EWS для этого.) 
    
5. Организатор можно обновлять их собрания с помощью нового предложенного времени и отправлять обновления всех участников с помощью операции EWS [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) (или метод управляемый API EWS [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) ). 
    
На следующем рисунке показана процесс, который происходит между Организатор собрания, участником и на сервере Exchange, обрабатывать вызовы веб-служб Exchange.
  
**На рисунке 1. Процесс предложение нового времени проведения собрания**

![На рисунке показан рабочий процесс между организатором, Exchange и участником, когда предлагается новое время собрания. если организатор разрешил предложения новых собраний, участник может предложить новое время собрания с помощью объекта ответа.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a>Различия версий
<a name="bk_Behavior"> </a>

Новая функция время предложить была представлена в версии Exchange построения 15.00.0800.007. В более ранних версиях Exchange пользователи приложений веб-служб Exchange должны отправлять отдельные электронной почты организатора собрания для запроса другое время собрания. 
  
## <a name="see-also"></a>См. также


- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Получение встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

