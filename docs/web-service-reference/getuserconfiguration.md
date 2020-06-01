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
ms.openlocfilehash: 46a2a5ebbabfc038692a5de83e0a960e05295061
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457713"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="2a235-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a235-103">GetUserConfiguration</span></span>

<span data-ttu-id="2a235-104">Элемент **GetUserConfiguration** представляет запрос на получение объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a235-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="2a235-105">**жетусерконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="2a235-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a235-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2a235-106">Attributes and elements</span></span>

<span data-ttu-id="2a235-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2a235-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a235-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2a235-108">Attributes</span></span>

<span data-ttu-id="2a235-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2a235-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a235-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2a235-110">Child elements</span></span>

|<span data-ttu-id="2a235-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2a235-111">**Element**</span></span>|<span data-ttu-id="2a235-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2a235-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a235-113">усерконфигуратионнаме</span><span class="sxs-lookup"><span data-stu-id="2a235-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="2a235-114">Представляет имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a235-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="2a235-115">Этот элемент должен присутствовать в запросе GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2a235-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="2a235-116">усерконфигуратионпропертиес</span><span class="sxs-lookup"><span data-stu-id="2a235-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="2a235-117">Задает возвращаемые типы свойств конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a235-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="2a235-118">Этот элемент должен присутствовать в запросе GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2a235-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a235-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2a235-119">Parent elements</span></span>

<span data-ttu-id="2a235-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2a235-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2a235-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2a235-121">Text value</span></span>

<span data-ttu-id="2a235-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="2a235-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2a235-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="2a235-123">Remarks</span></span>

<span data-ttu-id="2a235-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2a235-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a235-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2a235-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a235-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2a235-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2a235-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2a235-127">Schema Name</span></span>  <br/> |<span data-ttu-id="2a235-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="2a235-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2a235-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2a235-129">Validation File</span></span>  <br/> |<span data-ttu-id="2a235-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2a235-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2a235-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2a235-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="2a235-132">False</span><span class="sxs-lookup"><span data-stu-id="2a235-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a235-133">См. также</span><span class="sxs-lookup"><span data-stu-id="2a235-133">See also</span></span>



- [<span data-ttu-id="2a235-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2a235-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

