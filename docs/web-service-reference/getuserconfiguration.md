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
description: Элемент GetUserConfiguration представляет запрос на получение объекта конфигурации пользователя.
ms.openlocfilehash: 81f2ca4995de69d6547412ec699a2ceaddcce385
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833688"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="5165e-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="5165e-103">GetUserConfiguration</span></span>

<span data-ttu-id="5165e-104">Элемент **GetUserConfiguration** представляет запрос на получение объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="5165e-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="5165e-105">**жетусерконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="5165e-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5165e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5165e-106">Attributes and elements</span></span>

<span data-ttu-id="5165e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5165e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5165e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5165e-108">Attributes</span></span>

<span data-ttu-id="5165e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5165e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5165e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5165e-110">Child elements</span></span>

|<span data-ttu-id="5165e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5165e-111">**Element**</span></span>|<span data-ttu-id="5165e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5165e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5165e-113">усерконфигуратионнаме</span><span class="sxs-lookup"><span data-stu-id="5165e-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="5165e-114">Представляет имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="5165e-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="5165e-115">Этот элемент должен присутствовать в запросе GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5165e-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="5165e-116">усерконфигуратионпропертиес</span><span class="sxs-lookup"><span data-stu-id="5165e-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="5165e-117">Задает возвращаемые типы свойств конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="5165e-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="5165e-118">Этот элемент должен присутствовать в запросе GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5165e-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5165e-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5165e-119">Parent elements</span></span>

<span data-ttu-id="5165e-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="5165e-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5165e-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5165e-121">Text value</span></span>

<span data-ttu-id="5165e-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="5165e-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5165e-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="5165e-123">Remarks</span></span>

<span data-ttu-id="5165e-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5165e-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5165e-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5165e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5165e-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5165e-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5165e-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5165e-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5165e-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5165e-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5165e-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5165e-129">Validation File</span></span>  <br/> |<span data-ttu-id="5165e-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5165e-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5165e-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5165e-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="5165e-132">False</span><span class="sxs-lookup"><span data-stu-id="5165e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5165e-133">См. также</span><span class="sxs-lookup"><span data-stu-id="5165e-133">See also</span></span>



- [<span data-ttu-id="5165e-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5165e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

