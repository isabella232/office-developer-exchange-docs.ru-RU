---
title: Документшаринглокатион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: Элемент Документшаринглокатион содержит сведения о расположении и метаданных расположения для общего доступа к документу.
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762198"
---
# <a name="documentsharinglocation-soap"></a><span data-ttu-id="086f8-103">Документшаринглокатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-103">DocumentSharingLocation (SOAP)</span></span>

<span data-ttu-id="086f8-104">Элемент **документшаринглокатион** содержит сведения о расположении и метаданных расположения для общего доступа к документу.</span><span class="sxs-lookup"><span data-stu-id="086f8-104">The **DocumentSharingLocation** element contains location and metadata information for a document sharing location.</span></span> 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 <span data-ttu-id="086f8-105">**документшаринглокатион**</span><span class="sxs-lookup"><span data-stu-id="086f8-105">**DocumentSharingLocation**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="086f8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="086f8-106">Attributes and elements</span></span>

<span data-ttu-id="086f8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="086f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="086f8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="086f8-108">Attributes</span></span>

<span data-ttu-id="086f8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="086f8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="086f8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="086f8-110">Child elements</span></span>

|<span data-ttu-id="086f8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="086f8-111">**Element**</span></span>|<span data-ttu-id="086f8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="086f8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="086f8-113">Сервицеурл (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-113">ServiceUrl (SOAP)</span></span>](serviceurl-soap.md) <br/> |<span data-ttu-id="086f8-114">Представляет URL-адрес веб-службы общего доступа к документам.</span><span class="sxs-lookup"><span data-stu-id="086f8-114">Represents the URL of the document sharing web service.</span></span>  <br/> |
|[<span data-ttu-id="086f8-115">Локатионурл (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-115">LocationUrl (SOAP)</span></span>](locationurl-soap.md) <br/> |<span data-ttu-id="086f8-116">Представляет URL-адрес расположения общего доступа к документу.</span><span class="sxs-lookup"><span data-stu-id="086f8-116">Represents the URL of the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="086f8-117">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-117">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="086f8-118">Представляет имя расположения для общего доступа к документу, которое будет использоваться в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="086f8-118">Represents the name of the document sharing location to use in the UI.</span></span>  <br/> |
|[<span data-ttu-id="086f8-119">Суппортедфиликстенсионс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-119">SupportedFileExtensions (SOAP)</span></span>](supportedfileextensions-soap.md) <br/> |<span data-ttu-id="086f8-120">Представляет расширения файлов, которые могут храниться в расположении общего доступа к документам.</span><span class="sxs-lookup"><span data-stu-id="086f8-120">Represents the file extensions that can be stored in the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="086f8-121">Екстерналакцессалловед (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-121">ExternalAccessAllowed (SOAP)</span></span>](externalaccessallowed-soap.md) <br/> |<span data-ttu-id="086f8-122">Указывает, доступно ли расположение для общего доступа к документу для внешнего подключения.</span><span class="sxs-lookup"><span data-stu-id="086f8-122">Indicates whether the document sharing location is available to outside connections.</span></span>  <br/> |
|[<span data-ttu-id="086f8-123">Анонимаусакцессалловед (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-123">AnonymousAccessAllowed (SOAP)</span></span>](anonymousaccessallowed-soap.md) <br/> |<span data-ttu-id="086f8-124">Указывает, требуется ли пользователю, прошедшему проверку подлинности, доступ к общему ресурсу.</span><span class="sxs-lookup"><span data-stu-id="086f8-124">Indicates whether access to the sharing location requires an authenticated user.</span></span>  <br/> |
|[<span data-ttu-id="086f8-125">Канмодифипермиссионс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-125">CanModifyPermissions (SOAP)</span></span>](canmodifypermissions-soap.md) <br/> |<span data-ttu-id="086f8-126">Указывает, может ли пользователь изменять разрешения доступа к расположению общего доступа к документам.</span><span class="sxs-lookup"><span data-stu-id="086f8-126">Indicates whether the user can modify access permissions to the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="086f8-127">По умолчанию (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-127">IsDefault (SOAP)</span></span>](isdefault-soap.md) <br/> |<span data-ttu-id="086f8-128">Указывает, является ли расположение общего доступа к документу общим расположением пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="086f8-128">Indicates whether the document sharing location is the user's default sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="086f8-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="086f8-129">Parent elements</span></span>

|<span data-ttu-id="086f8-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="086f8-130">**Element**</span></span>|<span data-ttu-id="086f8-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="086f8-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="086f8-132">Документшаринглокатионс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-132">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="086f8-133">Содержит список расположений и метаданных общего доступа к документам.</span><span class="sxs-lookup"><span data-stu-id="086f8-133">Contains a list of document sharing locations and metadata.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="086f8-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="086f8-134">Text value</span></span>

<span data-ttu-id="086f8-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="086f8-135">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="086f8-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="086f8-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="086f8-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="086f8-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="086f8-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="086f8-138">Schema Name</span></span>  <br/> |<span data-ttu-id="086f8-139">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="086f8-139">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="086f8-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="086f8-140">Validation File</span></span>  <br/> |<span data-ttu-id="086f8-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="086f8-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="086f8-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="086f8-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="086f8-143">True</span><span class="sxs-lookup"><span data-stu-id="086f8-143">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="086f8-144">См. также</span><span class="sxs-lookup"><span data-stu-id="086f8-144">See also</span></span>

- [<span data-ttu-id="086f8-145">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="086f8-145">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="086f8-146">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="086f8-146">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="086f8-147">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="086f8-147">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

