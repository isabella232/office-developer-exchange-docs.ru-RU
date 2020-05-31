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
# <a name="getserviceconfiguration"></a><span data-ttu-id="68738-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="68738-103">GetServiceConfiguration</span></span>

<span data-ttu-id="68738-104">Элемент **GetServiceConfiguration** определяет запрос GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68738-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="68738-105">**жетсервицеконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="68738-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68738-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="68738-106">Attributes and elements</span></span>

<span data-ttu-id="68738-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="68738-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68738-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="68738-108">Attributes</span></span>

<span data-ttu-id="68738-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="68738-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68738-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="68738-110">Child elements</span></span>

|<span data-ttu-id="68738-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68738-111">**Element**</span></span>|<span data-ttu-id="68738-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68738-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68738-113">актингас</span><span class="sxs-lookup"><span data-stu-id="68738-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="68738-114">Указывает, кому отправляется вызывающий абонент.</span><span class="sxs-lookup"><span data-stu-id="68738-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="68738-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="68738-115">This element is optional.</span></span> <span data-ttu-id="68738-116">Если этот элемент отсутствует, предполагается, что пользователь, прошедший проверку подлинности, является отправителем.</span><span class="sxs-lookup"><span data-stu-id="68738-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="68738-117">Элемент **актингас** должен быть включен для запроса подсказок отправителя.</span><span class="sxs-lookup"><span data-stu-id="68738-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="68738-118">Если элемент **актингас** отсутствует, в отклике может быть возвращена ошибка ерроринвалидаргумент, не включающая в себя тип маршрутизации, не включает адрес электронной почты, содержит недопустимый адрес электронной почты, не разрешается пользователю в доменных службах Active Directory (AD DS) или разрешается нескольким пользователям в доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="68738-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="68738-119">рекуестедконфигуратион</span><span class="sxs-lookup"><span data-stu-id="68738-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="68738-120">Содержит требуемые конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="68738-120">Contains the requested service configurations.</span></span> <span data-ttu-id="68738-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="68738-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68738-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="68738-122">Parent elements</span></span>

<span data-ttu-id="68738-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="68738-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="68738-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="68738-124">Text value</span></span>

<span data-ttu-id="68738-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="68738-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="68738-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="68738-126">Remarks</span></span>

<span data-ttu-id="68738-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="68738-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68738-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="68738-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68738-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="68738-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68738-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="68738-130">Schema Name</span></span>  <br/> |<span data-ttu-id="68738-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="68738-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68738-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="68738-132">Validation File</span></span>  <br/> |<span data-ttu-id="68738-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="68738-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68738-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="68738-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="68738-135">False</span><span class="sxs-lookup"><span data-stu-id="68738-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68738-136">См. также</span><span class="sxs-lookup"><span data-stu-id="68738-136">See also</span></span>



- [<span data-ttu-id="68738-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="68738-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

