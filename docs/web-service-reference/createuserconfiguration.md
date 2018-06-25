---
title: CreateUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfiguration
api_type:
- schema
ms.assetid: 43e12e8b-5629-4f5f-9cbd-a99084d8460f
description: Элемент CreateUserConfiguration представляет запрос на создание объекта конфигурации пользователя.
ms.openlocfilehash: dcf3acc356110b993bdb7f4f83245753835f299f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761923"
---
# <a name="createuserconfiguration"></a><span data-ttu-id="8272d-103">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="8272d-103">CreateUserConfiguration</span></span>

<span data-ttu-id="8272d-104">Элемент **CreateUserConfiguration** представляет запрос на создание объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="8272d-104">The **CreateUserConfiguration** element represents a request to create a user configuration object.</span></span> 
  
```xml
<CreateUserConfiguration>
   <UserConfiguration/>
</CreateUserConfiguration>
```

 <span data-ttu-id="8272d-105">**CreateUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="8272d-105">**CreateUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8272d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8272d-106">Attributes and elements</span></span>

<span data-ttu-id="8272d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8272d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8272d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8272d-108">Attributes</span></span>

<span data-ttu-id="8272d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8272d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8272d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8272d-110">Child elements</span></span>

|<span data-ttu-id="8272d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8272d-111">**Element**</span></span>|<span data-ttu-id="8272d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8272d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8272d-113">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="8272d-113">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="8272d-114">Представляет объект конфигурации одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8272d-114">Represents a single user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8272d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8272d-115">Parent elements</span></span>

<span data-ttu-id="8272d-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="8272d-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8272d-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8272d-117">Text value</span></span>

<span data-ttu-id="8272d-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="8272d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8272d-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="8272d-119">Remarks</span></span>

<span data-ttu-id="8272d-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8272d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8272d-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8272d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8272d-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8272d-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8272d-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8272d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8272d-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8272d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8272d-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8272d-125">Validation File</span></span>  <br/> |<span data-ttu-id="8272d-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8272d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8272d-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8272d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8272d-128">False</span><span class="sxs-lookup"><span data-stu-id="8272d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8272d-129">См. также</span><span class="sxs-lookup"><span data-stu-id="8272d-129">See also</span></span>



- [<span data-ttu-id="8272d-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8272d-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

