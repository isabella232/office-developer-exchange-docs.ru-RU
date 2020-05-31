---
title: Жетфедератионинформатионрекуест (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: df5bface-f070-49e0-8527-6129ed8e8095
description: Элемент Жетфедератионинформатионрекуест представляет параметры вызова операции операции Жетфедератионинформатион (SOAP).
ms.openlocfilehash: fee9340fdb0cb388bd18b95187f20b72e0e46a92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762791"
---
# <a name="getfederationinformationrequest-soap"></a><span data-ttu-id="0c97a-103">Жетфедератионинформатионрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c97a-103">GetFederationInformationRequest (SOAP)</span></span>

<span data-ttu-id="0c97a-104">Элемент **жетфедератионинформатионрекуест** представляет параметры вызова операции [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="0c97a-104">The **GetFederationInformationRequest** element represents the parameters of a call to the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md)operation.</span></span>
  
```XML
<GetFederationInformationRequest>
   <Domain/>
</GetFederationInformationRequest>
```

<span data-ttu-id="0c97a-105">**жетфедератионинформатионрекуест**</span><span class="sxs-lookup"><span data-stu-id="0c97a-105">**GetFederationInformationRequest**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0c97a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0c97a-106">Attributes and elements</span></span>

<span data-ttu-id="0c97a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0c97a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c97a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0c97a-108">Attributes</span></span>

<span data-ttu-id="0c97a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c97a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c97a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0c97a-110">Child elements</span></span>

|<span data-ttu-id="0c97a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c97a-111">**Element**</span></span>|<span data-ttu-id="0c97a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c97a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c97a-113">Домен (Жетфедератионинформатион) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c97a-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="0c97a-114">Определяет домен, который имеет доверие федерации.</span><span class="sxs-lookup"><span data-stu-id="0c97a-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c97a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0c97a-115">Parent elements</span></span>

<span data-ttu-id="0c97a-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c97a-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0c97a-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0c97a-117">Text value</span></span>

<span data-ttu-id="0c97a-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c97a-118">None.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="0c97a-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0c97a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c97a-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0c97a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0c97a-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0c97a-121">Schema Name</span></span>  <br/> |<span data-ttu-id="0c97a-122">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="0c97a-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0c97a-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0c97a-123">Validation File</span></span>  <br/> |<span data-ttu-id="0c97a-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0c97a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0c97a-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0c97a-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c97a-126">True</span><span class="sxs-lookup"><span data-stu-id="0c97a-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c97a-127">См. также</span><span class="sxs-lookup"><span data-stu-id="0c97a-127">See also</span></span>

- [<span data-ttu-id="0c97a-128">Операция Жетфедератионинформатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c97a-128">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

