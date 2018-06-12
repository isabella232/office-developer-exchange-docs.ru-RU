---
title: Параметры пользователя (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ac3b827c-2e46-49ef-8c5a-f88084c0a12c
description: Параметры пользователя элемент представляет коллекцию параметров пользователя.
ms.openlocfilehash: 177c068077e755af51175c36824fb55a96494dca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840446"
---
# <a name="usersettings-soap"></a><span data-ttu-id="69337-103">Параметры пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="69337-103">UserSettings (SOAP)</span></span>

<span data-ttu-id="69337-104">**Параметры пользователя** элемент представляет коллекцию параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="69337-104">The **UserSettings** element represents a collection of user settings.</span></span> 
  
```XML
<UserSettings>
    <UserSetting/>
</UserSettings>
```

 <span data-ttu-id="69337-105">**Параметры пользователя**</span><span class="sxs-lookup"><span data-stu-id="69337-105">**UserSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69337-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="69337-106">Attributes and elements</span></span>

<span data-ttu-id="69337-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="69337-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69337-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="69337-108">Attributes</span></span>

<span data-ttu-id="69337-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="69337-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69337-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="69337-110">Child elements</span></span>

|<span data-ttu-id="69337-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69337-111">**Element**</span></span>|<span data-ttu-id="69337-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69337-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69337-113">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="69337-113">UserSetting (SOAP)</span></span>](usersetting-soap.md) <br/> |<span data-ttu-id="69337-114">Представляет параметр с одним пользователем.</span><span class="sxs-lookup"><span data-stu-id="69337-114">Represents a single user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69337-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="69337-115">Parent elements</span></span>

|<span data-ttu-id="69337-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69337-116">**Element**</span></span>|<span data-ttu-id="69337-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69337-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69337-118">Ответ пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="69337-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="69337-119">Представляет ответ на запрос GetUserSettings для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="69337-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="69337-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="69337-120">Text value</span></span>

<span data-ttu-id="69337-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="69337-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69337-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="69337-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69337-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="69337-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="69337-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="69337-124">Schema Name</span></span>  <br/> |<span data-ttu-id="69337-125">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="69337-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="69337-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="69337-126">Validation File</span></span>  <br/> |<span data-ttu-id="69337-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="69337-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69337-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="69337-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="69337-129">True</span><span class="sxs-lookup"><span data-stu-id="69337-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69337-130">См. также</span><span class="sxs-lookup"><span data-stu-id="69337-130">See also</span></span>



[<span data-ttu-id="69337-131">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="69337-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

