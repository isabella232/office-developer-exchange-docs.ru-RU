---
title: актингас
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ActingAs
api_type:
- schema
ms.assetid: 3896afff-5c2c-4eaf-8621-c70e0371ea78
description: Элемент Актингас определяет, как вызывающий абонент отправляется.
ms.openlocfilehash: 9c007ed45f85dba265261dd79a6fd846dbd9d2f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762510"
---
# <a name="actingas"></a><span data-ttu-id="3bda2-103">актингас</span><span class="sxs-lookup"><span data-stu-id="3bda2-103">ActingAs</span></span>

<span data-ttu-id="3bda2-104">Элемент **актингас** определяет, как вызывающий абонент отправляется.</span><span class="sxs-lookup"><span data-stu-id="3bda2-104">The **ActingAs** element identifies who the caller is sending as.</span></span> 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 <span data-ttu-id="3bda2-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="3bda2-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3bda2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3bda2-106">Attributes and elements</span></span>

<span data-ttu-id="3bda2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3bda2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3bda2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3bda2-108">Attributes</span></span>

<span data-ttu-id="3bda2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3bda2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3bda2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3bda2-110">Child elements</span></span>

|<span data-ttu-id="3bda2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3bda2-111">**Element**</span></span>|<span data-ttu-id="3bda2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3bda2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bda2-113">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="3bda2-113">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="3bda2-114">Определяет SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3bda2-114">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="3bda2-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3bda2-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3bda2-116">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="3bda2-116">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="3bda2-117">Определяет маршрутизацию, используемую для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3bda2-117">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="3bda2-118">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="3bda2-118">The default is SMTP.</span></span> <span data-ttu-id="3bda2-119">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3bda2-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3bda2-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3bda2-120">Parent elements</span></span>

|<span data-ttu-id="3bda2-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3bda2-121">**Element**</span></span>|<span data-ttu-id="3bda2-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3bda2-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bda2-123">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bda2-123">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="3bda2-124">Определяет запрос **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="3bda2-124">Defines a **GetServiceConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3bda2-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="3bda2-125">Remarks</span></span>

<span data-ttu-id="3bda2-126">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3bda2-126">This element is optional.</span></span> <span data-ttu-id="3bda2-127">Если этот элемент отсутствует, предполагается, что пользователь, прошедший проверку подлинности, является отправителем.</span><span class="sxs-lookup"><span data-stu-id="3bda2-127">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="3bda2-128">Элемент **актингас** должен быть включен для запроса подсказок отправителя.</span><span class="sxs-lookup"><span data-stu-id="3bda2-128">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="3bda2-129">Если элемент **актингас** отсутствует, в отклике может быть возвращена ошибка **ерроринвалидаргумент** , не включающая в себя тип маршрутизации, не включает адрес электронной почты, содержит недопустимый адрес электронной почты, не разрешается пользователю в доменных службах Active Directory (AD DS) или разрешается нескольким пользователям в доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3bda2-129">An **ErrorInvalidArgument** error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span> 
  
<span data-ttu-id="3bda2-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3bda2-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3bda2-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3bda2-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3bda2-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3bda2-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3bda2-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3bda2-133">Schema Name</span></span>  <br/> |<span data-ttu-id="3bda2-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3bda2-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3bda2-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3bda2-135">Validation File</span></span>  <br/> |<span data-ttu-id="3bda2-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3bda2-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3bda2-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3bda2-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="3bda2-138">False</span><span class="sxs-lookup"><span data-stu-id="3bda2-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3bda2-139">См. также</span><span class="sxs-lookup"><span data-stu-id="3bda2-139">See also</span></span>

- [<span data-ttu-id="3bda2-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3bda2-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

