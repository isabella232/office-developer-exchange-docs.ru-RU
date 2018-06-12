---
title: SourceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fccdedc0-83ed-4bb7-a1d2-623e70d1a7bf
description: Элемент SourceId указывает идентификатор атрибутами контакт в пользователя.
ms.openlocfilehash: b08c28f93318a01e45a0d9cb812fef01905694ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835521"
---
# <a name="sourceid"></a><span data-ttu-id="1a43a-103">SourceId</span><span class="sxs-lookup"><span data-stu-id="1a43a-103">SourceId</span></span>

<span data-ttu-id="1a43a-104">Элемент **SourceId** указывает идентификатор атрибутами контакт в пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a43a-104">The **SourceId** element specifies the identifier of the attributed contact in a persona.</span></span> 
  
```XML
<SourceId Id="" ChangeKey=""/>
```

 <span data-ttu-id="1a43a-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="1a43a-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a43a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1a43a-106">Attributes and elements</span></span>

<span data-ttu-id="1a43a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1a43a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a43a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1a43a-108">Attributes</span></span>

|<span data-ttu-id="1a43a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="1a43a-109">**Attribute**</span></span>|<span data-ttu-id="1a43a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a43a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a43a-111">Id</span><span class="sxs-lookup"><span data-stu-id="1a43a-111">Id</span></span>  <br/> |<span data-ttu-id="1a43a-112">Текстовое значение атрибута **Id** является идентификатор контакта.</span><span class="sxs-lookup"><span data-stu-id="1a43a-112">The text value of the **Id** attribute is the identifier of the contact.</span></span>  <br/> |
|<span data-ttu-id="1a43a-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="1a43a-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="1a43a-114">Текстовое значение атрибута **ChangeKey** — это ключ изменения контакта.</span><span class="sxs-lookup"><span data-stu-id="1a43a-114">The text value of the **ChangeKey** attribute is the change key of the contact.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1a43a-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1a43a-115">Child elements</span></span>

<span data-ttu-id="1a43a-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="1a43a-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a43a-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1a43a-117">Parent elements</span></span>

[<span data-ttu-id="1a43a-118">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="1a43a-118">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
  
## <a name="remarks"></a><span data-ttu-id="1a43a-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="1a43a-119">Remarks</span></span>

<span data-ttu-id="1a43a-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1a43a-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1a43a-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a43a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a43a-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1a43a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a43a-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1a43a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a43a-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1a43a-124">Schema name</span></span>  <br/> |<span data-ttu-id="1a43a-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1a43a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a43a-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1a43a-126">Validation file</span></span>  <br/> |<span data-ttu-id="1a43a-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1a43a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a43a-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1a43a-128">Can be empty</span></span>  <br/> ||
   

