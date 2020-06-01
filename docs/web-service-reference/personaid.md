---
title: персонаид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: eec3a468-afd5-4d72-a61e-cd1964fb686c
description: Элемент Персонаид указывает идентификатор пользователя для связанного пользователя.
ms.openlocfilehash: 3d7315097a14fb1eed5f378422cba80414601675
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457244"
---
# <a name="personaid"></a><span data-ttu-id="e7e98-103">персонаид</span><span class="sxs-lookup"><span data-stu-id="e7e98-103">PersonaId</span></span>

<span data-ttu-id="e7e98-104">Элемент **персонаид** указывает идентификатор пользователя для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e7e98-104">The **PersonaId** element specifies the persona identifier for the associated persona.</span></span> 
  
```XML
<PersonaId Id="" ChangeKey=""/>
```

 <span data-ttu-id="e7e98-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="e7e98-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7e98-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e7e98-106">Attributes and elements</span></span>

<span data-ttu-id="e7e98-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e7e98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7e98-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e7e98-108">Attributes</span></span>

|<span data-ttu-id="e7e98-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e7e98-109">**Attribute**</span></span>|<span data-ttu-id="e7e98-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7e98-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7e98-111">Id</span><span class="sxs-lookup"><span data-stu-id="e7e98-111">Id</span></span>  <br/> |<span data-ttu-id="e7e98-112">Текстовое значение атрибута **ID** — идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="e7e98-112">The text value of the **Id** attribute is the identifier of the persona.</span></span>  <br/> |
|<span data-ttu-id="e7e98-113">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="e7e98-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="e7e98-114">Текстовое значение атрибута **чанжекэй** — это ключ изменения пользователя.</span><span class="sxs-lookup"><span data-stu-id="e7e98-114">The text value of the **ChangeKey** attribute is the change key of the persona.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e7e98-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e7e98-115">Child elements</span></span>

<span data-ttu-id="e7e98-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e7e98-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7e98-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e7e98-117">Parent elements</span></span>

<span data-ttu-id="e7e98-118">[Долицо](getpersona.md)  |  [Персонаж](persona.md)</span><span class="sxs-lookup"><span data-stu-id="e7e98-118">[GetPersona](getpersona.md) | [Persona](persona.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7e98-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="e7e98-119">Remarks</span></span>

<span data-ttu-id="e7e98-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e7e98-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e7e98-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7e98-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7e98-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e7e98-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7e98-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e7e98-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e7e98-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e7e98-124">Schema name</span></span>  <br/> |<span data-ttu-id="e7e98-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e7e98-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e7e98-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e7e98-126">Validation file</span></span>  <br/> |<span data-ttu-id="e7e98-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e7e98-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7e98-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e7e98-128">Can be empty</span></span>  <br/> ||
   

