---
title: SupportedFileExtensions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 6f73d18c-7bb1-4ab6-a23b-6d948e590b53
description: Элемент SupportedFileExtensions список расширений файлов, которые могут храниться в документе общего ресурса.
ms.openlocfilehash: 0f1dbbce2b836fe05e4bc612c607302783d5e05d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840117"
---
# <a name="supportedfileextensions-soap"></a><span data-ttu-id="3a60f-103">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a60f-103">SupportedFileExtensions (SOAP)</span></span>

<span data-ttu-id="3a60f-104">Элемент **SupportedFileExtensions** список расширений файлов, которые могут храниться в документе общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="3a60f-104">The **SupportedFileExtensions** element lists the file extensions that can be stored in a document sharing location.</span></span> 
  
```XML
<SupportedFileExtensions /> 
```

 <span data-ttu-id="3a60f-105">**ArrayOfFileExtension**</span><span class="sxs-lookup"><span data-stu-id="3a60f-105">**ArrayOfFileExtension**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a60f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3a60f-106">Attributes and elements</span></span>

<span data-ttu-id="3a60f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3a60f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a60f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3a60f-108">Attributes</span></span>

<span data-ttu-id="3a60f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3a60f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a60f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3a60f-110">Child elements</span></span>

|<span data-ttu-id="3a60f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3a60f-111">**Element**</span></span>|<span data-ttu-id="3a60f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a60f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a60f-113">Добавляемое (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a60f-113">FileExtension (SOAP)</span></span>](fileextension-soap.md) <br/> |<span data-ttu-id="3a60f-114">Представляет расширение файла.</span><span class="sxs-lookup"><span data-stu-id="3a60f-114">Represents a file extension.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a60f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3a60f-115">Parent elements</span></span>

|<span data-ttu-id="3a60f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3a60f-116">**Element**</span></span>|<span data-ttu-id="3a60f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a60f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a60f-118">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a60f-118">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="3a60f-119">Представляет сведения о расположении и метаданных для документа расположение для обмена.</span><span class="sxs-lookup"><span data-stu-id="3a60f-119">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="3a60f-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3a60f-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a60f-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3a60f-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3a60f-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3a60f-122">Schema Name</span></span>  <br/> |<span data-ttu-id="3a60f-123">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="3a60f-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3a60f-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3a60f-124">Validation File</span></span>  <br/> |<span data-ttu-id="3a60f-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a60f-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a60f-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3a60f-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a60f-127">True</span><span class="sxs-lookup"><span data-stu-id="3a60f-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a60f-128">См. также</span><span class="sxs-lookup"><span data-stu-id="3a60f-128">See also</span></span>



[<span data-ttu-id="3a60f-129">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a60f-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="3a60f-130">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="3a60f-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="3a60f-131">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="3a60f-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

