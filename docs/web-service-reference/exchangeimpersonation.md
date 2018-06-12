---
title: ExchangeImpersonation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: Элемент ExchangeImpersonation используется в заголовке SOAP запроса. Если этот элемент, вызывающего абонента пытается олицетворить учетную запись, которая содержится в элементе ExchangeImpersonation.
ms.openlocfilehash: aedeff22cda865ce1eec80dab9760d49fdc178f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762415"
---
# <a name="exchangeimpersonation"></a><span data-ttu-id="4549d-104">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="4549d-104">ExchangeImpersonation</span></span>

<span data-ttu-id="4549d-105">Элемент **ExchangeImpersonation** используется в заголовке SOAP запроса.</span><span class="sxs-lookup"><span data-stu-id="4549d-105">The **ExchangeImpersonation** element is used in the SOAP header of a request.</span></span> <span data-ttu-id="4549d-106">Если этот элемент, вызывающего абонента пытается олицетворить учетную запись, которая содержится в элементе **ExchangeImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="4549d-106">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span> 
  
[<span data-ttu-id="4549d-107">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="4549d-107">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 <span data-ttu-id="4549d-108">**ExchangeImpersonationType**</span><span class="sxs-lookup"><span data-stu-id="4549d-108">**ExchangeImpersonationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4549d-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4549d-109">Attributes and elements</span></span>

<span data-ttu-id="4549d-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4549d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4549d-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4549d-111">Attributes</span></span>

<span data-ttu-id="4549d-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="4549d-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4549d-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4549d-113">Child elements</span></span>

|<span data-ttu-id="4549d-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4549d-114">**Element**</span></span>|<span data-ttu-id="4549d-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4549d-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4549d-116">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="4549d-116">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="4549d-117">Представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.</span><span class="sxs-lookup"><span data-stu-id="4549d-117">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4549d-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4549d-118">Parent elements</span></span>

<span data-ttu-id="4549d-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="4549d-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4549d-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="4549d-120">Remarks</span></span>

<span data-ttu-id="4549d-121">Вызывающий учетная запись должна иметь **ms-exch-impersonation** непосредственно на сервер клиентского доступа и **ms-exch-MayImpersonate** непосредственно в либо базы данных почтовых ящиков, почтовых ящиков для олицетворения или пользователей/контакт Active Directory объект.</span><span class="sxs-lookup"><span data-stu-id="4549d-121">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory User/Contact object.</span></span> 
  
<span data-ttu-id="4549d-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4549d-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4549d-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4549d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4549d-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4549d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4549d-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4549d-125">Schema name</span></span>  <br/> |<span data-ttu-id="4549d-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4549d-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="4549d-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4549d-127">Validation file</span></span>  <br/> |<span data-ttu-id="4549d-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4549d-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4549d-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4549d-129">Can be empty</span></span>  <br/> |<span data-ttu-id="4549d-130">False</span><span class="sxs-lookup"><span data-stu-id="4549d-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4549d-131">См. также</span><span class="sxs-lookup"><span data-stu-id="4549d-131">See also</span></span>



[<span data-ttu-id="4549d-132">Сервер сервер авторизации в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="4549d-132">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

