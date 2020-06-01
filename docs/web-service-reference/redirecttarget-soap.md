---
title: Редиректтаржет (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: Элемент Редиректтаржет (SOAP) содержит целевой объект URL-адреса перенаправления или адреса электронной почты.
ms.openlocfilehash: 092d575560379d43b12dd98a3efa155b59c31450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462201"
---
# <a name="redirecttarget-soap"></a><span data-ttu-id="fd387-103">Редиректтаржет (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd387-103">RedirectTarget (SOAP)</span></span>

<span data-ttu-id="fd387-104">Элемент [редиректтаржет (SOAP)](redirecttarget-soap.md) содержит целевой объект URL-адреса перенаправления или адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fd387-104">The [RedirectTarget (SOAP)](redirecttarget-soap.md) element contains the target of the redirection URL or e-mail address.</span></span> 
  
```XML
<RedirectTarget/>
```

 <span data-ttu-id="fd387-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="fd387-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd387-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fd387-106">Attributes and elements</span></span>

<span data-ttu-id="fd387-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fd387-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd387-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fd387-108">Attributes</span></span>

<span data-ttu-id="fd387-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fd387-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd387-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fd387-110">Child elements</span></span>

<span data-ttu-id="fd387-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fd387-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd387-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fd387-112">Parent elements</span></span>

|<span data-ttu-id="fd387-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fd387-113">**Element**</span></span>|<span data-ttu-id="fd387-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd387-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd387-115">Усерреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd387-115">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="fd387-116">Представляет ответ на запрос GetUserSettings для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd387-116">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
|[<span data-ttu-id="fd387-117">Домаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd387-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="fd387-118">Содержит запрошенные параметры для указанного домена.</span><span class="sxs-lookup"><span data-stu-id="fd387-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd387-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fd387-119">Text value</span></span>

<span data-ttu-id="fd387-120">Текстовое значение содержит целевой объект URL-адреса перенаправления или адрес электронной почты, который должен использоваться для последующего запроса GetUserSettings или Жетдомаинсеттингс.</span><span class="sxs-lookup"><span data-stu-id="fd387-120">The text value contains the target of the redirection URL or e-mail address that should be used for a subsequent GetUserSettings or GetDomainSettings request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd387-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fd387-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd387-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fd387-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fd387-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fd387-123">Schema Name</span></span>  <br/> |<span data-ttu-id="fd387-124">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="fd387-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fd387-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fd387-125">Validation File</span></span>  <br/> |<span data-ttu-id="fd387-126">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fd387-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd387-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fd387-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd387-128">True</span><span class="sxs-lookup"><span data-stu-id="fd387-128">True</span></span>  <br/> |
   

