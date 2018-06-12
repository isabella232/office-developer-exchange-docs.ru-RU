---
title: ExternalAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 967df8c0-ee95-4202-b037-0c4b9fbbf5ee
description: Элемент ExternalAccessAllowed указывает, является ли документ расположение для обмена доступны за пределами подключений.
ms.openlocfilehash: 7d2a4027fe6de0c24191272d65605310af6a16bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762492"
---
# <a name="externalaccessallowed-soap"></a><span data-ttu-id="6b149-103">ExternalAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6b149-103">ExternalAccessAllowed (SOAP)</span></span>

<span data-ttu-id="6b149-104">Элемент **ExternalAccessAllowed** указывает, является ли документ расположение для обмена доступны за пределами подключений.</span><span class="sxs-lookup"><span data-stu-id="6b149-104">The **ExternalAccessAllowed** element indicates whether a document sharing location is available to outside connections.</span></span> 
  
```XML
<ExternalAccessAllowed /> 
```

 <span data-ttu-id="6b149-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6b149-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b149-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6b149-106">Attributes and elements</span></span>

<span data-ttu-id="6b149-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6b149-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b149-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6b149-108">Attributes</span></span>

<span data-ttu-id="6b149-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b149-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b149-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6b149-110">Child elements</span></span>

<span data-ttu-id="6b149-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b149-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b149-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6b149-112">Parent elements</span></span>

|<span data-ttu-id="6b149-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b149-113">**Element**</span></span>|<span data-ttu-id="6b149-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b149-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b149-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6b149-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="6b149-116">Представляет сведения о расположении и метаданных для документа расположение для обмена.</span><span class="sxs-lookup"><span data-stu-id="6b149-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b149-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6b149-117">Text value</span></span>

<span data-ttu-id="6b149-118">Логическое значение элемента **ExternalAccessAllowed** указывает ли доступны за пределами подключения к месту общего доступа.</span><span class="sxs-lookup"><span data-stu-id="6b149-118">The Boolean value of the **ExternalAccessAllowed** element indicates whether the sharing location is available to outside connections.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6b149-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6b149-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b149-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6b149-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6b149-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6b149-121">Schema Name</span></span>  <br/> |<span data-ttu-id="6b149-122">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="6b149-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6b149-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6b149-123">Validation File</span></span>  <br/> |<span data-ttu-id="6b149-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6b149-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b149-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6b149-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b149-126">True</span><span class="sxs-lookup"><span data-stu-id="6b149-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b149-127">См. также</span><span class="sxs-lookup"><span data-stu-id="6b149-127">See also</span></span>



[<span data-ttu-id="6b149-128">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6b149-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="6b149-129">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="6b149-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="6b149-130">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6b149-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

