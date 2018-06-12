---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: Элемент ConnectingSID представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.
ms.openlocfilehash: 6e0bb90e197ce22bcd982a6d51954a88f3a2cf03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761720"
---
# <a name="connectingsid"></a><span data-ttu-id="35de7-103">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="35de7-103">ConnectingSID</span></span>

<span data-ttu-id="35de7-104">Элемент **ConnectingSID** представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.</span><span class="sxs-lookup"><span data-stu-id="35de7-104">The **ConnectingSID** element represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span> 
  
[<span data-ttu-id="35de7-105">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="35de7-105">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
[<span data-ttu-id="35de7-106">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="35de7-106">ConnectingSID</span></span>](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

 <span data-ttu-id="35de7-107">**ConnectingSIDType**</span><span class="sxs-lookup"><span data-stu-id="35de7-107">**ConnectingSIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35de7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="35de7-108">Attributes and elements</span></span>

<span data-ttu-id="35de7-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="35de7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35de7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="35de7-110">Attributes</span></span>

<span data-ttu-id="35de7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="35de7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35de7-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="35de7-112">Child elements</span></span>

|<span data-ttu-id="35de7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="35de7-113">**Element**</span></span>|<span data-ttu-id="35de7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="35de7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35de7-115">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="35de7-115">PrincipalName</span></span>](principalname.md) <br/> |<span data-ttu-id="35de7-116">Представляет имя участника-пользователя (UPN) учетную запись, используемую для олицетворения.</span><span class="sxs-lookup"><span data-stu-id="35de7-116">Represents the user principal name (UPN) of the account to use for impersonation.</span></span> <span data-ttu-id="35de7-117">Это должно быть имя участника-пользователя для домена, где существует учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="35de7-117">This should be the UPN for the domain where the user account exists.</span></span>  <br/> |
|[<span data-ttu-id="35de7-118">ИД БЕЗОПАСНОСТИ</span><span class="sxs-lookup"><span data-stu-id="35de7-118">SID</span></span>](sid.md) <br/> |<span data-ttu-id="35de7-119">Представляет идентификатор безопасности (SID) формы языке SDDL определения дескриптор безопасности для учетной записи для использования при олицетворении.</span><span class="sxs-lookup"><span data-stu-id="35de7-119">Represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation.</span></span>  <br/> |
|[<span data-ttu-id="35de7-120">Параметр PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="35de7-120">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="35de7-121">Представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетную запись, используемую для олицетворения Exchange.</span><span class="sxs-lookup"><span data-stu-id="35de7-121">Represents the primary Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange impersonation.</span></span> <span data-ttu-id="35de7-122">Если предоставлен основной SMTP-адрес, это потребует дополнительного поиска службы каталогов Active Directory для получения ИД безопасности пользователя.</span><span class="sxs-lookup"><span data-stu-id="35de7-122">If the primary SMTP address is supplied, it will cost an extra Active Directory directory service lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="35de7-123">Мы рекомендуем использовать ИД безопасности или имя участника-пользователя, если они доступны.</span><span class="sxs-lookup"><span data-stu-id="35de7-123">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
|[<span data-ttu-id="35de7-124">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="35de7-124">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="35de7-125">Представляет адрес Simple Mail Transfer Protocol (SMTP) учетную запись, используемую для олицетворения Exchange.</span><span class="sxs-lookup"><span data-stu-id="35de7-125">Represents the Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange Impersonation.</span></span> <span data-ttu-id="35de7-126">Если предоставлен SMTP-адрес, это потребует дополнительного поиска Active Directory для получения ИД безопасности пользователя.</span><span class="sxs-lookup"><span data-stu-id="35de7-126">If the SMTP address is supplied, it will cost an extra Active Directory lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="35de7-127">Мы рекомендуем использовать ИД безопасности или имя участника-пользователя, если они доступны.</span><span class="sxs-lookup"><span data-stu-id="35de7-127">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="35de7-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="35de7-128">Parent elements</span></span>

|<span data-ttu-id="35de7-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="35de7-129">**Element**</span></span>|<span data-ttu-id="35de7-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="35de7-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35de7-131">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="35de7-131">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="35de7-132">Используется в заголовке SOAP запроса.</span><span class="sxs-lookup"><span data-stu-id="35de7-132">Used in the SOAP header of a request.</span></span> <span data-ttu-id="35de7-133">Если этот элемент, вызывающего абонента пытается олицетворить учетную запись, которая содержится в элементе **ExchangeImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="35de7-133">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span>  <br/> <span data-ttu-id="35de7-134">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="35de7-134">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="35de7-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="35de7-135">Remarks</span></span>

<span data-ttu-id="35de7-136">Вызывающий учетная запись должна иметь **ms-exch-impersonation** непосредственно на сервер клиентского доступа и **ms-exch-MayImpersonate** непосредственно в либо базы данных почтовых ящиков, почтовых ящиков для олицетворения или Active Directory пользователя или контакта объект.</span><span class="sxs-lookup"><span data-stu-id="35de7-136">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory user or contact object.</span></span> 
  
<span data-ttu-id="35de7-137">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="35de7-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35de7-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="35de7-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35de7-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="35de7-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="35de7-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="35de7-140">Schema name</span></span>  <br/> |<span data-ttu-id="35de7-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="35de7-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="35de7-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="35de7-142">Validation file</span></span>  <br/> |<span data-ttu-id="35de7-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="35de7-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="35de7-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="35de7-144">Can be empty</span></span>  <br/> |<span data-ttu-id="35de7-145">False</span><span class="sxs-lookup"><span data-stu-id="35de7-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35de7-146">См. также</span><span class="sxs-lookup"><span data-stu-id="35de7-146">See also</span></span>



[<span data-ttu-id="35de7-147">Сервер сервер авторизации в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="35de7-147">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

