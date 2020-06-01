---
title: Жетдомаинсеттингсреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43ebd17b-3a70-4878-9254-97a4c2c87b77
description: Элемент Жетдомаинсеттингсреспонсе представляет ответ на операцию Жетдомаинсеттингс (SOAP), которая возвращает параметры домена.
ms.openlocfilehash: 94cb202948e6a0d5a34f5547132c052d1d1b6a40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461879"
---
# <a name="getdomainsettingsresponse-soap"></a><span data-ttu-id="3aa91-103">Жетдомаинсеттингсреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3aa91-103">GetDomainSettingsResponse (SOAP)</span></span>

<span data-ttu-id="3aa91-104">Элемент **жетдомаинсеттингсреспонсе** представляет ответ на [операцию жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md), которая возвращает параметры домена.</span><span class="sxs-lookup"><span data-stu-id="3aa91-104">The **GetDomainSettingsResponse** element represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), which returns the domain settings.</span></span>
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 <span data-ttu-id="3aa91-105">**жетдомаинсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="3aa91-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3aa91-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3aa91-106">Attributes and elements</span></span>

<span data-ttu-id="3aa91-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3aa91-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3aa91-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3aa91-108">Attributes</span></span>

<span data-ttu-id="3aa91-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3aa91-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3aa91-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3aa91-110">Child elements</span></span>

|<span data-ttu-id="3aa91-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3aa91-111">**Element**</span></span>|<span data-ttu-id="3aa91-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3aa91-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3aa91-113">Домаинреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3aa91-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="3aa91-114">Содержит массив ответов для каждого параметра запрашиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="3aa91-114">Contains an array of responses for each requested domain's settings.</span></span>  <br/> |
|[<span data-ttu-id="3aa91-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3aa91-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="3aa91-116">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="3aa91-116">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3aa91-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3aa91-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="3aa91-118">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="3aa91-118">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3aa91-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3aa91-119">Parent elements</span></span>

<span data-ttu-id="3aa91-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3aa91-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3aa91-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3aa91-121">Text value</span></span>

<span data-ttu-id="3aa91-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3aa91-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3aa91-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3aa91-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3aa91-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3aa91-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3aa91-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3aa91-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3aa91-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="3aa91-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3aa91-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3aa91-127">Validation File</span></span>  <br/> |<span data-ttu-id="3aa91-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3aa91-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3aa91-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3aa91-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="3aa91-130">True</span><span class="sxs-lookup"><span data-stu-id="3aa91-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3aa91-131">См. также</span><span class="sxs-lookup"><span data-stu-id="3aa91-131">See also</span></span>



[<span data-ttu-id="3aa91-132">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3aa91-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

