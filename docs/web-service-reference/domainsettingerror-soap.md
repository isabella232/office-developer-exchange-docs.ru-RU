---
title: Домаинсеттинжеррор (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: Элемент Домаинсеттинжеррор представляет ошибку, возникшую при получении параметра домена. Представляет ошибку в запросе Жетдомаинсеттингс.
ms.openlocfilehash: 08b0a47acea8d35ec78efd701168a251771effac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762216"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="74fde-104">Домаинсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74fde-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="74fde-105">Элемент **домаинсеттинжеррор** представляет ошибку, возникшую при получении параметра домена.</span><span class="sxs-lookup"><span data-stu-id="74fde-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="74fde-106">Представляет ошибку в запросе **жетдомаинсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="74fde-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="74fde-107">**домаинсеттинжеррор**</span><span class="sxs-lookup"><span data-stu-id="74fde-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74fde-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="74fde-108">Attributes and elements</span></span>

<span data-ttu-id="74fde-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="74fde-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74fde-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="74fde-110">Attributes</span></span>

<span data-ttu-id="74fde-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="74fde-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74fde-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="74fde-112">Child elements</span></span>

|<span data-ttu-id="74fde-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="74fde-113">**Element**</span></span>|<span data-ttu-id="74fde-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74fde-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74fde-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74fde-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="74fde-116">Определяет код ошибки, связанный с конкретным запросом.</span><span class="sxs-lookup"><span data-stu-id="74fde-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="74fde-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74fde-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="74fde-118">Содержит сообщение об ошибке, связанное с конкретным запросом.</span><span class="sxs-lookup"><span data-stu-id="74fde-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="74fde-119">Свойства settingname (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74fde-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="74fde-120">Представляет имя параметра.</span><span class="sxs-lookup"><span data-stu-id="74fde-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74fde-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="74fde-121">Parent elements</span></span>

|<span data-ttu-id="74fde-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="74fde-122">**Element**</span></span>|<span data-ttu-id="74fde-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74fde-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74fde-124">Домаинсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74fde-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="74fde-125">Содержит сведения об ошибках для параметров, которые не удалось вернуть.</span><span class="sxs-lookup"><span data-stu-id="74fde-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74fde-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="74fde-126">Text value</span></span>

<span data-ttu-id="74fde-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="74fde-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74fde-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="74fde-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74fde-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="74fde-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="74fde-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="74fde-130">Schema Name</span></span>  <br/> |<span data-ttu-id="74fde-131">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="74fde-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="74fde-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="74fde-132">Validation File</span></span>  <br/> |<span data-ttu-id="74fde-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="74fde-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74fde-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="74fde-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="74fde-135">True</span><span class="sxs-lookup"><span data-stu-id="74fde-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74fde-136">См. также</span><span class="sxs-lookup"><span data-stu-id="74fde-136">See also</span></span>

- [<span data-ttu-id="74fde-137">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="74fde-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

