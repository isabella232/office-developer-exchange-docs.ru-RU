---
title: коннектингсид
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
description: Элемент Коннектингсид представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.
ms.openlocfilehash: f4edf63f129fc769f4a2d710a505b40da4057fab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459281"
---
# <a name="connectingsid"></a><span data-ttu-id="106bf-103">коннектингсид</span><span class="sxs-lookup"><span data-stu-id="106bf-103">ConnectingSID</span></span>

<span data-ttu-id="106bf-104">Элемент **коннектингсид** представляет учетную запись для олицетворения при использовании заголовка SOAP ексчанжеимперсонатион.</span><span class="sxs-lookup"><span data-stu-id="106bf-104">The **ConnectingSID** element represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span> 
  
- [<span data-ttu-id="106bf-105">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="106bf-105">ExchangeImpersonation</span></span>](exchangeimpersonation.md) 
- [<span data-ttu-id="106bf-106">коннектингсид</span><span class="sxs-lookup"><span data-stu-id="106bf-106">ConnectingSID</span></span>](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

```xml
<ConnectingSID>
   <SmtpAddress/>
</ConnectingSID>
```

```xml
<ConnectingSID>
    <SID/> 
</ConnectingSID>
```

```xml
<ConnectingSID>
   <PrimarySmtpAddress/>
</ConnectingSID>
```

<span data-ttu-id="106bf-107">**коннектингсидтипе**</span><span class="sxs-lookup"><span data-stu-id="106bf-107">**ConnectingSIDType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="106bf-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="106bf-108">Attributes and elements</span></span>

<span data-ttu-id="106bf-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="106bf-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="106bf-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="106bf-110">Attributes</span></span>

<span data-ttu-id="106bf-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="106bf-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="106bf-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="106bf-112">Child elements</span></span>

|<span data-ttu-id="106bf-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="106bf-113">**Element**</span></span>|<span data-ttu-id="106bf-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="106bf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="106bf-115">Имя участника-</span><span class="sxs-lookup"><span data-stu-id="106bf-115">PrincipalName</span></span>](principalname.md) <br/> |<span data-ttu-id="106bf-116">Представляет имя участника-пользователя (UPN) учетной записи, используемой для олицетворения.</span><span class="sxs-lookup"><span data-stu-id="106bf-116">Represents the user principal name (UPN) of the account to use for impersonation.</span></span> <span data-ttu-id="106bf-117">Это должно быть имя участника-пользователя для домена, в котором находится учетная запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="106bf-117">This should be the UPN for the domain where the user account exists.</span></span>  <br/> |
|[<span data-ttu-id="106bf-118">SID</span><span class="sxs-lookup"><span data-stu-id="106bf-118">SID</span></span>](sid.md) <br/> |<span data-ttu-id="106bf-119">Представляет форму идентификатора безопасности (SID) для учетной записи, используемой для олицетворения, на языке определения дескрипторов безопасности (SDDL).</span><span class="sxs-lookup"><span data-stu-id="106bf-119">Represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation.</span></span>  <br/> |
|[<span data-ttu-id="106bf-120">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="106bf-120">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="106bf-121">Представляет основной SMTP-адрес учетной записи, используемой для олицетворения Exchange.</span><span class="sxs-lookup"><span data-stu-id="106bf-121">Represents the primary Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange impersonation.</span></span> <span data-ttu-id="106bf-122">Если указан основной SMTP-адрес, будет стоить дополнительное средство поиска службы каталогов Active Directory, чтобы получить идентификатор SID пользователя.</span><span class="sxs-lookup"><span data-stu-id="106bf-122">If the primary SMTP address is supplied, it will cost an extra Active Directory directory service lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="106bf-123">Рекомендуется использовать SID или UPN, если они доступны.</span><span class="sxs-lookup"><span data-stu-id="106bf-123">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
|[<span data-ttu-id="106bf-124">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="106bf-124">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="106bf-125">Представляет SMTP-адрес учетной записи, используемой для олицетворения Exchange.</span><span class="sxs-lookup"><span data-stu-id="106bf-125">Represents the Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange Impersonation.</span></span> <span data-ttu-id="106bf-126">Если указан SMTP-адрес, будет стоить дополнительный поиск в Active Directory, чтобы получить идентификатор SID пользователя.</span><span class="sxs-lookup"><span data-stu-id="106bf-126">If the SMTP address is supplied, it will cost an extra Active Directory lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="106bf-127">Рекомендуется использовать SID или UPN, если они доступны.</span><span class="sxs-lookup"><span data-stu-id="106bf-127">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="106bf-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="106bf-128">Parent elements</span></span>

|<span data-ttu-id="106bf-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="106bf-129">**Element**</span></span>|<span data-ttu-id="106bf-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="106bf-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="106bf-131">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="106bf-131">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="106bf-132">Используется в заголовке SOAP запроса.</span><span class="sxs-lookup"><span data-stu-id="106bf-132">Used in the SOAP header of a request.</span></span> <span data-ttu-id="106bf-133">Когда этот элемент присутствует, вызывающий абонент пытается олицетворить учетную запись, содержащуюся в элементе **ексчанжеимперсонатион** .</span><span class="sxs-lookup"><span data-stu-id="106bf-133">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span>  <br/> <span data-ttu-id="106bf-134">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="106bf-134">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="106bf-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="106bf-135">Remarks</span></span>

<span data-ttu-id="106bf-136">У вызывающей учетной записи должно быть право **MS – дов** на сервере клиентского доступа и в учетной записи **MS майимперсонате** в базе данных почтовых ящиков, которая содержит почтовый ящик для олицетворения или пользователя Active Directory или объекта Contact.</span><span class="sxs-lookup"><span data-stu-id="106bf-136">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory user or contact object.</span></span> 
  
<span data-ttu-id="106bf-137">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="106bf-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="106bf-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="106bf-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="106bf-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="106bf-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="106bf-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="106bf-140">Schema name</span></span>  <br/> |<span data-ttu-id="106bf-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="106bf-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="106bf-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="106bf-142">Validation file</span></span>  <br/> |<span data-ttu-id="106bf-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="106bf-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="106bf-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="106bf-144">Can be empty</span></span>  <br/> |<span data-ttu-id="106bf-145">False</span><span class="sxs-lookup"><span data-stu-id="106bf-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="106bf-146">См. также</span><span class="sxs-lookup"><span data-stu-id="106bf-146">See also</span></span>

- [<span data-ttu-id="106bf-147">Авторизация между серверами в EWS</span><span class="sxs-lookup"><span data-stu-id="106bf-147">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

