---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: Элемент UserParameters содержит список расширений клиента включено.
ms.openlocfilehash: e0a72fe13255380ee56b32c863fb3bffb2e1ac5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840434"
---
# <a name="userparameters"></a><span data-ttu-id="6f525-103">UserParameters</span><span class="sxs-lookup"><span data-stu-id="6f525-103">UserParameters</span></span>

<span data-ttu-id="6f525-104">Элемент **UserParameters** содержит список расширений клиента включено.</span><span class="sxs-lookup"><span data-stu-id="6f525-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="6f525-105">**GetClientExtensionUserParametersType**</span><span class="sxs-lookup"><span data-stu-id="6f525-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f525-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6f525-106">Attributes and elements</span></span>

<span data-ttu-id="6f525-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6f525-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f525-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6f525-108">Attributes</span></span>

|<span data-ttu-id="6f525-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6f525-109">**Attribute**</span></span>|<span data-ttu-id="6f525-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f525-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6f525-111">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="6f525-111">UserId</span></span>  <br/> |<span data-ttu-id="6f525-112">Текстовое значение атрибута **идентификатор пользователя** — это идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f525-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="6f525-113">EnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6f525-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="6f525-114">Текстовое значение **EnabledOnly** показывает, содержит ли ответ только включенных расширений.</span><span class="sxs-lookup"><span data-stu-id="6f525-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6f525-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6f525-115">Child elements</span></span>

<span data-ttu-id="6f525-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="6f525-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f525-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6f525-117">Parent elements</span></span>

[<span data-ttu-id="6f525-118">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="6f525-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="6f525-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="6f525-119">Remarks</span></span>

<span data-ttu-id="6f525-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6f525-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6f525-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f525-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f525-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6f525-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f525-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6f525-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f525-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6f525-124">Schema name</span></span>  <br/> |<span data-ttu-id="6f525-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6f525-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f525-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6f525-126">Validation file</span></span>  <br/> |<span data-ttu-id="6f525-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f525-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f525-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6f525-128">Can be empty</span></span>  <br/> ||
   

