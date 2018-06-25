---
title: GetUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfiguration
api_type:
- schema
ms.assetid: 4044c0a1-cd88-41ae-9cc4-a7cf2b279094
description: Элемент GetUserConfiguration представляют запрос на получение объекта конфигурации пользователя.
ms.openlocfilehash: 81f2ca4995de69d6547412ec699a2ceaddcce385
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833688"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="f1781-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1781-103">GetUserConfiguration</span></span>

<span data-ttu-id="f1781-104">Элемент **GetUserConfiguration** представляют запрос на получение объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1781-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="f1781-105">**GetUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="f1781-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1781-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f1781-106">Attributes and elements</span></span>

<span data-ttu-id="f1781-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f1781-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1781-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f1781-108">Attributes</span></span>

<span data-ttu-id="f1781-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1781-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1781-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f1781-110">Child elements</span></span>

|<span data-ttu-id="f1781-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1781-111">**Element**</span></span>|<span data-ttu-id="f1781-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1781-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1781-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="f1781-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="f1781-114">Представляет имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1781-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="f1781-115">Этот элемент должен присутствовать в запросе GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f1781-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="f1781-116">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="f1781-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="f1781-117">Указывает типы свойств конфигурации пользователя для возврата.</span><span class="sxs-lookup"><span data-stu-id="f1781-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="f1781-118">Этот элемент должен присутствовать в запросе GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f1781-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1781-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f1781-119">Parent elements</span></span>

<span data-ttu-id="f1781-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1781-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f1781-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f1781-121">Text value</span></span>

<span data-ttu-id="f1781-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1781-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1781-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="f1781-123">Remarks</span></span>

<span data-ttu-id="f1781-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1781-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1781-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f1781-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1781-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f1781-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f1781-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f1781-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f1781-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f1781-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f1781-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f1781-129">Validation File</span></span>  <br/> |<span data-ttu-id="f1781-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f1781-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1781-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f1781-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1781-132">False</span><span class="sxs-lookup"><span data-stu-id="f1781-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1781-133">См. также</span><span class="sxs-lookup"><span data-stu-id="f1781-133">See also</span></span>



- [<span data-ttu-id="f1781-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f1781-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

