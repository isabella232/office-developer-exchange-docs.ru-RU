---
title: Предложение нового времени проведения собрания с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Сведения о том, как предлагать новое время проведения собрания из клиентского приложения Exchange с помощью EWS в Exchange.
ms.openlocfilehash: 4f001bb82d2325624b567412620283619b51f25b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456814"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a>Предложение нового времени проведения собрания с помощью EWS в Exchange

Сведения о том, как предлагать новое время проведения собрания из клиентского приложения Exchange с помощью EWS в Exchange.
  
Функция "предложить новое время" позволяет участникам предлагать новое время проведения собрания организатору собрания в рамках рабочего процесса календаря Exchange. Когда участник предлагает новое собрание, организатор может использовать предложенное новое время собрания для обновления собрания и отправки обновлений всем участникам. Прежде чем разрешить участникам предлагать новое время проведения собрания, необходимо определить, разрешает ли организатор новые предложения времени. В этой статье описывается, как определить, можно ли предложить новое время и как использовать EWS для предложения нового времени.
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a>Определите, можно ли предложить новое время для собрания с помощью EWS.
<a name="bk_Determine"> </a>

Прежде чем можно будет предложить новое время собрания, необходимо найти ссылку на это собрание и определить, будет ли организатор собрания настроил собрание для поддержки новых предложений времени. Ссылку на собрание можно получить, выполнив одно из следующих действий. 
  
- Поиск приглашения на собрание в папке "Входящие"
    
- Поиск встречи в календаре
    
Чтобы найти ссылку на собрание, выполните указанные ниже действия.
  
1. Используйте операцию [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS (или метод [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) , управляемый API EWS), чтобы найти целевое приглашение на собрание или элемент календаря. Кроме того, вы можете использовать операцию [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS, чтобы получить идентификатор целевого приглашения на собрание или элемента календаря. 
    
2. Выполните синтаксический анализ результатов операции **FindItem** (или метода **Folder. FindItems** ), чтобы получить идентификатор элемента собрания. 
    
3. Используйте операцию [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для получения объектов Response для собрания. 
    
В следующем XML-коде показано, что отправляется, чтобы запросить объекты ответа для элемента.
  
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

Отклик операции **GetItem** будет выглядеть аналогично следующему XML-коду, если вы запрашиваете идентификатор элемента, время начала и окончания собрания, коллекцию объектов Response и, если организатор допускает предложенные изменения времени собрания. Коллекция объектов Response, представленная элементом [респонсеобжектс](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) , содержит набор ответов, допустимых для элемента календаря. Элемент **пропосеневтиме** — это объект Response, указывающий на то, что пользователь может предложить новое время собрания. Элементы [акцептитем](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [тентативелякцептитем](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)и [деклинеитем](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) представляют объекты ответа, которые можно использовать для предложения нового времени собрания организатору собрания. 
  
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

## <a name="propose-a-new-meeting-time-by-using-ews"></a>Предложение нового времени проведения собрания с помощью EWS
<a name="bk_Propose"> </a>

Если вы получили объект Response **пропосеневтиме** при **использовании операции GetItem** для получения элемента календаря или приглашения на собрание, вы можете ответить на новое время собрания. Если вы не получили объект ответа **пропосеневтиме** , вы не сможете предложить новое время проведения собрания в рамках рабочего процесса календаря. Тем не менее, вы можете ответить организатору, чтобы запросить новое время проведения собрания. Если получен объект ответа **пропосеневтиме** , вы можете ответить на собрание, обратившись к его идентификатору, и предложить новому времени проведения собрания организатору. В этом случае объект ответа **пропосеневтиме** отличается от типичного шаблона объекта ответа, в котором вы не отвечаете на объект отклика **пропосеневтиме** . Для предложения нового собрания используется один из других объектов ответа на приглашение, например **акцептитем**, **тентативелякцептитем**или **деклинеитем**. В этом примере используется объект Response **акцептитем** . 
  
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

Ответ на этот запрос содержит идентификатор элемента календаря, который был добавлен в календарь участника, и копию приглашения на собрание, которое было размещено в папке "Удаленные" участника. Ответное сообщение с новым предложением времени также было сохранено в папке "Отправленные" участника (вам потребуется найти ответное сообщение о собрании, чтобы получить его дескриптор).
  
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

Организатор получит сообщение [митингреспонсе](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) , когда участник ответит на новое время собрания. Сообщение **митингреспонсе** содержит предложенное новое время начала собрания и время окончания, а также идентификатор связанного элемента календаря в календаре организатора. Организатор может использовать эти сведения для обновления существующего элемента календаря для собрания. Ниже приведен рабочий процесс для ответа организатора на сообщение **митингреспонсе** , которое предлагает новое время проведения собрания: 
  
1. Определите, были ли заданы элементы **ProposedStart** или **пропоседенд** в **митингреспонсе**. Если это так, перейдите к шагу 2. В противном случае сообщение **митингреспонсе** только указывает, принял ли участник приглашение, приняли приглашение или отклонил его. 
    
2. Получение существующего элемента календаря организатора для собрания с помощью идентификатора EWS, возвращенного в элементе **ассоЦиатедкалендаритемид** . 
    
3. Сравните начальное и конечное время с предложенным новым временем собрания. Если предложенное новое время собрания приемлемо для организатора, перейдите к шагу 4. В противном случае Организатор собрания может игнорировать предложенное время собрания или отправить ему сообщение электронной почты участнику, который предложил новое время проведения собрания.
    
4. Необязательно Выполните вызов операции [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS, чтобы узнать, будет ли предложенное время работать для всех участников, включая почтовые ящики помещений и ресурсов. Для этого можно также использовать метод управляемого API [ExchangeService. GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS. 
    
5. После этого организатор может обновить собрание с новым предполагаемым временем собрания и отправить обновления всем участникам с помощью операции [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS (или метода [встречи. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) Managed API EWS). 
    
На следующем рисунке показан процесс, выполняемый между организатором собрания, участником и сервером Exchange, который обработал вызовы EWS.
  
**Рис. 1. Процесс, с помощью которого вы предлагаете новое время проведения собрания**

![На рисунке показан рабочий процесс между организатором, Exchange и участником, когда предлагается новое время собрания. если организатор разрешил предложения новых собраний, участник может предложить новое время собрания с помощью объекта ответа.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a>Различия версий
<a name="bk_Behavior"> </a>

Функция "предложить новое время" была введена в версии сборки Exchange 15.00.0800.007. В более ранних версиях Exchange пользователям приложения EWS необходимо отправить отдельное сообщение электронной почты организатору собрания, чтобы запросить другое время собрания. 
  
## <a name="see-also"></a>См. также


- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Получение встреч и собраний с помощью EWS в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Удаление встреч и отмена собраний с помощью EWS в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

