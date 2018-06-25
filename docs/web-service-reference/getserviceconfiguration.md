---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: Элемент GetServiceConfiguration определяет запрос GetServiceConfiguration.
ms.openlocfilehash: 7ff7124ff062f21a02fc69b86b7cc7367ba3fcb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833666"
---
# <a name="getserviceconfiguration"></a><span data-ttu-id="256cd-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="256cd-103">GetServiceConfiguration</span></span>

<span data-ttu-id="256cd-104">Элемент **GetServiceConfiguration** определяет запрос GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="256cd-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="256cd-105">**GetServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="256cd-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="256cd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="256cd-106">Attributes and elements</span></span>

<span data-ttu-id="256cd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="256cd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="256cd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="256cd-108">Attributes</span></span>

<span data-ttu-id="256cd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="256cd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="256cd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="256cd-110">Child elements</span></span>

|<span data-ttu-id="256cd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="256cd-111">**Element**</span></span>|<span data-ttu-id="256cd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="256cd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="256cd-113">ActingAs</span><span class="sxs-lookup"><span data-stu-id="256cd-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="256cd-114">Определяет, как отправляющего вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="256cd-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="256cd-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="256cd-115">This element is optional.</span></span> <span data-ttu-id="256cd-116">Если этот элемент не указан, прошедшего проверку пользователя считается отправителя.</span><span class="sxs-lookup"><span data-stu-id="256cd-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="256cd-117">Элемент **ActingAs** должны быть включены для разрешения на запрос подсказки отправителя.</span><span class="sxs-lookup"><span data-stu-id="256cd-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="256cd-118">Ошибка ErrorInvalidArgument можно получить в ответ, если элемент **ActingAs** отсутствует, не включает тип маршрутизации, не содержит адрес электронной почты, содержит недопустимый адрес электронной почты, не удается устранить для пользователя в домене Active Directory Службы (AD DS) или разрешается в нескольких пользователей в Доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="256cd-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="256cd-119">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="256cd-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="256cd-120">Содержит конфигурации запрошенные службы.</span><span class="sxs-lookup"><span data-stu-id="256cd-120">Contains the requested service configurations.</span></span> <span data-ttu-id="256cd-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="256cd-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="256cd-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="256cd-122">Parent elements</span></span>

<span data-ttu-id="256cd-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="256cd-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="256cd-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="256cd-124">Text value</span></span>

<span data-ttu-id="256cd-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="256cd-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="256cd-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="256cd-126">Remarks</span></span>

<span data-ttu-id="256cd-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="256cd-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="256cd-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="256cd-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="256cd-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="256cd-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="256cd-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="256cd-130">Schema Name</span></span>  <br/> |<span data-ttu-id="256cd-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="256cd-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="256cd-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="256cd-132">Validation File</span></span>  <br/> |<span data-ttu-id="256cd-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="256cd-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="256cd-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="256cd-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="256cd-135">False</span><span class="sxs-lookup"><span data-stu-id="256cd-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="256cd-136">См. также</span><span class="sxs-lookup"><span data-stu-id="256cd-136">See also</span></span>



- [<span data-ttu-id="256cd-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="256cd-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

