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
ms.openlocfilehash: 189a614e7629033c8db2f60b8fd3679835a696ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530714"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="bc0d4-104">Домаинсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc0d4-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="bc0d4-105">Элемент **домаинсеттинжеррор** представляет ошибку, возникшую при получении параметра домена.</span><span class="sxs-lookup"><span data-stu-id="bc0d4-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="bc0d4-106">Представляет ошибку в запросе **жетдомаинсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="bc0d4-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="bc0d4-107">**домаинсеттинжеррор**</span><span class="sxs-lookup"><span data-stu-id="bc0d4-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc0d4-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc0d4-108">Attributes and elements</span></span>

<span data-ttu-id="bc0d4-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc0d4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc0d4-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc0d4-110">Attributes</span></span>

<span data-ttu-id="bc0d4-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc0d4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc0d4-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc0d4-112">Child elements</span></span>

|<span data-ttu-id="bc0d4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc0d4-113">**Element**</span></span>|<span data-ttu-id="bc0d4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc0d4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc0d4-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc0d4-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="bc0d4-116">Определяет код ошибки, связанный с конкретным запросом.</span><span class="sxs-lookup"><span data-stu-id="bc0d4-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="bc0d4-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc0d4-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="bc0d4-118">Содержит сообщение об ошибке, связанное с конкретным запросом.</span><span class="sxs-lookup"><span data-stu-id="bc0d4-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="bc0d4-119">Свойства settingname (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc0d4-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="bc0d4-120">Представляет имя параметра.</span><span class="sxs-lookup"><span data-stu-id="bc0d4-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc0d4-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc0d4-121">Parent elements</span></span>

|<span data-ttu-id="bc0d4-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc0d4-122">**Element**</span></span>|<span data-ttu-id="bc0d4-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc0d4-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc0d4-124">Домаинсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc0d4-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="bc0d4-125">Содержит сведения об ошибках для параметров, которые не удалось вернуть.</span><span class="sxs-lookup"><span data-stu-id="bc0d4-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc0d4-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bc0d4-126">Text value</span></span>

<span data-ttu-id="bc0d4-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc0d4-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc0d4-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc0d4-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc0d4-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc0d4-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bc0d4-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc0d4-130">Schema Name</span></span>  <br/> |<span data-ttu-id="bc0d4-131">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bc0d4-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bc0d4-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc0d4-132">Validation File</span></span>  <br/> |<span data-ttu-id="bc0d4-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bc0d4-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc0d4-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc0d4-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc0d4-135">True</span><span class="sxs-lookup"><span data-stu-id="bc0d4-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc0d4-136">См. также</span><span class="sxs-lookup"><span data-stu-id="bc0d4-136">See also</span></span>

- [<span data-ttu-id="bc0d4-137">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc0d4-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

