---
title: Идентификация учетной записи для олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Узнайте, как приложения-службы с помощью веб-служб Exchange для идентификации пользователя для олицетворения.
ms.openlocfilehash: 78df4b511a9947d4d815b2802a53ab178b14622b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761015"
---
# <a name="identify-the-account-to-impersonate"></a><span data-ttu-id="aad97-103">Идентификация учетной записи для олицетворения</span><span class="sxs-lookup"><span data-stu-id="aad97-103">Identify the account to impersonate</span></span>

<span data-ttu-id="aad97-104">Узнайте, как приложения-службы с помощью веб-служб Exchange для идентификации пользователя для олицетворения.</span><span class="sxs-lookup"><span data-stu-id="aad97-104">Learn how your service application uses EWS to identify the user to impersonate.</span></span>
  
<span data-ttu-id="aad97-105">Приложение службы указываются учетной записи пользователя для олицетворения, используя один из следующих трех идентификаторов:</span><span class="sxs-lookup"><span data-stu-id="aad97-105">Your service application identifies the user account to impersonate by using one of the following three identifiers:</span></span>
  
- <span data-ttu-id="aad97-106">Основной SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="aad97-106">The primary SMTP address.</span></span>
    
- <span data-ttu-id="aad97-107">Имя участника пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="aad97-107">The user principle name (UPN).</span></span>
    
- <span data-ttu-id="aad97-108">Идентификатор безопасности (SID).</span><span class="sxs-lookup"><span data-stu-id="aad97-108">The security identifier (SID).</span></span>
    
<span data-ttu-id="aad97-109">Идентификатор, который можно использовать зависит от того, конечно, сведения, в приложении есть недоступны.</span><span class="sxs-lookup"><span data-stu-id="aad97-109">The identifier that you use depends, of course, on the information that your application has available.</span></span>
  
## <a name="identifying-the-user-account-to-impersonate"></a><span data-ttu-id="aad97-110">Определение учетной записи пользователя для олицетворения</span><span class="sxs-lookup"><span data-stu-id="aad97-110">Identifying the user account to impersonate</span></span>

<span data-ttu-id="aad97-111">Приложение может использовать управляемый API EWS или веб-служб Exchange SOAP запросов для идентификации учетной записи пользователя, который олицетворении.</span><span class="sxs-lookup"><span data-stu-id="aad97-111">Your application can use either the EWS Managed API or EWS SOAP requests to identify the user account that it is impersonating.</span></span> <span data-ttu-id="aad97-112">Управляемый API EWS использует свойство [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) для идентификации олицетворения пользователя.</span><span class="sxs-lookup"><span data-stu-id="aad97-112">The EWS Managed API uses the [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property to identify the impersonated user.</span></span> <span data-ttu-id="aad97-113">Веб-служб Exchange используется элемент [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , как показано в следующем фрагменте XML.</span><span class="sxs-lookup"><span data-stu-id="aad97-113">EWS uses the [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) element, as shown in the following XML fragment.</span></span> 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

<span data-ttu-id="aad97-114">Каждой из следующих разделах показано, как использовать один из идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="aad97-114">Each of the following sections shows how to use one of the identifiers.</span></span> <span data-ttu-id="aad97-115">Пример идентификатор олицетворения в действии в разделе [Добавление встреч с помощью олицетворения Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="aad97-115">For an example that shows the impersonation identifier in action, see [Add appointments by using Exchange impersonation](how-to-add-appointments-by-using-exchange-impersonation.md).</span></span>
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a><span data-ttu-id="aad97-116">Используйте адрес электронной почты SMTP для учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="aad97-116">Use the SMTP email address to identify the user account</span></span>

<span data-ttu-id="aad97-117">Адрес электронной почты SMTP — это основной адрес электронной почты, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="aad97-117">The SMTP email address is the primary email address that is associated with a user account.</span></span>
  
<span data-ttu-id="aad97-118">В приложении, управляемый API веб-служб Exchange укажите адрес электронной почты SMTP, а также значение перечисления [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="aad97-118">In an EWS Managed API application, you specify the SMTP email address along with the [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

<span data-ttu-id="aad97-119">В запрос SOAP веб-служб Exchange элемент [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) содержит адрес электронной почты для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="aad97-119">In an EWS SOAP request, the [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) element contains the email address for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a><span data-ttu-id="aad97-120">Используйте имя участника-пользователя для учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="aad97-120">Use the UPN to identify the user account</span></span>

<span data-ttu-id="aad97-121">Имя участника-пользователя содержит полное доменное имя (FQDN) для расположения учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="aad97-121">The UPN contains the fully qualified domain name (FQDN) for the location of the user account.</span></span> <span data-ttu-id="aad97-122">Это не обязательно домен почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="aad97-122">This is not necessarily the user's mailbox domain.</span></span> <span data-ttu-id="aad97-123">Атрибут **UserPrincipleName** необходимо правильно задать для учетной записи пользователя в доменных службах Active Directory (AD DS) для успешного завершения поиска пользователя.</span><span class="sxs-lookup"><span data-stu-id="aad97-123">The **UserPrincipleName** attribute must be set correctly on the user account in Active Directory Domain Services (AD DS) for the user lookup to succeed.</span></span> 
  
<span data-ttu-id="aad97-124">В приложении, управляемый API веб-служб Exchange укажите имя участника-пользователя, а также значение перечисления [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="aad97-124">In an EWS Managed API application, you specify the UPN along with the [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

<span data-ttu-id="aad97-125">В запрос SOAP веб-служб Exchange [элемент PrincipalName (ConnectingSIDType complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) элемент содержит имя участника-пользователя для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="aad97-125">In an EWS SOAP request, the [PrincipalName element (ConnectingSIDType complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) element contains the UPN for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a><span data-ttu-id="aad97-126">Используйте идентификатор безопасности для учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="aad97-126">Use the SID to identify the user account</span></span>

<span data-ttu-id="aad97-127">Идентификатор безопасности — это идентификатор учетной записи для олицетворения в виде языке SDDL определения дескриптора безопасности.</span><span class="sxs-lookup"><span data-stu-id="aad97-127">The SID is the identifier of the account to be impersonated in security descriptor definition language (SDDL) form.</span></span>
  
<span data-ttu-id="aad97-128">В приложении, управляемый API веб-служб Exchange укажите идентификатор безопасности, а также значение перечисления [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="aad97-128">In an EWS Managed API application, you specify the SID along with the [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

<span data-ttu-id="aad97-129">В запрос SOAP веб-служб Exchange элемент [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) содержит идентификатор безопасности для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="aad97-129">In an EWS SOAP request, the [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) element contains the SID for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a><span data-ttu-id="aad97-130">См. также</span><span class="sxs-lookup"><span data-stu-id="aad97-130">See also</span></span>


- [<span data-ttu-id="aad97-131">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="aad97-131">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="aad97-132">Добавление встреч с использованием олицетворения Exchange</span><span class="sxs-lookup"><span data-stu-id="aad97-132">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [<span data-ttu-id="aad97-133">Класс ExchangeService</span><span class="sxs-lookup"><span data-stu-id="aad97-133">ExchangeService class</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [<span data-ttu-id="aad97-134">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="aad97-134">ExchangeImpersonation</span></span>](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

