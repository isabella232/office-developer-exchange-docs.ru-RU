---
title: Добавление встреч с помощью олицетворения Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Узнайте, как использовать олицетворение с помощью управляемого API EWS или EWS в Exchange для добавления встреч в календари пользователей.
localization_priority: Priority
ms.openlocfilehash: b1473d72113f8cc07d05364a4d87fedf23c7351d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455333"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a><span data-ttu-id="3d738-103">Добавление встреч с помощью олицетворения Exchange</span><span class="sxs-lookup"><span data-stu-id="3d738-103">Add appointments by using Exchange impersonation</span></span>

<span data-ttu-id="3d738-104">Узнайте, как использовать олицетворение с помощью управляемого API EWS или EWS в Exchange для добавления встреч в календари пользователей.</span><span class="sxs-lookup"><span data-stu-id="3d738-104">Learn how to use impersonation with the EWS Managed API or EWS in Exchange to add appointments to users' calendars.</span></span>
  
<span data-ttu-id="3d738-105">Вы можете создать приложение службы, которое вставляет встречи непосредственно в календарь Exchange, используя учетную запись службы с [включенной ролью](how-to-configure-impersonation.md) **ApplicationImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="3d738-105">You can create a service application that inserts appointments directly into an Exchange calendar by using a service account that has the **ApplicationImpersonation** [role enabled](how-to-configure-impersonation.md).</span></span> <span data-ttu-id="3d738-106">При использовании олицетворения приложение выступает в роли пользователя; Это так, как если бы пользователь добавил встречу в календарь с помощью клиента, например Outlook.</span><span class="sxs-lookup"><span data-stu-id="3d738-106">When you use impersonation, the application is acting as the user; it's as if the user added the appointment to the calendar by using a client such as Outlook.</span></span> 
  
<span data-ttu-id="3d738-107">При использовании олицетворения учитывайте следующие моменты.</span><span class="sxs-lookup"><span data-stu-id="3d738-107">When you are using impersonation, keep in mind the following:</span></span>
  
- <span data-ttu-id="3d738-108">Объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) должен быть связан с учетной записью службы.</span><span class="sxs-lookup"><span data-stu-id="3d738-108">Your [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) object must be bound to the service account.</span></span> <span data-ttu-id="3d738-109">Вы можете использовать один и тот же объект **ExchangeService** для олицетворения нескольких учетных записей, изменив свойство [имперсонатедусерид](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) для каждой учетной записи, для которой необходимо выполнить олицетворение.</span><span class="sxs-lookup"><span data-stu-id="3d738-109">You can use the same **ExchangeService** object to impersonate multiple accounts by changing the [ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property for each account that you want to impersonate.</span></span> 
    
- <span data-ttu-id="3d738-110">Любой элемент, сохраненный для олицетворенной учетной записи, можно использовать только один раз.</span><span class="sxs-lookup"><span data-stu-id="3d738-110">Any item that you save to an impersonated account can only be used once.</span></span> <span data-ttu-id="3d738-111">Если вы хотите сохранить одну и ту же встречу в нескольких учетных записях, например, необходимо создать объект [встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) для каждой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="3d738-111">If you want to save the same appointment in multiple accounts, for example, you have to create an [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) object for each account.</span></span> 
    
## <a name="prerequisites"></a><span data-ttu-id="3d738-112">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3d738-112">Prerequisites</span></span>

<span data-ttu-id="3d738-113">Для подключения к серверу Exchange приложение должно использовать учетную запись, прежде чем она сможет использовать олицетворение.</span><span class="sxs-lookup"><span data-stu-id="3d738-113">Your application needs an account to use to connect to the Exchange server before it can use impersonation.</span></span> <span data-ttu-id="3d738-114">Мы рекомендуем использовать учетную запись службы для приложения, которому была предоставлена роль олицетворения приложения для учетных записей, к которым будет осуществляться доступ.</span><span class="sxs-lookup"><span data-stu-id="3d738-114">We suggest that you use a service account for the application that has been granted the Application Impersonation role for the accounts that it will be accessing.</span></span> <span data-ttu-id="3d738-115">Дополнительные сведения см в разделе [Настройка олицетворения](how-to-configure-impersonation.md)</span><span class="sxs-lookup"><span data-stu-id="3d738-115">For more information, see [Configure impersonation](how-to-configure-impersonation.md)</span></span>
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a><span data-ttu-id="3d738-116">Добавление встреч с помощью олицетворения с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="3d738-116">Add appointments by using impersonation with the EWS Managed API</span></span>

<span data-ttu-id="3d738-117">В приведенном ниже примере показано, как добавить встречу или собрание в календарь одной или нескольких учетных записей Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d738-117">The following example adds an appointment or meeting to the calendar of one or more Exchange accounts.</span></span> <span data-ttu-id="3d738-118">Метод принимает три параметра.</span><span class="sxs-lookup"><span data-stu-id="3d738-118">The method takes three parameters.</span></span>
  
-  <span data-ttu-id="3d738-119">_Service_ — объект **ExchangeService** , привязанный к учетной записи приложения-службы на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d738-119">_service_ — An **ExchangeService** object bound to the service application's account on the Exchange server.</span></span> 
    
-  <span data-ttu-id="3d738-120">_EmailAddresses_ — объект [System. List](https://msdn.microsoft.com/library/6sh2ey19.aspx) , содержащий список строк адресов электронной почты SMTP.</span><span class="sxs-lookup"><span data-stu-id="3d738-120">_emailAddresses_ — A [System.List](https://msdn.microsoft.com/library/6sh2ey19.aspx) object containing a list of SMTP email address strings.</span></span> 
    
-  <span data-ttu-id="3d738-121">_фабрика_ — объект, который реализует интерфейс **иаппоинтментфактори** .</span><span class="sxs-lookup"><span data-stu-id="3d738-121">_factory_ — An object that implements the **IAppointmentFactory** interface.</span></span> <span data-ttu-id="3d738-122">Этот интерфейс содержит один **метод, метод ExchangeService, который** принимает объект **ExchangeService** в качестве параметра и возвращает объект **встречи** .</span><span class="sxs-lookup"><span data-stu-id="3d738-122">This interface has one method, **GetAppointment** that takes an **ExchangeService** object as a parameter and returns an **Appointment** object.</span></span> <span data-ttu-id="3d738-123">Интерфейс **иаппоинтментфактори** определяется [интерфейсом иаппоинтментфактори](#bk_IAppointmentFactory).</span><span class="sxs-lookup"><span data-stu-id="3d738-123">The **IAppointmentFactory** interface is defined [IAppointmentFactory interface](#bk_IAppointmentFactory).</span></span>
    
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

<span data-ttu-id="3d738-124">При сохранении встречи код проверяет, добавлены ли какие бы то ни было участников в свойство [RequiredAttendees](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3d738-124">When saving the appointment, the code checks to determine whether any attendees have been added to the [RequiredAttendees](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) property.</span></span> <span data-ttu-id="3d738-125">В противном случае метод [встреча. Save](https://msdn.microsoft.com/library/dd635394.aspx) вызывается со значением перечисления [сендтоалландсавекопи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) , чтобы участники получали приглашения на собрания; в противном случае метод **встреча. Save** вызывается со значением перечисления [сендтононе](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) , чтобы сохранить встречу в календаре олицетворенного пользователя с помощью свойства [Meeting.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) IsFalse, равное **false**.</span><span class="sxs-lookup"><span data-stu-id="3d738-125">If they have, the [Appointment.Save](https://msdn.microsoft.com/library/dd635394.aspx) method is called with the [SendToAllAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the attendees receive meeting requests; otherwise, the **Appointment.Save** method is called with the [SendToNone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the appointment is saved into the impersonated user's calendar with the [Appointment.IsMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) property set to **false**.</span></span>
  
### <a name="iappointmentfactory-interface"></a><span data-ttu-id="3d738-126">Интерфейс Иаппоинтментфактори</span><span class="sxs-lookup"><span data-stu-id="3d738-126">IAppointmentFactory interface</span></span>
<span data-ttu-id="3d738-127"><a name="bk_IAppointmentFactory"> </a></span><span class="sxs-lookup"><span data-stu-id="3d738-127"><a name="bk_IAppointmentFactory"> </a></span></span>

<span data-ttu-id="3d738-128">Так как для сохранения встречи в календаре олицетворенного пользователя необходим новый объект **встречи** , интерфейс **иаппоинтментфактори** абстрагирует объект, используемый для заполнения каждого объекта " **встреча** ".</span><span class="sxs-lookup"><span data-stu-id="3d738-128">Because you need a new **Appointment** object each time that you want to save an appointment on an impersonated user's calendar, the **IAppointmentFactory** interface abstracts the object used to populate each **Appointment** object.</span></span> <span data-ttu-id="3d738-129">Эта версия представляет собой простой интерфейс, который содержит только один метод, метод- **встречу**, который принимает объект **ExchangeService** в качестве параметра и возвращает новый объект **встречи** , привязанный к этому объекту **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="3d738-129">This version is a simple interface that contains only one method, **GetAppointment**, that takes an **ExchangeService** object as a parameter and returns a new **Appointment** object bound to that **ExchangeService** object.</span></span> 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

<span data-ttu-id="3d738-130">В приведенном ниже примере класса **аппоинтментфактори** показана реализация интерфейса **иаппоинтментфактори** , который возвращает простую встречу, которая находится в течение трех дней с этого момента.</span><span class="sxs-lookup"><span data-stu-id="3d738-130">The following **AppointmentFactory** class example shows an implementation of the **IAppointmentFactory** interface that returns a simple appointment that occurs three days from now.</span></span> <span data-ttu-id="3d738-131">Если вы раскомментируйте `appointment.RequiredAttendees.Add` строку, метод **GetAppointment** "метод" будет возвращать собрание, а адрес электронной почты, указанный в этой строке, будет получать приглашение на собрание с олицетворенным пользователем, указанным в качестве организатора.</span><span class="sxs-lookup"><span data-stu-id="3d738-131">If you uncomment the  `appointment.RequiredAttendees.Add` line, the **GetAppointment** method will return a meeting and the email address specified in that line will receive a meeting request with the impersonated user listed as the organizer.</span></span> 
  
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

## <a name="add-appointments-by-using-impersonation-with-ews"></a><span data-ttu-id="3d738-132">Добавление встреч с помощью службы EWS с помощью олицетворения</span><span class="sxs-lookup"><span data-stu-id="3d738-132">Add appointments by using impersonation with EWS</span></span>

<span data-ttu-id="3d738-133">С помощью служб EWS вы можете использовать олицетворение для добавления элементов в календарь от имени владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="3d738-133">EWS enables you application to use impersonation to add items to a calendar on behalf the calendar's owner.</span></span> <span data-ttu-id="3d738-134">В этом примере показано, как с помощью операции [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) добавить встречу в календарь олицетворенной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="3d738-134">This example shows how to use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to add an appointment to the calendar of an impersonated account.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="3d738-135">Обратите внимание, что кроме добавления элемента **ексчанжеимперсонатион** в заголовке SOAP для указания учетной записи, которую вы олицетворять, это тот же XML-запрос, который используется для создания встречи без использования олицетворения.</span><span class="sxs-lookup"><span data-stu-id="3d738-135">Note that other than the addition of the **ExchangeImpersonation** element in the SOAP header to specify the account that we are impersonating, this is the same XML request used to create an appointment without using impersonation.</span></span> 
  
<span data-ttu-id="3d738-136">В следующем примере показан XML-код отклика, возвращаемый операцией **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="3d738-136">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3d738-137">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3d738-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="3d738-138">Опять же, это тот же XML-код, который возвращается при использовании операции **CreateItem** без олицетворения.</span><span class="sxs-lookup"><span data-stu-id="3d738-138">Again, this is the same XML that is returned when you use the **CreateItem** operation without using impersonation.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3d738-139">См. также</span><span class="sxs-lookup"><span data-stu-id="3d738-139">See also</span></span>


- [<span data-ttu-id="3d738-140">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="3d738-140">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="3d738-141">Роль ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="3d738-141">ApplicationImpersonation role</span></span>](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="3d738-142">Настройка олицетворения</span><span class="sxs-lookup"><span data-stu-id="3d738-142">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="3d738-143">Идентификация учетной записи для олицетворения</span><span class="sxs-lookup"><span data-stu-id="3d738-143">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="3d738-144">Создание встреч и собраний с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="3d738-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="3d738-145">Операция CreateItem (элемент календаря)</span><span class="sxs-lookup"><span data-stu-id="3d738-145">CreateItem operation (calendar item)</span></span>](../web-service-reference/createitem-operation-calendar-item.md)
    
- [<span data-ttu-id="3d738-146">Свойство ExchangeService. Имперсонатедусерид</span><span class="sxs-lookup"><span data-stu-id="3d738-146">ExchangeService.ImpersonatedUserId property</span></span>](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid?view=exchange-ews-api)
    

