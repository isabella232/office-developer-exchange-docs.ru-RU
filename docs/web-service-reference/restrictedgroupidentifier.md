---
title: рестриктедграупидентифиер
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
description: Элемент Рестриктграупидентифиер представляет идентификатор безопасности группы (SID) и атрибуты для группы с ограниченным доступом в маркере пользователя.
ms.openlocfilehash: c95af4e09324e96f4551a05490dc200aec0cbd46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465368"
---
# <a name="restrictedgroupidentifier"></a><span data-ttu-id="4eb7f-103">рестриктедграупидентифиер</span><span class="sxs-lookup"><span data-stu-id="4eb7f-103">RestrictedGroupIdentifier</span></span>

<span data-ttu-id="4eb7f-104">Элемент **рестриктграупидентифиер** представляет идентификатор безопасности группы (SID) и атрибуты для группы с ограниченным доступом в маркере пользователя.</span><span class="sxs-lookup"><span data-stu-id="4eb7f-104">The **RestrictGroupIdentifier** element represents the group security identifier (SID) and attributes for a restricted group within a user token.</span></span> 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 <span data-ttu-id="4eb7f-105">**сидандаттрибутестипе**</span><span class="sxs-lookup"><span data-stu-id="4eb7f-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4eb7f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4eb7f-106">Attributes and elements</span></span>

<span data-ttu-id="4eb7f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4eb7f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4eb7f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4eb7f-108">Attributes</span></span>

|<span data-ttu-id="4eb7f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4eb7f-109">**Attribute**</span></span>|<span data-ttu-id="4eb7f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4eb7f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4eb7f-111">**Attributes**</span><span class="sxs-lookup"><span data-stu-id="4eb7f-111">**Attributes**</span></span> <br/> |<span data-ttu-id="4eb7f-112">Содержит атрибуты группы.</span><span class="sxs-lookup"><span data-stu-id="4eb7f-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4eb7f-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4eb7f-113">Child elements</span></span>

|<span data-ttu-id="4eb7f-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4eb7f-114">**Element**</span></span>|<span data-ttu-id="4eb7f-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4eb7f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4eb7f-116">секуритидентифиер</span><span class="sxs-lookup"><span data-stu-id="4eb7f-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="4eb7f-117">Представляет собой форму языка определения дескрипторов безопасности (SDDL) идентификатора безопасности.</span><span class="sxs-lookup"><span data-stu-id="4eb7f-117">Represents the security descriptor definition language (SDDL) form of a security identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4eb7f-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4eb7f-118">Parent elements</span></span>

|<span data-ttu-id="4eb7f-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4eb7f-119">**Element**</span></span>|<span data-ttu-id="4eb7f-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4eb7f-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4eb7f-121">рестриктедграупсидс</span><span class="sxs-lookup"><span data-stu-id="4eb7f-121">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="4eb7f-122">Представляет коллекцию ограниченных групп в маркере пользователя.</span><span class="sxs-lookup"><span data-stu-id="4eb7f-122">Represents a collection of restricted groups within a user token.</span></span> <span data-ttu-id="4eb7f-123">Сериализация маркеров не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb7f-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4eb7f-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="4eb7f-124">Remarks</span></span>

<span data-ttu-id="4eb7f-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4eb7f-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4eb7f-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4eb7f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4eb7f-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4eb7f-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4eb7f-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4eb7f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4eb7f-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4eb7f-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="4eb7f-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4eb7f-130">Validation File</span></span>  <br/> |<span data-ttu-id="4eb7f-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4eb7f-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4eb7f-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4eb7f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4eb7f-133">False</span><span class="sxs-lookup"><span data-stu-id="4eb7f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4eb7f-134">См. также</span><span class="sxs-lookup"><span data-stu-id="4eb7f-134">See also</span></span>



- [<span data-ttu-id="4eb7f-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4eb7f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

