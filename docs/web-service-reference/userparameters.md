---
title: усерпараметерс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: Элемент Усерпараметерс содержит список включенных и отключенных расширений клиентов.
ms.openlocfilehash: 76bf858adfb6d2ef76a25c234117131752c60d7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526755"
---
# <a name="userparameters"></a><span data-ttu-id="76cc5-103">усерпараметерс</span><span class="sxs-lookup"><span data-stu-id="76cc5-103">UserParameters</span></span>

<span data-ttu-id="76cc5-104">Элемент **усерпараметерс** содержит список включенных и отключенных расширений клиентов.</span><span class="sxs-lookup"><span data-stu-id="76cc5-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="76cc5-105">**жетклиентекстенсионусерпараметерстипе**</span><span class="sxs-lookup"><span data-stu-id="76cc5-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76cc5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="76cc5-106">Attributes and elements</span></span>

<span data-ttu-id="76cc5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="76cc5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76cc5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="76cc5-108">Attributes</span></span>

|<span data-ttu-id="76cc5-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="76cc5-109">**Attribute**</span></span>|<span data-ttu-id="76cc5-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="76cc5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="76cc5-111">UserId</span><span class="sxs-lookup"><span data-stu-id="76cc5-111">UserId</span></span>  <br/> |<span data-ttu-id="76cc5-112">Текстовое значение атрибута **UserID** — идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="76cc5-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="76cc5-113">енабледонли</span><span class="sxs-lookup"><span data-stu-id="76cc5-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="76cc5-114">Текстовое значение **енабледонли** указывает, содержит ли отклик только включенные расширения.</span><span class="sxs-lookup"><span data-stu-id="76cc5-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="76cc5-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="76cc5-115">Child elements</span></span>

<span data-ttu-id="76cc5-116">[Усеренабледекстенсионс](userenabledextensions.md)  |  [Усердисабледекстенсионс](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="76cc5-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="76cc5-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="76cc5-117">Parent elements</span></span>

[<span data-ttu-id="76cc5-118">жетклиентекстенсион</span><span class="sxs-lookup"><span data-stu-id="76cc5-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="76cc5-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="76cc5-119">Remarks</span></span>

<span data-ttu-id="76cc5-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="76cc5-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="76cc5-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="76cc5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76cc5-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="76cc5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76cc5-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="76cc5-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76cc5-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="76cc5-124">Schema name</span></span>  <br/> |<span data-ttu-id="76cc5-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="76cc5-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="76cc5-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="76cc5-126">Validation file</span></span>  <br/> |<span data-ttu-id="76cc5-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="76cc5-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="76cc5-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="76cc5-128">Can be empty</span></span>  <br/> ||
   

