---
title: Получение встреч и собраний с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bae582a-8cb3-4e77-be2a-7e107fad26fe
description: Сведения о том, как получать встречи и собрания с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: c78d70ca2266bd192b82f644d902ad8c958d2d4a
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353695"
---
# <a name="get-appointments-and-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="fa76a-103">Получение встреч и собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="fa76a-103">Get appointments and meetings by using EWS in Exchange</span></span>

<span data-ttu-id="fa76a-104">Сведения о том, как получать встречи и собрания с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa76a-104">Learn how to get appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="fa76a-105">Вы можете получать встречи и собрания из папки "Календарь", используя метод управляемого API [календарфолдер. FindAppointments](http://msdn.microsoft.com/en-us/library/dd636179%28v=exchg.80%29.aspx) EWS или операцию [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="fa76a-105">You can retrieve appointments and meetings from a calendar folder by using the [CalendarFolder.FindAppointments](http://msdn.microsoft.com/en-us/library/dd636179%28v=exchg.80%29.aspx) EWS Managed API method or the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation.</span></span> 
  
## <a name="get-appointments-by-using-the-ews-managed-api"></a><span data-ttu-id="fa76a-106">Получение встреч с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="fa76a-106">Get appointments by using the EWS Managed API</span></span>
<span data-ttu-id="fa76a-107"><a name="bk_retrieveappsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fa76a-107"><a name="bk_retrieveappsEWSMA"> </a></span></span>

<span data-ttu-id="fa76a-108">В приведенном ниже примере кода показано, как использовать управляемый API EWS для получения встреч пользователя, которые находятся между заданным начальным и конечным временем.</span><span class="sxs-lookup"><span data-stu-id="fa76a-108">The following code example shows how to use the EWS Managed API to retrieve a user's appointments that fall between a specified start and end time.</span></span>
  
```cs
       // Initialize values for the start and end times, and the number of appointments to retrieve.
            DateTime startDate = DateTime.Now;
            DateTime endDate = startDate.AddDays(30);
            const int NUM_APPTS = 5;
            // Initialize the calendar folder object with only the folder ID. 
            CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
            // Set the start and end time and number of appointments to retrieve.
            CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
            // Limit the properties returned to the appointment's subject, start time, and end time.
            cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
            // Retrieve a collection of appointments by using the calendar view.
            FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
            Console.WriteLine("\nThe first " + NUM_APPTS + " appointments on your calendar from " + startDate.Date.ToShortDateString() + 
                              " to " + endDate.Date.ToShortDateString() + " are: \n");
            
            foreach (Appointment a in appointments)
            {
                Console.Write("Subject: " + a.Subject.ToString() + " ");
                Console.Write("Start: " + a.Start.ToString() + " ");
                Console.Write("End: " + a.End.ToString());
                Console.WriteLine();
            }

```

<br/>

<span data-ttu-id="fa76a-109">Ниже показан результат выполнения примера кода.</span><span class="sxs-lookup"><span data-stu-id="fa76a-109">The following is the output from the code example.</span></span>
  
```text
The first five appointments on your calendar from 8/21/2013 to 9/20/2013 are: 
  
Subject: Contoso devs team meeting Start: 8/21/2013 12:30:00 PM End: 8/21/2013 1:00:00 PM
  
Subject: Daily status meeting Start: 8/21/2013 1:00:00 PM End: 8/21/2013 2:00:00 PM
  
Subject: Lunch with sales team Start: 8/21/2013 2:30:00 PM End: 8/21/2013 3:30:00 PM
  
Subject: Tennis at the club Start: 8/22/2013 11:00:00 AM End: 8/22/2013 12:00:00 PM
  
Subject: Online training webcast: 8/22/2013 2:00:00 PM End: 8/22/2013 3:00:00 PM
```

## <a name="get-appointments-by-using-ews"></a><span data-ttu-id="fa76a-110">Получение встреч с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="fa76a-110">Get appointments by using EWS</span></span>
<span data-ttu-id="fa76a-111"><a name="bk_xml"> </a></span><span class="sxs-lookup"><span data-stu-id="fa76a-111"><a name="bk_xml"> </a></span></span>

<span data-ttu-id="fa76a-112">В следующем XML-коде показан запрос операции- [папки](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для возврата идентификатора папки для операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fa76a-112">The following XML shows a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request to return a folder ID for the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<br/>

<span data-ttu-id="fa76a-113">В приведенном ниже XML-коде показан ответ на **папку** .</span><span class="sxs-lookup"><span data-stu-id="fa76a-113">The following XML shows the **GetFolder** response.</span></span> <span data-ttu-id="fa76a-114">Обратите внимание, что атрибуты **FolderId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fa76a-114">Note that the **FolderID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:CalendarFolder>
              <t:FolderId Id="AAMk" ChangeKey="AgAA" />
            </t:CalendarFolder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<br/>

<span data-ttu-id="fa76a-115">В приведенном ниже XML-коде показан запрос **FindItem** , используемый для возврата запрошенных встреч.</span><span class="sxs-lookup"><span data-stu-id="fa76a-115">The following XML shows the **FindItem** request used to return the requested appointments.</span></span> <span data-ttu-id="fa76a-116">Обратите внимание, что атрибуты **FolderId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fa76a-116">Note that the **FolderID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-08-21T17:30:24.127Z" EndDate="2013-09-20T17:30:24.127Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAMk" ChangeKey="AgAA" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<br/>

<span data-ttu-id="fa76a-117">В следующем XML-коде показан ответ **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="fa76a-117">The following XML shows the **FindItem** response.</span></span> <span data-ttu-id="fa76a-118">Обратите внимание, что атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fa76a-118">Note that the **ItemID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="33" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Contoso devs team meeting</t:Subject>
                <t:Start>2013-08-21T19:30:00Z</t:Start>
                <t:End>2013-08-21T20:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Daily status meeting</t:Subject>
                <t:Start>2013-08-21T20:00:00Z</t:Start>
                <t:End>2013-08-21T21:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Lunch with sales team</t:Subject>
                <t:Start>2013-08-21T21:30:00Z</t:Start>
                <t:End>2013-08-21T22:30:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Tennis at the club</t:Subject>
                <t:Start>2013-08-22T18:00:00Z</t:Start>
                <t:End>2013-08-22T19:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA" ChangeKey="DwAA" />
                <t:Subject>Online training webcast</t:Subject>
                <t:Start>2013-08-22T21:00:00Z</t:Start>
                <t:End>2013-08-22T22:00:00Z</t:End>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="recurring-meetings-and-the-calendar-view"></a><span data-ttu-id="fa76a-119">Повторяющиеся собрания и представление календаря</span><span class="sxs-lookup"><span data-stu-id="fa76a-119">Recurring meetings and the calendar view</span></span>
<span data-ttu-id="fa76a-120"><a name="bk_recurring"> </a></span><span class="sxs-lookup"><span data-stu-id="fa76a-120"><a name="bk_recurring"> </a></span></span>

<span data-ttu-id="fa76a-121">Папка Calendar немного отличается от других папок в почтовом ящике, так как повторения в повторяющихся рядах и исключения в повторяющихся рядах не являются фактическими элементами в почтовом ящике, а хранятся внутренне как вложения в повторяющейся основной реплике.</span><span class="sxs-lookup"><span data-stu-id="fa76a-121">The calendar folder is a little different from other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master.</span></span> <span data-ttu-id="fa76a-122">Это означает, что несмотря на то, что вы можете создать запрос EWS, который возвращает значения между набором **начальных** и **конечных** значений, с помощью одного из методов перегрузки **FindItems** управляемого API EWS, таких как [EXCHANGESERVICE. FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или операция [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , EWS не просматривает таблицу вложений каждого элемента календаря для поиска исключений и вхождений.</span><span class="sxs-lookup"><span data-stu-id="fa76a-122">This means that although you can create an EWS request that returns values between a set of **start** and **end** values by using one of the EWS Managed API **FindItems** overload methods, such as [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or the EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, EWS would not look through the attachment table of every calendar item to find exceptions and occurrences.</span></span> 
  
<span data-ttu-id="fa76a-123">Вместо этого вы можете использовать объект *DataView* на объединении двух таблиц SQL с помощью объекта [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fa76a-123">Instead, what you really want to do is something akin to applying a  *Dataview*  onto a union of two SQL tables, using a [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="fa76a-124">Обратите внимание, что в целях повышения производительности мы рекомендуем использовать свойство [Property](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) , чтобы ограничить размер ответа, указав количество возвращаемых встреч и собраний, а также определенные свойства.</span><span class="sxs-lookup"><span data-stu-id="fa76a-124">Note that for performance reasons, we recommend that you use the [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) property to limit the size of the response by indicating the number of appointments or meetings you want returned, as well as the specific properties you want.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fa76a-125">См. также</span><span class="sxs-lookup"><span data-stu-id="fa76a-125">See also</span></span>
<span data-ttu-id="fa76a-126"><a name="bk_additional"> </a></span><span class="sxs-lookup"><span data-stu-id="fa76a-126"><a name="bk_additional"> </a></span></span>

- [<span data-ttu-id="fa76a-127">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="fa76a-127">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)   
- [<span data-ttu-id="fa76a-128">Создание встреч и собраний с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="fa76a-128">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [<span data-ttu-id="fa76a-129">Обновление встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fa76a-129">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="fa76a-130">Удаление встреч и отмена собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="fa76a-130">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="fa76a-131">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="fa76a-131">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

