---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: Элемент RedirectTarget (SOAP) содержит целевой перенаправления URL-адрес или адрес электронной почты.
ms.openlocfilehash: 3a8a0c39c6889730c9d17778c6a26f84fcbcd4a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835019"
---
# <a name="redirecttarget-soap"></a><span data-ttu-id="db73f-103">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="db73f-103">RedirectTarget (SOAP)</span></span>

<span data-ttu-id="db73f-104">Элемент [RedirectTarget (SOAP)](redirecttarget-soap.md) содержит целевой перенаправления URL-адрес или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="db73f-104">The [RedirectTarget (SOAP)](redirecttarget-soap.md) element contains the target of the redirection URL or e-mail address.</span></span> 
  
```XML
<RedirectTarget/>
```

 <span data-ttu-id="db73f-105">**string**</span><span class="sxs-lookup"><span data-stu-id="db73f-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db73f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="db73f-106">Attributes and elements</span></span>

<span data-ttu-id="db73f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="db73f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db73f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="db73f-108">Attributes</span></span>

<span data-ttu-id="db73f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="db73f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db73f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="db73f-110">Child elements</span></span>

<span data-ttu-id="db73f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="db73f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db73f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="db73f-112">Parent elements</span></span>

|<span data-ttu-id="db73f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db73f-113">**Element**</span></span>|<span data-ttu-id="db73f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db73f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db73f-115">Ответ пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="db73f-115">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="db73f-116">Представляет ответ на запрос GetUserSettings для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="db73f-116">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
|[<span data-ttu-id="db73f-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="db73f-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="db73f-118">Содержит запрошенные параметры для конкретного домена.</span><span class="sxs-lookup"><span data-stu-id="db73f-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db73f-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="db73f-119">Text value</span></span>

<span data-ttu-id="db73f-120">Текстовое значение содержит целевой перенаправления URL-адрес или адрес электронной почты, которая должна использоваться для последующих GetUserSettings или GetDomainSettings запроса.</span><span class="sxs-lookup"><span data-stu-id="db73f-120">The text value contains the target of the redirection URL or e-mail address that should be used for a subsequent GetUserSettings or GetDomainSettings request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db73f-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="db73f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db73f-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="db73f-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="db73f-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="db73f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="db73f-124">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="db73f-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="db73f-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="db73f-125">Validation File</span></span>  <br/> |<span data-ttu-id="db73f-126">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="db73f-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db73f-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="db73f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="db73f-128">True</span><span class="sxs-lookup"><span data-stu-id="db73f-128">True</span></span>  <br/> |
   

