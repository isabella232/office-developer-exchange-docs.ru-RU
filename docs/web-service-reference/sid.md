---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: Элемент SID представляет форме безопасности определения дескриптора языке SDDL идентификатор безопасности (SID) для учетной записи для использования при олицетворении или передача прав доступа.
ms.openlocfilehash: efcea42c12ec1d26ea31fdb8de337c37a2338a96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835492"
---
# <a name="sid"></a><span data-ttu-id="c44a8-103">SID</span><span class="sxs-lookup"><span data-stu-id="c44a8-103">SID</span></span>

<span data-ttu-id="c44a8-104">Элемент **SID** представляет форме безопасности определения дескриптора языке SDDL идентификатор безопасности (SID) для учетной записи для использования при олицетворении или передача прав доступа.</span><span class="sxs-lookup"><span data-stu-id="c44a8-104">The **SID** element represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation or delegate access.</span></span> 
  
```xml
<SID/>
```

 <span data-ttu-id="c44a8-105">**SIDType**</span><span class="sxs-lookup"><span data-stu-id="c44a8-105">**SIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c44a8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c44a8-106">Attributes and elements</span></span>

<span data-ttu-id="c44a8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c44a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c44a8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c44a8-108">Attributes</span></span>

<span data-ttu-id="c44a8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c44a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c44a8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c44a8-110">Child elements</span></span>

<span data-ttu-id="c44a8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c44a8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c44a8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c44a8-112">Parent elements</span></span>

|<span data-ttu-id="c44a8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c44a8-113">**Element**</span></span>|<span data-ttu-id="c44a8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c44a8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c44a8-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="c44a8-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="c44a8-116">Представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.</span><span class="sxs-lookup"><span data-stu-id="c44a8-116">Represents an account to impersonate when using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="c44a8-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="c44a8-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="c44a8-118">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="c44a8-118">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="c44a8-119">Идентифицирует пользователя делегатом или пользователь с правами доступа к папке.</span><span class="sxs-lookup"><span data-stu-id="c44a8-119">Identifies a delegate user or a user with folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c44a8-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c44a8-120">Text value</span></span>

<span data-ttu-id="c44a8-121">Текстовое значение является строковое представление ИД безопасности.</span><span class="sxs-lookup"><span data-stu-id="c44a8-121">The text value is a string representation of a SID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c44a8-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="c44a8-122">Remarks</span></span>

<span data-ttu-id="c44a8-123">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c44a8-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c44a8-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c44a8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c44a8-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c44a8-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c44a8-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c44a8-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c44a8-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c44a8-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="c44a8-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c44a8-128">Validation File</span></span>  <br/> |<span data-ttu-id="c44a8-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c44a8-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c44a8-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c44a8-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c44a8-131">False</span><span class="sxs-lookup"><span data-stu-id="c44a8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c44a8-132">См. также</span><span class="sxs-lookup"><span data-stu-id="c44a8-132">See also</span></span>



- [<span data-ttu-id="c44a8-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c44a8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

