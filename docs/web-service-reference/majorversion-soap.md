---
title: MajorVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0b2a83cf-e173-4073-9603-b2ea3b36ec1a
description: Элемент MajorVersion представляет основной номер версии для сервера.
ms.openlocfilehash: ca619d4c36e17ca9a811019f0a13b45353cab1e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834333"
---
# <a name="majorversion-soap"></a><span data-ttu-id="014ef-103">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="014ef-103">MajorVersion (SOAP)</span></span>

<span data-ttu-id="014ef-104">Элемент **MajorVersion** представляет основной номер версии для сервера.</span><span class="sxs-lookup"><span data-stu-id="014ef-104">The **MajorVersion** element represents the major version number for the server.</span></span> 
  
```XML
<MajorVersion/>
```

 <span data-ttu-id="014ef-105">**int**</span><span class="sxs-lookup"><span data-stu-id="014ef-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="014ef-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="014ef-106">Attributes and elements</span></span>

<span data-ttu-id="014ef-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="014ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="014ef-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="014ef-108">Attributes</span></span>

<span data-ttu-id="014ef-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="014ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="014ef-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="014ef-110">Child elements</span></span>

<span data-ttu-id="014ef-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="014ef-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="014ef-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="014ef-112">Parent elements</span></span>

|<span data-ttu-id="014ef-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="014ef-113">**Element**</span></span>|<span data-ttu-id="014ef-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="014ef-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="014ef-115">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="014ef-115">ServerVersionInfo (SOAP)</span></span>](serverversioninfo-soap.md) <br/> |<span data-ttu-id="014ef-116">Содержит версию сервера, на обработку запроса.</span><span class="sxs-lookup"><span data-stu-id="014ef-116">Contains the version of the server that processed the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="014ef-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="014ef-117">Text value</span></span>

<span data-ttu-id="014ef-118">Текстовое значение для элемента **MajorVersion** — целое число, представляющее основной номер версии сервера, на котором обработать запрос.</span><span class="sxs-lookup"><span data-stu-id="014ef-118">The text value for the **MajorVersion** element is an integer that represents the major version number of the server that processed the request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="014ef-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="014ef-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="014ef-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="014ef-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="014ef-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="014ef-121">Schema Name</span></span>  <br/> |<span data-ttu-id="014ef-122">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="014ef-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="014ef-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="014ef-123">Validation File</span></span>  <br/> |<span data-ttu-id="014ef-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="014ef-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="014ef-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="014ef-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="014ef-126">True</span><span class="sxs-lookup"><span data-stu-id="014ef-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="014ef-127">См. также</span><span class="sxs-lookup"><span data-stu-id="014ef-127">See also</span></span>



[<span data-ttu-id="014ef-128">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="014ef-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="014ef-129">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="014ef-129">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

