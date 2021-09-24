---
title: Предложите новое время собрания с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Узнайте, как предлагать новое время собраний из Exchange клиентского приложения с помощью EWS в Exchange.
ms.openlocfilehash: a6406aaef2005e74165e647510af891d2a59503e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522231"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a>Предложите новое время собрания с помощью EWS в Exchange

Узнайте, как предлагать новое время собраний из Exchange клиентского приложения с помощью EWS в Exchange.
  
Предлагаемая новая функция времени позволяет участникам предлагать организатору собрания новое время собраний в рамках рабочего процесса Exchange календаря. Если участник предлагает новое собрание, организатор может использовать предлагаемое новое время собрания для обновления собрания и отправки обновлений всем участникам. Прежде чем разрешить участникам предлагать новое время собраний, необходимо определить, разрешает ли организатор предлагать новое время. В этой статье описывается, как определить, можно ли предложить новое время и как использовать EWS для предложения нового времени.
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a>Определите, можно ли предложить новое время собрания с помощью EWS
<a name="bk_Determine"> </a>

Прежде чем предложить новое время для собрания, необходимо найти ссылку на это собрание и определить, настроен ли организатор собрания на поддержку предложений о новом времени. Вы можете получить ссылку на собрание, делая один из следующих: 
  
- Поиск запроса на собрание в почтовом ящике
    
- Поиск встречи в календаре
    
Чтобы найти ссылку на собрание, используйте следующие действия:
  
1. Чтобы найти целевой запрос на собрание или элемент календаря, используйте операцию [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS (или метод [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) EWS Managed API). Кроме того, вы можете использовать операцию [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS для получения идентификатора целевого запроса собрания или элемента календаря. 
    
2. Анализ результатов операции **FindItem** (или метода **Folder.FindItems),** чтобы получить идентификатор элемента элемента собрания. 
    
3. Чтобы получить объекты ответа для собрания, используйте операцию [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS. 
    
В следующем XML показано, что отправляется для запроса объектов ответа на элементе.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Ответ **на операцию GetItem** будет похож на следующий XML при запросе идентификатора элемента, времени начала и окончания собрания, коллекции объектов ответа, а также если организатор допускает предлагаемые изменения в время собрания. Коллекция объектов ответа, представленная элементом [ResponseObjects,](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) содержит набор ответов, допустимый для элемента календаря. Элемент **SuggestNewTime** — это объект отклика, который указывает, что пользователь может предложить новое время для собрания. Элементы [AcceptItem,](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx) [TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)и [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) представляют объекты отклика, которые можно использовать для предложения организатору собрания нового времени собрания. 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="propose-a-new-meeting-time-by-using-ews"></a>Предложить новое время собрания с помощью EWS
<a name="bk_Propose"> </a>

Если вы получили объект **response SuggestNewTime,** когда вы использовали операцию **GetItem** для получения элемента календаря или запроса на собрание, вы можете ответить предлагаемым новым временем собрания. Если вы не получили объект **ответа SuggestNewTime,** вы не сможете предложить новое время собрания в рамках рабочего процесса календаря. Однако вы можете ответить организатору на запрос нового времени собрания. Если вы получаете **объект response SuggestNewTime,** вы можете ответить на собрание ссылками на его идентификатор и предложить организатору новое время собрания. В этом случае **объект ответа SuggestNewTime** отличается от типичного шаблона объекта ответа в том, что вы не отвечаете объектом **ответа SuggestNewTime.** Вы используете один из других объектов ответа на собрания, например **AcceptItem,** **TentativelyAcceptItem** или **DeclineItem,** чтобы предложить новое собрание. В этом примере используется **объект ответа AcceptItem.** 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Ответ на этот запрос содержит идентификатор элемента календаря, добавленного в календарь участника, и копию запроса собрания, размещенного в папке удаленных элементов участника. Сообщение ответа с предложением о новом времени также сохранено в папке Отправленные элементы участника (для получения ручки необходимо найти сообщение ответа на собрание).
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Организатор получит сообщение [MeetingResponse,](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) когда участник ответит предложенным новым временем собрания. Сообщение **MeetingResponse** содержит предлагаемое новое время начала и окончания собрания и идентификатор связанного элемента календаря в календаре организатора. Организатор может использовать эти сведения для обновления существующего элемента календаря для собрания. Ниже приводится рабочий процесс для организатора для ответа на сообщение **MeetingResponse,** которое предлагает новое время собрания: 
  
1. Определите, заданы ли элементы **ProposedStart** или **ProposedEnd** в **MeetingResponse.** Если да, перейдите на шаг 2. Если нет, **в сообщении MeetingResponse** указывается только, принял ли, предварительно принял или отклонил собрание. 
    
2. Получите существующий элемент календаря организатора для собрания с помощью идентификатора EWS, возвращенного в **элементе AssociatedCalendarItemId.** 
    
3. Сравните исходное время начала и окончания с предлагаемым новым временем собрания. Если предлагаемое новое время собрания приемлемо для организатора, перейдите к шагу 4. В противном случае организатор собрания может либо проигнорировать предлагаемое время собрания, либо отправить ответ по электронной почте участнику, который предложил новое время собрания.
    
4. (Необязательный) Выполните [вызов операции GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS, чтобы узнать, будет ли предложенное время работать для всех участников, включая почтовые ящики комнат и ресурсов. (Для этого также можно использовать метод Управляемого API [API ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS.) 
    
5. Затем организатор может обновить собрание с новыми предлагаемыми временем собраний и отправить обновления всем участникам с помощью операции [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS (или метода Managed API EWS [Appointment.Update).](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) 
    
На следующем рисунке показан процесс, который происходит между организатором собрания, участниками и сервером Exchange, обрабатываемом вызовами EWS.
  
**Рис. 1. Процесс предложения нового времени собрания**

![На рисунке показан рабочий процесс между организатором, Exchange и участником, когда предлагается новое время собрания. если организатор разрешил предложения новых собраний, участник может предложить новое время собрания с помощью объекта ответа.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a>Различия версий
<a name="bk_Behavior"> </a>

Предлагаемая новая функция времени была представлена в Exchange версии сборки 15.00.0800.007. В более ранних версиях Exchange пользователям приложений EWS необходимо отправить организатору собрания отдельное электронное письмо, чтобы запросить другое время собрания. 
  
## <a name="see-also"></a>См. также


- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013 г.](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Встреча и собрания с помощью EWS в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Удаление встреч и отмена собраний с помощью EWS в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

