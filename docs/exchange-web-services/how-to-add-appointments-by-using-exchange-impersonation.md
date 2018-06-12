---
title: Добавление встреч с использованием олицетворения Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Узнайте, как использовать олицетворение управляемый API EWS или веб-служб Exchange в Exchange на добавление встреч календарей пользователей.
ms.openlocfilehash: fe737658b88aca66d8b4c2860245db000888ba17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760997"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a><span data-ttu-id="ebfed-103">Добавление встреч с использованием олицетворения Exchange</span><span class="sxs-lookup"><span data-stu-id="ebfed-103">Add appointments by using Exchange impersonation</span></span>

<span data-ttu-id="ebfed-104">Узнайте, как использовать олицетворение управляемый API EWS или веб-служб Exchange в Exchange на добавление встреч календарей пользователей.</span><span class="sxs-lookup"><span data-stu-id="ebfed-104">Learn how to use impersonation with the EWS Managed API or EWS in Exchange to add appointments to users' calendars.</span></span>
  
<span data-ttu-id="ebfed-105">Можно создать приложения-службы, которая вставляет встреч непосредственно в календаре Exchange с помощью учетной записи службы, имеющей[роли включены](how-to-configure-impersonation.md) **AppplicationImpersonation**.</span><span class="sxs-lookup"><span data-stu-id="ebfed-105">You can create a service application that inserts appointments directly into an Exchange calendar by using a service account that has the **AppplicationImpersonation**[role enabled](how-to-configure-impersonation.md).</span></span> <span data-ttu-id="ebfed-106">При использовании олицетворения приложения используется в качестве пользователя; Это, как если бы пользователь добавлен встречи календаря с помощью клиента, такие как Outlook.</span><span class="sxs-lookup"><span data-stu-id="ebfed-106">When you use impersonation, the application is acting as the user; it's as if the user added the appointment to the calendar by using a client such as Outlook.</span></span> 
  
<span data-ttu-id="ebfed-107">При использовании олицетворения необходимо учитывать следующее:</span><span class="sxs-lookup"><span data-stu-id="ebfed-107">When you are using impersonation, keep in mind the following:</span></span>
  
- <span data-ttu-id="ebfed-108">Объект [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) должен быть привязан к учетной записи службы.</span><span class="sxs-lookup"><span data-stu-id="ebfed-108">Your [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) object must be bound to the service account.</span></span> <span data-ttu-id="ebfed-109">Можно использовать один и тот же объект **ExchangeService** для олицетворения нескольких учетных записей с помощью изменения свойства [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) для каждой учетной записи, которую требуется олицетворения.</span><span class="sxs-lookup"><span data-stu-id="ebfed-109">You can use the same **ExchangeService** object to impersonate multiple accounts by changing the [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property for each account that you want to impersonate.</span></span> 
    
- <span data-ttu-id="ebfed-110">Любой элемент, сохранять олицетворенным учетной записи может использоваться только один раз.</span><span class="sxs-lookup"><span data-stu-id="ebfed-110">Any item that you save to an impersonated account can only be used once.</span></span> <span data-ttu-id="ebfed-111">Если вы хотите сохранить же встречу в нескольких учетных записей, например, необходимо создать [объект для каждой учетной записи](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ebfed-111">If you want to save the same appointment in multiple accounts, for example, you have to create an [Appointment](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) object for each account.</span></span> 
    
## <a name="prerequisites"></a><span data-ttu-id="ebfed-112">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ebfed-112">Prerequisites</span></span>

<span data-ttu-id="ebfed-113">Приложению учетной записи, используемой для подключения к Exchange server для использования олицетворения.</span><span class="sxs-lookup"><span data-stu-id="ebfed-113">Your application needs an account to use to connect to the Exchange server before it can use impersonation.</span></span> <span data-ttu-id="ebfed-114">Рекомендуется использовать учетную запись службы для приложения, которому назначена роль олицетворения приложения для учетных записей, которые будут пользоваться.</span><span class="sxs-lookup"><span data-stu-id="ebfed-114">We suggest that you use a service account for the application that has been granted the Application Impersonation role for the accounts that it will be accessing.</span></span> <span data-ttu-id="ebfed-115">Дополнительные сведения можно [настроить олицетворения](how-to-configure-impersonation.md)</span><span class="sxs-lookup"><span data-stu-id="ebfed-115">For more information, see [Configure impersonation](how-to-configure-impersonation.md)</span></span>
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a><span data-ttu-id="ebfed-116">Добавление встреч с использованием олицетворения с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ebfed-116">Add appointments by using impersonation with the EWS Managed API</span></span>

<span data-ttu-id="ebfed-117">В следующем примере добавляется встречи или собрания в календарь одного или нескольких учетных записей Exchange.</span><span class="sxs-lookup"><span data-stu-id="ebfed-117">The following example adds an appointment or meeting to the calendar of one or more Exchange accounts.</span></span> <span data-ttu-id="ebfed-118">Метод принимает три параметра.</span><span class="sxs-lookup"><span data-stu-id="ebfed-118">The method takes three parameters.</span></span>
  
-  <span data-ttu-id="ebfed-119">_Служба_ — объект **ExchangeService** привязан к учетной записи приложения-службы на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="ebfed-119">_service_ — An **ExchangeService** object bound to the service application's account on the Exchange server.</span></span> 
    
-  <span data-ttu-id="ebfed-120">_emailAddresses_ — [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) object, содержащий список строк адресов электронной почты SMTP.</span><span class="sxs-lookup"><span data-stu-id="ebfed-120">_emailAddresses_ — A [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) object containing a list of SMTP email address strings.</span></span> 
    
-  <span data-ttu-id="ebfed-121">_фабрика_ — это объект, реализующий интерфейс **IAppointmentFactory** .</span><span class="sxs-lookup"><span data-stu-id="ebfed-121">_factory_ — An object that implements the **IAppointmentFactory** interface.</span></span> <span data-ttu-id="ebfed-122">Этот интерфейс содержит один метод **GetAppointment** , который принимает объект **ExchangeService** как параметр и возвращает объект **встречи** .</span><span class="sxs-lookup"><span data-stu-id="ebfed-122">This interface has one method, **GetAppointment** that takes an **ExchangeService** object as a parameter and returns an **Appointment** object.</span></span> <span data-ttu-id="ebfed-123">Интерфейс **IAppointmentFactory** определен [интерфейс IAppointmentFactory](#bk_IAppointmentFactory).</span><span class="sxs-lookup"><span data-stu-id="ebfed-123">The **IAppointmentFactory** interface is defined [IAppointmentFactory interface](#bk_IAppointmentFactory).</span></span>
    
```cs
private static void CreateAppointments(ExchangeService service, List<string> emailAddresses, IAppointmentFactory factory)
{
  // Loop through the list of email addresses to add the appointment.
  foreach (var emailAddress in emailAddresses)
  {
    Console.WriteLine(string.Format("  Placing appointment in calendar for {0}.", emailAddress));
    // Set the email address of the account to get the appointment.
    service.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, emailAddress);
    // Get the appointment to add.
    Appointment appointment = factory.GetAppointment(service);
    // Save the appointment.
    try
    {
      if (appointment.RequiredAttendees.Count > 0)
      {
        // The appointment has attendees so send them the meeting request.
        appointment.Save(SendInvitationsMode.SendToAllAndSaveCopy);
      }
      else
      {
        // The appointment does not have attendees, so just save to calendar.
        appointment.Save(SendInvitationsMode.SendToNone);
      }
    }
    catch (ServiceResponseException ex)
    {
      Console.WriteLine(string.Format("Could not create appointment for {0}", emailAddress));
      Console.WriteLine(ex.Message);
    }
  }
}
```

<span data-ttu-id="ebfed-124">При сохранении встречи, код проверяется ли свойство [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) были добавлены участников собрания.</span><span class="sxs-lookup"><span data-stu-id="ebfed-124">When saving the appointment, the code checks to determine whether any attendees have been added to the [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) property.</span></span> <span data-ttu-id="ebfed-125">Если у них есть метод [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) вызывается с значение перечисления [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) , чтобы участники получают приглашения на собрания; в противном случае метод **Appointment.Save** вызывается с значение перечисления [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) , чтобы встречи сохраняется в календарь для олицетворения пользователя с помощью свойства [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) значение **false**.</span><span class="sxs-lookup"><span data-stu-id="ebfed-125">If they have, the [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) method is called with the [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the attendees receive meeting requests; otherwise, the **Appointment.Save** method is called with the [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the appointment is saved into the impersonated user's calendar with the [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) property set to **false**.</span></span>
  
### <a name="iappointmentfactory-interface"></a><span data-ttu-id="ebfed-126">Интерфейс IAppointmentFactory</span><span class="sxs-lookup"><span data-stu-id="ebfed-126">IAppointmentFactory interface</span></span>
<span data-ttu-id="ebfed-127"><a name="bk_IAppointmentFactory"> </a></span><span class="sxs-lookup"><span data-stu-id="ebfed-127"></span></span>

<span data-ttu-id="ebfed-128">Так как новый объект **встречи** требуется каждый раз, когда вы хотите сохранить встречу в календаре олицетворения пользователя, интерфейс **IAppointmentFactory** выделяет объект, используемый для заполнения каждого объекта **встречи** .</span><span class="sxs-lookup"><span data-stu-id="ebfed-128">Because you need a new **Appointment** object each time that you want to save an appointment on an impersonated user's calendar, the **IAppointmentFactory** interface abstracts the object used to populate each **Appointment** object.</span></span> <span data-ttu-id="ebfed-129">Эта версия — это простой интерфейс, который содержит только один метод, **GetAppointment**, который принимает объект **ExchangeService** как параметр и возвращает объект новой **встречи** , привязанные к объекту **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="ebfed-129">This version is a simple interface that contains only one method, **GetAppointment**, that takes an **ExchangeService** object as a parameter and returns a new **Appointment** object bound to that **ExchangeService** object.</span></span> 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

<span data-ttu-id="ebfed-130">В следующем примере класс **AppointmentFactory** показано, что реализацию интерфейса **IAppointmentFactory** , которое возвращает простой встречи, которая происходит через три дня.</span><span class="sxs-lookup"><span data-stu-id="ebfed-130">The following **AppointmentFactory** class example shows an implementation of the **IAppointmentFactory** interface that returns a simple appointment that occurs three days from now.</span></span> <span data-ttu-id="ebfed-131">При раскомментировании `appointment.RequiredAttendees.Add` строку, **GetAppointment** метод возвратит собрания и адрес электронной почты, указанных в том, что строка будет получать приглашения на собрание с олицетворенным пользователем, указано, что организатора.</span><span class="sxs-lookup"><span data-stu-id="ebfed-131">If you uncomment the  `appointment.RequiredAttendees.Add` line, the **GetAppointment** method will return a meeting and the email address specified in that line will receive a meeting request with the impersonated user listed as the organizer.</span></span> 
  
```cs
class AppointmentFactory : IAppointmentFactory
{
  public Appointment GetAppointment(ExchangeService service)
  {
    // First create the appointment to add.
    Appointment appointment = new Appointment(service);
    // Set the properties on the appointment.
    appointment.Subject = "Tennis lesson";
    appointment.Body = "Focus on backhand this week.";
    appointment.Start = DateTime.Now.AddDays(3);
    appointment.End = appointment.Start.AddHours(1);
    appointment.Location = "Tennis club";
    // appointment.RequiredAttendees.Add(new Attendee("sonyaf@contoso1000.onmicrosoft.com"));
    return appointment;
  }
}

```

## <a name="add-appointments-by-using-impersonation-with-ews"></a><span data-ttu-id="ebfed-132">Добавление встреч с использованием олицетворения с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ebfed-132">Add appointments by using impersonation with EWS</span></span>

<span data-ttu-id="ebfed-133">Веб-служб Exchange позволяет приложения для использования олицетворения для добавления элементов в календаре от имени владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="ebfed-133">EWS enables you application to use impersonation to add items to a calendar on behalf the calendar's owner.</span></span> <span data-ttu-id="ebfed-134">В этом примере показано, как использовать операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для добавления встречи в календаре олицетворенным учетной записи.</span><span class="sxs-lookup"><span data-stu-id="ebfed-134">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to add an appointment to the calendar of an impersonated account.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Tennis lesson</t:Subject>
          <t:Body BodyType="HTML">Focus on backhand this week.</t:Body>
          <t:ReminderDueBy>2013-09-19T14:37:10.732-07:00</t:ReminderDueBy>
          <t:Start>2013-09-21T19:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Tennis club</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ebfed-135">Обратите внимание на то, что кроме элемента **ExchangeImpersonation** в заголовке SOAP, чтобы указать учетную запись, мы олицетворения это же запрос XML, используемые для создания встречи без использования олицетворения.</span><span class="sxs-lookup"><span data-stu-id="ebfed-135">Note that other than the addition of the **ExchangeImpersonation** element in the SOAP header to specify the account that we are impersonating, this is the same XML request used to create an appointment without using impersonation.</span></span> 
  
<span data-ttu-id="ebfed-136">В следующем примере показано XML, возвращенные операцией **CreateItem** ответа.</span><span class="sxs-lookup"><span data-stu-id="ebfed-136">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ebfed-137">Атрибуты **ItemId** и **ChangeKey** сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="ebfed-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="ebfed-138">Опять же это же XML-ФАЙЛ, который возвращается при использовании операции **CreateItem** без использования олицетворения.</span><span class="sxs-lookup"><span data-stu-id="ebfed-138">Again, this is the same XML that is returned when you use the **CreateItem** operation without using impersonation.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ebfed-139">См. также</span><span class="sxs-lookup"><span data-stu-id="ebfed-139">See also</span></span>


- [<span data-ttu-id="ebfed-140">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="ebfed-140">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="ebfed-141">Роль ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="ebfed-141">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="ebfed-142">Настройка олицетворения</span><span class="sxs-lookup"><span data-stu-id="ebfed-142">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="ebfed-143">Идентификация учетной записи для олицетворения</span><span class="sxs-lookup"><span data-stu-id="ebfed-143">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="ebfed-144">Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="ebfed-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="ebfed-145">Операции CreateItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="ebfed-145">CreateItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)
    
- [<span data-ttu-id="ebfed-146">Свойство ExchangeService.ImpersonatedUserId</span><span class="sxs-lookup"><span data-stu-id="ebfed-146">ExchangeService.ImpersonatedUserId property</span></span>](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx.aspx)
    
