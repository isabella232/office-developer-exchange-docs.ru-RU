---
title: DeleteUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfiguration
api_type:
- schema
ms.assetid: 91b18b6a-d904-476c-996d-b041e859da1e
description: Элемент DeleteUserConfiguration представляет запрос на удаление объекта конфигурации пользователя.
ms.openlocfilehash: e357c32f95cddc866b77b6f1172ab260837b061b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762047"
---
# <a name="deleteuserconfiguration"></a><span data-ttu-id="dd1e5-103">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd1e5-103">DeleteUserConfiguration</span></span>

<span data-ttu-id="dd1e5-104">Элемент **DeleteUserConfiguration** представляет запрос на удаление объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd1e5-104">The **DeleteUserConfiguration** element represents a request to delete a user configuration object.</span></span> 
  
```xml
<DeleteUserConfiguration>
   <UserConfigurationName/>
</DeleteUserConfiguration>
```

 <span data-ttu-id="dd1e5-105">**DeleteUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="dd1e5-105">**DeleteUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd1e5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dd1e5-106">Attributes and elements</span></span>

<span data-ttu-id="dd1e5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dd1e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd1e5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dd1e5-108">Attributes</span></span>

<span data-ttu-id="dd1e5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd1e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd1e5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dd1e5-110">Child elements</span></span>

|<span data-ttu-id="dd1e5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd1e5-111">**Element**</span></span>|<span data-ttu-id="dd1e5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd1e5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd1e5-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="dd1e5-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="dd1e5-114">Представляет имя объекта конфигурации пользователя для удаления.</span><span class="sxs-lookup"><span data-stu-id="dd1e5-114">Represents the name of the user configuration object to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd1e5-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dd1e5-115">Parent elements</span></span>

<span data-ttu-id="dd1e5-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd1e5-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="dd1e5-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dd1e5-117">Text value</span></span>

<span data-ttu-id="dd1e5-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd1e5-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd1e5-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="dd1e5-119">Remarks</span></span>

<span data-ttu-id="dd1e5-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd1e5-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd1e5-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dd1e5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd1e5-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dd1e5-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd1e5-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dd1e5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="dd1e5-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dd1e5-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd1e5-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dd1e5-125">Validation File</span></span>  <br/> |<span data-ttu-id="dd1e5-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd1e5-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd1e5-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dd1e5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd1e5-128">False</span><span class="sxs-lookup"><span data-stu-id="dd1e5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd1e5-129">См. также</span><span class="sxs-lookup"><span data-stu-id="dd1e5-129">See also</span></span>

- [<span data-ttu-id="dd1e5-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dd1e5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
