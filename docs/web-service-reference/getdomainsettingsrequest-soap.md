---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: Элемент GetDomainSettingsRequest представляет запрос операции GetDomainSettings операции (SOAP).
ms.openlocfilehash: 4de525a9ba47a0d9afb0d6db9200fe32845f31d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762755"
---
# <a name="getdomainsettingsrequest-soap"></a><span data-ttu-id="d1198-103">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d1198-103">GetDomainSettingsRequest (SOAP)</span></span>

<span data-ttu-id="d1198-104">Элемент **GetDomainSettingsRequest** представляет запрос операции [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="d1198-104">The **GetDomainSettingsRequest** element represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 <span data-ttu-id="d1198-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="d1198-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1198-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d1198-106">Attributes and elements</span></span>

<span data-ttu-id="d1198-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d1198-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1198-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d1198-108">Attributes</span></span>

<span data-ttu-id="d1198-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d1198-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1198-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d1198-110">Child elements</span></span>

|<span data-ttu-id="d1198-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d1198-111">**Element**</span></span>|<span data-ttu-id="d1198-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d1198-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1198-113">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d1198-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="d1198-114">Представляет коллекцию идентификаторов домена.</span><span class="sxs-lookup"><span data-stu-id="d1198-114">Represents a collection of domain identifiers.</span></span>  <br/> |
|[<span data-ttu-id="d1198-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d1198-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="d1198-116">Содержит имена параметров конфигурации запрошенного домена.</span><span class="sxs-lookup"><span data-stu-id="d1198-116">Contains the names of the requested domain configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="d1198-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d1198-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="d1198-118">Указывает версию сервера, который будет использоваться поставщик.</span><span class="sxs-lookup"><span data-stu-id="d1198-118">Specifies the server version that the provider will use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d1198-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d1198-119">Parent elements</span></span>

<span data-ttu-id="d1198-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="d1198-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d1198-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d1198-121">Text value</span></span>

<span data-ttu-id="d1198-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="d1198-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1198-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d1198-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1198-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d1198-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d1198-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d1198-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d1198-126">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="d1198-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d1198-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d1198-127">Validation File</span></span>  <br/> |<span data-ttu-id="d1198-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d1198-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d1198-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d1198-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1198-130">True</span><span class="sxs-lookup"><span data-stu-id="d1198-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1198-131">См. также</span><span class="sxs-lookup"><span data-stu-id="d1198-131">See also</span></span>



[<span data-ttu-id="d1198-132">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d1198-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

