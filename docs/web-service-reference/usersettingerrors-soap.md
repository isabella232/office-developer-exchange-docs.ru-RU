---
title: UserSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a9b94bae-cab9-412d-a811-801e849ed6c5
description: Элемент UserSettingErrors представляет набор сведений о параметрах, которые не будут получены.
ms.openlocfilehash: 4477c30145d2cb187a4309d018512537af974ee8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840448"
---
# <a name="usersettingerrors-soap"></a><span data-ttu-id="aa314-103">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa314-103">UserSettingErrors (SOAP)</span></span>

<span data-ttu-id="aa314-104">Элемент **UserSettingErrors** представляет набор сведений о параметрах, которые не будут получены.</span><span class="sxs-lookup"><span data-stu-id="aa314-104">The **UserSettingErrors** element represents a collection of information about settings that could not be returned.</span></span> 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 <span data-ttu-id="aa314-105">**UserSettingErrors**</span><span class="sxs-lookup"><span data-stu-id="aa314-105">**UserSettingErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa314-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aa314-106">Attributes and elements</span></span>

<span data-ttu-id="aa314-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="aa314-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa314-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aa314-108">Attributes</span></span>

<span data-ttu-id="aa314-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa314-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa314-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aa314-110">Child elements</span></span>

|<span data-ttu-id="aa314-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa314-111">**Element**</span></span>|<span data-ttu-id="aa314-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa314-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa314-113">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa314-113">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="aa314-114">Представляет ошибку, который возвращается при получении параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa314-114">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa314-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aa314-115">Parent elements</span></span>

|<span data-ttu-id="aa314-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa314-116">**Element**</span></span>|<span data-ttu-id="aa314-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa314-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa314-118">Ответ пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa314-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="aa314-119">Представляет ответ на запрос GetUserSettings для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa314-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa314-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="aa314-120">Text value</span></span>

<span data-ttu-id="aa314-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa314-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa314-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aa314-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa314-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aa314-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="aa314-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aa314-124">Schema Name</span></span>  <br/> |<span data-ttu-id="aa314-125">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="aa314-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="aa314-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aa314-126">Validation File</span></span>  <br/> |<span data-ttu-id="aa314-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aa314-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa314-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aa314-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa314-129">True</span><span class="sxs-lookup"><span data-stu-id="aa314-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa314-130">См. также</span><span class="sxs-lookup"><span data-stu-id="aa314-130">See also</span></span>



[<span data-ttu-id="aa314-131">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="aa314-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

