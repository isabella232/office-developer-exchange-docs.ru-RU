---
title: SupportedFileExtensions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 6f73d18c-7bb1-4ab6-a23b-6d948e590b53
description: Элемент SupportedFileExtensions перечисляет расширения файлов, которые можно хранить в расположении для общего доступа к документам.
ms.openlocfilehash: d783b147a25ebbe3bff59c2142012b50bd80004e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44433989"
---
# <a name="supportedfileextensions-soap"></a><span data-ttu-id="88242-103">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88242-103">SupportedFileExtensions (SOAP)</span></span>

<span data-ttu-id="88242-104">Элемент **SupportedFileExtensions** перечисляет расширения файлов, которые можно хранить в расположении для общего доступа к документам.</span><span class="sxs-lookup"><span data-stu-id="88242-104">The **SupportedFileExtensions** element lists the file extensions that can be stored in a document sharing location.</span></span> 
  
```XML
<SupportedFileExtensions /> 
```

 <span data-ttu-id="88242-105">**ArrayOfFileExtension**</span><span class="sxs-lookup"><span data-stu-id="88242-105">**ArrayOfFileExtension**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88242-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="88242-106">Attributes and elements</span></span>

<span data-ttu-id="88242-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="88242-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88242-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="88242-108">Attributes</span></span>

<span data-ttu-id="88242-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="88242-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88242-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="88242-110">Child elements</span></span>

|<span data-ttu-id="88242-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88242-111">**Element**</span></span>|<span data-ttu-id="88242-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88242-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88242-113">FileExtension (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88242-113">FileExtension (SOAP)</span></span>](fileextension-soap.md) <br/> |<span data-ttu-id="88242-114">Представляет расширение файла.</span><span class="sxs-lookup"><span data-stu-id="88242-114">Represents a file extension.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88242-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="88242-115">Parent elements</span></span>

|<span data-ttu-id="88242-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88242-116">**Element**</span></span>|<span data-ttu-id="88242-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88242-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88242-118">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88242-118">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="88242-119">Представляет сведения о расположении и метаданных для общего доступа к документам.</span><span class="sxs-lookup"><span data-stu-id="88242-119">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="88242-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="88242-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88242-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="88242-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="88242-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="88242-122">Schema Name</span></span>  <br/> |<span data-ttu-id="88242-123">Схема автооружия</span><span class="sxs-lookup"><span data-stu-id="88242-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="88242-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="88242-124">Validation File</span></span>  <br/> |<span data-ttu-id="88242-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="88242-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88242-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="88242-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="88242-127">True</span><span class="sxs-lookup"><span data-stu-id="88242-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88242-128">См. также</span><span class="sxs-lookup"><span data-stu-id="88242-128">See also</span></span>



[<span data-ttu-id="88242-129">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88242-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="88242-130">Справочник по веб-службе автообнаружия для Exchange</span><span class="sxs-lookup"><span data-stu-id="88242-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="88242-131">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="88242-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

