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
ms.openlocfilehash: e9357a9e3be22e129c4910c01231f9dbd22a2dbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457874"
---
# <a name="getserviceconfiguration"></a><span data-ttu-id="3c1ae-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3c1ae-103">GetServiceConfiguration</span></span>

<span data-ttu-id="3c1ae-104">Элемент **GetServiceConfiguration** определяет запрос GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="3c1ae-105">**жетсервицеконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="3c1ae-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c1ae-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3c1ae-106">Attributes and elements</span></span>

<span data-ttu-id="3c1ae-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c1ae-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3c1ae-108">Attributes</span></span>

<span data-ttu-id="3c1ae-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c1ae-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3c1ae-110">Child elements</span></span>

|<span data-ttu-id="3c1ae-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c1ae-111">**Element**</span></span>|<span data-ttu-id="3c1ae-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c1ae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c1ae-113">актингас</span><span class="sxs-lookup"><span data-stu-id="3c1ae-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="3c1ae-114">Указывает, кому отправляется вызывающий абонент.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="3c1ae-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-115">This element is optional.</span></span> <span data-ttu-id="3c1ae-116">Если этот элемент отсутствует, предполагается, что пользователь, прошедший проверку подлинности, является отправителем.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="3c1ae-117">Элемент **актингас** должен быть включен для запроса подсказок отправителя.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="3c1ae-118">Если элемент **актингас** отсутствует, в отклике может быть возвращена ошибка ерроринвалидаргумент, не включающая в себя тип маршрутизации, не включает адрес электронной почты, содержит недопустимый адрес электронной почты, не разрешается пользователю в доменных службах Active Directory (AD DS) или разрешается нескольким пользователям в доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="3c1ae-119">рекуестедконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3c1ae-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="3c1ae-120">Содержит требуемые конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-120">Contains the requested service configurations.</span></span> <span data-ttu-id="3c1ae-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c1ae-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3c1ae-122">Parent elements</span></span>

<span data-ttu-id="3c1ae-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3c1ae-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3c1ae-124">Text value</span></span>

<span data-ttu-id="3c1ae-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3c1ae-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="3c1ae-126">Remarks</span></span>

<span data-ttu-id="3c1ae-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c1ae-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c1ae-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3c1ae-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c1ae-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3c1ae-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3c1ae-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3c1ae-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3c1ae-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3c1ae-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3c1ae-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3c1ae-132">Validation File</span></span>  <br/> |<span data-ttu-id="3c1ae-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3c1ae-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3c1ae-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3c1ae-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c1ae-135">False</span><span class="sxs-lookup"><span data-stu-id="3c1ae-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c1ae-136">См. также</span><span class="sxs-lookup"><span data-stu-id="3c1ae-136">See also</span></span>



- [<span data-ttu-id="3c1ae-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3c1ae-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

