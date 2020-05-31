---
title: Имя участника-
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrincipalName
api_type:
- schema
ms.assetid: 88c142d4-0bc7-43ea-a997-d7200664d900
description: Элемент имя участника-представляет имя участника-пользователя (UPN) учетной записи, которая будет использоваться для олицетворения Exchange.
ms.openlocfilehash: d8557ce0435a11a5602372517db1f576028a9c97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834882"
---
# <a name="principalname"></a><span data-ttu-id="52541-103">Имя участника-</span><span class="sxs-lookup"><span data-stu-id="52541-103">PrincipalName</span></span>

<span data-ttu-id="52541-104">Элемент **имя участника-** представляет имя участника-пользователя (UPN) учетной записи, которая будет использоваться для олицетворения Exchange.</span><span class="sxs-lookup"><span data-stu-id="52541-104">The **PrincipalName** element represents the user principal name (UPN) of the account to be used for Exchange impersonation.</span></span> 
  
```xml
<PrincipalName/>
```

 <span data-ttu-id="52541-105">**принЦипалнаметипе**</span><span class="sxs-lookup"><span data-stu-id="52541-105">**PrincipalNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52541-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="52541-106">Attributes and elements</span></span>

<span data-ttu-id="52541-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="52541-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52541-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="52541-108">Attributes</span></span>

<span data-ttu-id="52541-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="52541-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52541-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="52541-110">Child elements</span></span>

<span data-ttu-id="52541-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="52541-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="52541-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="52541-112">Parent elements</span></span>

|<span data-ttu-id="52541-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="52541-113">**Element**</span></span>|<span data-ttu-id="52541-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="52541-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52541-115">коннектингсид</span><span class="sxs-lookup"><span data-stu-id="52541-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="52541-116">Представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.</span><span class="sxs-lookup"><span data-stu-id="52541-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="52541-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="52541-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="52541-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="52541-118">Text value</span></span>

<span data-ttu-id="52541-119">Текстовое значение представляет имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="52541-119">The text value represents the UPN of a user.</span></span> <span data-ttu-id="52541-120">Это значение существует для объекта пользователя в службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52541-120">This value exists on the user object in the Active Directory directory service.</span></span> <span data-ttu-id="52541-121">Содержит имя входа пользователя и доменное имя, определяющее домен, в котором расположена учетная запись пользователя, в следующем формате: `someone@example.com`.</span><span class="sxs-lookup"><span data-stu-id="52541-121">This contains the user logon name and a domain name that identifies the domain in which the user account is located, in the following format:  `someone@example.com`.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="52541-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="52541-122">Remarks</span></span>

<span data-ttu-id="52541-123">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="52541-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52541-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="52541-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52541-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="52541-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52541-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="52541-126">Schema Name</span></span>  <br/> |<span data-ttu-id="52541-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="52541-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="52541-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="52541-128">Validation File</span></span>  <br/> |<span data-ttu-id="52541-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="52541-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="52541-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="52541-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="52541-131">False</span><span class="sxs-lookup"><span data-stu-id="52541-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52541-132">См. также</span><span class="sxs-lookup"><span data-stu-id="52541-132">See also</span></span>



- [<span data-ttu-id="52541-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="52541-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="52541-134">Авторизация между серверами в EWS</span><span class="sxs-lookup"><span data-stu-id="52541-134">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

