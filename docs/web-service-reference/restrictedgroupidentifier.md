---
title: RestrictedGroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RestrictedGroupIdentifier
api_type:
- schema
ms.assetid: a3ea3c81-9f99-4836-8cb4-2384ea63f093
description: Элемент RestrictGroupIdentifier представляет идентификатор группы безопасности (SID) и атрибуты, используемые для группа с ограниченным доступом в рамках маркера пользователя.
ms.openlocfilehash: c6db8672b2afa855e83f2e9a2bf84c9ff33bdc7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835206"
---
# <a name="restrictedgroupidentifier"></a><span data-ttu-id="a2be8-103">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="a2be8-103">RestrictedGroupIdentifier</span></span>

<span data-ttu-id="a2be8-104">Элемент **RestrictGroupIdentifier** представляет идентификатор группы безопасности (SID) и атрибуты, используемые для группа с ограниченным доступом в рамках маркера пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2be8-104">The **RestrictGroupIdentifier** element represents the group security identifier (SID) and attributes for a restricted group within a user token.</span></span> 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 <span data-ttu-id="a2be8-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="a2be8-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2be8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2be8-106">Attributes and elements</span></span>

<span data-ttu-id="a2be8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a2be8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2be8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2be8-108">Attributes</span></span>

|<span data-ttu-id="a2be8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a2be8-109">**Attribute**</span></span>|<span data-ttu-id="a2be8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2be8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2be8-111">**Атрибуты**</span><span class="sxs-lookup"><span data-stu-id="a2be8-111">**Attributes**</span></span> <br/> |<span data-ttu-id="a2be8-112">Содержит атрибуты группы.</span><span class="sxs-lookup"><span data-stu-id="a2be8-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a2be8-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2be8-113">Child elements</span></span>

|<span data-ttu-id="a2be8-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2be8-114">**Element**</span></span>|<span data-ttu-id="a2be8-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2be8-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2be8-116">Класс SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="a2be8-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="a2be8-117">Представляет идентификатор безопасности формы языке SDDL определения дескриптора безопасности.</span><span class="sxs-lookup"><span data-stu-id="a2be8-117">Represents the security descriptor definition language (SDDL) form of a security identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2be8-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2be8-118">Parent elements</span></span>

|<span data-ttu-id="a2be8-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2be8-119">**Element**</span></span>|<span data-ttu-id="a2be8-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2be8-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2be8-121">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="a2be8-121">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="a2be8-122">Представляет коллекцию групп с ограниченным доступом в рамках маркера пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2be8-122">Represents a collection of restricted groups within a user token.</span></span> <span data-ttu-id="a2be8-123">Сериализация маркера не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2be8-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2be8-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="a2be8-124">Remarks</span></span>

<span data-ttu-id="a2be8-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a2be8-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2be8-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2be8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2be8-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2be8-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2be8-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2be8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a2be8-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a2be8-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2be8-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2be8-130">Validation File</span></span>  <br/> |<span data-ttu-id="a2be8-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a2be8-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2be8-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2be8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2be8-133">False</span><span class="sxs-lookup"><span data-stu-id="a2be8-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2be8-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a2be8-134">See also</span></span>



- [<span data-ttu-id="a2be8-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2be8-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

