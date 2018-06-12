---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: Элемент GroupIdentifier представляет одиночный идентификатор безопасности и атрибут для группы объектов службы каталогов Active Directory, из которых учетная запись является участником.
ms.openlocfilehash: d73d72979762238ca09496cfbd6636b4ff44a969
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833767"
---
# <a name="groupidentifier"></a><span data-ttu-id="b984d-103">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="b984d-103">GroupIdentifier</span></span>

<span data-ttu-id="b984d-104">Элемент **GroupIdentifier** представляет одиночный идентификатор безопасности и атрибут для группы объектов службы каталогов Active Directory, из которых учетная запись является участником.</span><span class="sxs-lookup"><span data-stu-id="b984d-104">The **GroupIdentifier** element represents a single security identifier and attribute for an Active Directory directory service object group of which the account is a member.</span></span> 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 <span data-ttu-id="b984d-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="b984d-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b984d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b984d-106">Attributes and elements</span></span>

<span data-ttu-id="b984d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b984d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b984d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b984d-108">Attributes</span></span>

|<span data-ttu-id="b984d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b984d-109">**Attribute**</span></span>|<span data-ttu-id="b984d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b984d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b984d-111">**Атрибуты**</span><span class="sxs-lookup"><span data-stu-id="b984d-111">**Attributes**</span></span> <br/> |<span data-ttu-id="b984d-112">Содержит атрибуты группы.</span><span class="sxs-lookup"><span data-stu-id="b984d-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b984d-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b984d-113">Child elements</span></span>

|<span data-ttu-id="b984d-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b984d-114">**Element**</span></span>|<span data-ttu-id="b984d-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b984d-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b984d-116">Класс SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="b984d-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="b984d-117">Представляет идентификатор безопасности ([SID](sid.md)), который представляет группу формы языке SDDL определения дескриптора безопасности.</span><span class="sxs-lookup"><span data-stu-id="b984d-117">Represents the security descriptor definition language (SDDL) form of a security identifier ([SID](sid.md)) that represents the group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b984d-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b984d-118">Parent elements</span></span>

|<span data-ttu-id="b984d-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b984d-119">**Element**</span></span>|<span data-ttu-id="b984d-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b984d-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b984d-121">GroupSids</span><span class="sxs-lookup"><span data-stu-id="b984d-121">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="b984d-122">Представляет коллекцию идентификаторов безопасности объектов группы Active Directory, которые составляют маркер учетной записи для сериализация маркера.</span><span class="sxs-lookup"><span data-stu-id="b984d-122">Represents a collection of Active Directory group object security identifiers that make up an account token for token serialization.</span></span> <span data-ttu-id="b984d-123">Сериализация маркера не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b984d-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b984d-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="b984d-124">Remarks</span></span>

<span data-ttu-id="b984d-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b984d-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b984d-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b984d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b984d-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b984d-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b984d-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b984d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b984d-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b984d-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="b984d-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b984d-130">Validation File</span></span>  <br/> |<span data-ttu-id="b984d-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b984d-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b984d-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b984d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b984d-133">False</span><span class="sxs-lookup"><span data-stu-id="b984d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b984d-134">См. также</span><span class="sxs-lookup"><span data-stu-id="b984d-134">See also</span></span>



- [<span data-ttu-id="b984d-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b984d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

