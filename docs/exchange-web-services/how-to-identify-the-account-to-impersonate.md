---
title: Идентификация учетной записи для олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Узнайте, как приложение службы использует EWS для идентификации пользователя, который будет олицетворять.
localization_priority: Priority
ms.openlocfilehash: 7159707abe96632aba2ed70dc0057417e087349f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527994"
---
# <a name="identify-the-account-to-impersonate"></a><span data-ttu-id="78389-103">Идентификация учетной записи для олицетворения</span><span class="sxs-lookup"><span data-stu-id="78389-103">Identify the account to impersonate</span></span>

<span data-ttu-id="78389-104">Узнайте, как приложение службы использует EWS для идентификации пользователя, который будет олицетворять.</span><span class="sxs-lookup"><span data-stu-id="78389-104">Learn how your service application uses EWS to identify the user to impersonate.</span></span>
  
<span data-ttu-id="78389-105">Приложение службы определяет учетную запись пользователя для олицетворения с помощью одного из следующих трех идентификаторов:</span><span class="sxs-lookup"><span data-stu-id="78389-105">Your service application identifies the user account to impersonate by using one of the following three identifiers:</span></span>
  
- <span data-ttu-id="78389-106">Основной SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="78389-106">The primary SMTP address.</span></span>
    
- <span data-ttu-id="78389-107">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="78389-107">The user principal name (UPN).</span></span>
    
- <span data-ttu-id="78389-108">Идентификатор безопасности (SID).</span><span class="sxs-lookup"><span data-stu-id="78389-108">The security identifier (SID).</span></span>
    
<span data-ttu-id="78389-109">Используемый идентификатор зависит от сведений, доступных в приложении.</span><span class="sxs-lookup"><span data-stu-id="78389-109">The identifier that you use depends, of course, on the information that your application has available.</span></span>
  
## <a name="identifying-the-user-account-to-impersonate"></a><span data-ttu-id="78389-110">Идентификация учетной записи пользователя для олицетворения</span><span class="sxs-lookup"><span data-stu-id="78389-110">Identifying the user account to impersonate</span></span>

<span data-ttu-id="78389-111">Приложение может использовать управляемый API EWS или запросы SOAP для идентификации учетной записи пользователя, которая является олицетворенной.</span><span class="sxs-lookup"><span data-stu-id="78389-111">Your application can use either the EWS Managed API or EWS SOAP requests to identify the user account that it is impersonating.</span></span> <span data-ttu-id="78389-112">Управляемый API EWS использует свойство [ExchangeService. имперсонатедусерид](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) для идентификации олицетворяемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="78389-112">The EWS Managed API uses the [ExchangeService.ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property to identify the impersonated user.</span></span> <span data-ttu-id="78389-113">В веб-службах EWS используется элемент [ексчанжеимперсонатион](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , как показано в следующем фрагменте XML.</span><span class="sxs-lookup"><span data-stu-id="78389-113">EWS uses the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) element, as shown in the following XML fragment.</span></span> 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

<span data-ttu-id="78389-114">В каждом из следующих разделов показано, как использовать один из идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="78389-114">Each of the following sections shows how to use one of the identifiers.</span></span> <span data-ttu-id="78389-115">Пример кода олицетворения в действии представлен в статье [Добавление встреч с помощью олицетворения Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="78389-115">For an example that shows the impersonation identifier in action, see [Add appointments by using Exchange impersonation](how-to-add-appointments-by-using-exchange-impersonation.md).</span></span>
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a><span data-ttu-id="78389-116">Использование SMTP-адреса электронной почты для идентификации учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="78389-116">Use the SMTP email address to identify the user account</span></span>

<span data-ttu-id="78389-117">SMTP-адрес электронной почты это основной адрес электронной почты, связанный с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="78389-117">The SMTP email address is the primary email address that is associated with a user account.</span></span>
  
<span data-ttu-id="78389-118">В приложении управляемого API EWS вы указываете адрес электронной почты SMTP вместе со значением перечисления [коннектингидтипе. SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="78389-118">In an EWS Managed API application, you specify the SMTP email address along with the [ConnectingIdType.SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

<span data-ttu-id="78389-119">В запросе SOAP в EWS элемент [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) содержит адрес электронной почты для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="78389-119">In an EWS SOAP request, the [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) element contains the email address for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a><span data-ttu-id="78389-120">Определение учетной записи пользователя с помощью имени участника-пользователя</span><span class="sxs-lookup"><span data-stu-id="78389-120">Use the UPN to identify the user account</span></span>

<span data-ttu-id="78389-121">Имя участника-пользователя содержит полное доменное имя (FQDN) для расположения учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="78389-121">The UPN contains the fully qualified domain name (FQDN) for the location of the user account.</span></span> <span data-ttu-id="78389-122">Он не обязательно является доменом почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="78389-122">This is not necessarily the user's mailbox domain.</span></span> <span data-ttu-id="78389-123">Для успешного выполнения поиска пользователя атрибут **userPrincipalName** должен быть правильно задан для учетной записи пользователя в доменных службах Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="78389-123">The **UserPrincipalName** attribute must be set correctly on the user account in Active Directory Domain Services (AD DS) for the user lookup to succeed.</span></span> 
  
<span data-ttu-id="78389-124">В приложении управляемого API EWS указывается имя участника-пользователя вместе со значением перечисления [коннектингидтипе. имя участника-](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="78389-124">In an EWS Managed API application, you specify the UPN along with the [ConnectingIdType.PrincipalName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipalName, "alias@billing.contoso.com");
```

<span data-ttu-id="78389-125">В запросе SOAP для EWS элемент [имя участника-(Коннектингсидтипе complexType) (EWS)](../web-service-reference/principalname.md) содержит имя участника-пользователя для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="78389-125">In an EWS SOAP request, the [PrincipalName element (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) element contains the UPN for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a><span data-ttu-id="78389-126">Определение учетной записи пользователя с помощью идентификатора безопасности (SID)</span><span class="sxs-lookup"><span data-stu-id="78389-126">Use the SID to identify the user account</span></span>

<span data-ttu-id="78389-127">SID это идентификатор учетной записи, которая должна быть олицетворена в форме языка определения дескрипторов безопасности (SDDL).</span><span class="sxs-lookup"><span data-stu-id="78389-127">The SID is the identifier of the account to be impersonated in security descriptor definition language (SDDL) form.</span></span>
  
<span data-ttu-id="78389-128">В приложении управляемого API EWS укажите идентификатор безопасности вместе со значением перечисления [коннектингидтипе. SID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="78389-128">In an EWS Managed API application, you specify the SID along with the [ConnectingIdType.SID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

<span data-ttu-id="78389-129">В запросе SOAP для EWS элемент [SID](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) содержит идентификатор SID учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="78389-129">In an EWS SOAP request, the [SID](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) element contains the SID for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a><span data-ttu-id="78389-130">См. также</span><span class="sxs-lookup"><span data-stu-id="78389-130">See also</span></span>


- [<span data-ttu-id="78389-131">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="78389-131">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="78389-132">Добавление встреч с помощью олицетворения Exchange</span><span class="sxs-lookup"><span data-stu-id="78389-132">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [<span data-ttu-id="78389-133">Класс ExchangeService</span><span class="sxs-lookup"><span data-stu-id="78389-133">ExchangeService class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [<span data-ttu-id="78389-134">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="78389-134">ExchangeImpersonation</span></span>](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

