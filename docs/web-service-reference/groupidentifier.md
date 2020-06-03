---
title: граупидентифиер
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
description: Элемент Граупидентифиер представляет один идентификатор безопасности и атрибут для группы объектов службы каталогов Active Directory, членом которой является учетная запись.
ms.openlocfilehash: 8b427b9228cc5e66f46f70389acf2fa4bcd283b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530805"
---
# <a name="groupidentifier"></a><span data-ttu-id="dca55-103">граупидентифиер</span><span class="sxs-lookup"><span data-stu-id="dca55-103">GroupIdentifier</span></span>

<span data-ttu-id="dca55-104">Элемент **граупидентифиер** представляет один идентификатор безопасности и атрибут для группы объектов службы каталогов Active Directory, членом которой является учетная запись.</span><span class="sxs-lookup"><span data-stu-id="dca55-104">The **GroupIdentifier** element represents a single security identifier and attribute for an Active Directory directory service object group of which the account is a member.</span></span> 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 <span data-ttu-id="dca55-105">**сидандаттрибутестипе**</span><span class="sxs-lookup"><span data-stu-id="dca55-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dca55-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dca55-106">Attributes and elements</span></span>

<span data-ttu-id="dca55-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dca55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dca55-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dca55-108">Attributes</span></span>

|<span data-ttu-id="dca55-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="dca55-109">**Attribute**</span></span>|<span data-ttu-id="dca55-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dca55-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dca55-111">**Attributes**</span><span class="sxs-lookup"><span data-stu-id="dca55-111">**Attributes**</span></span> <br/> |<span data-ttu-id="dca55-112">Содержит атрибуты группы.</span><span class="sxs-lookup"><span data-stu-id="dca55-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dca55-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dca55-113">Child elements</span></span>

|<span data-ttu-id="dca55-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dca55-114">**Element**</span></span>|<span data-ttu-id="dca55-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dca55-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dca55-116">секуритидентифиер</span><span class="sxs-lookup"><span data-stu-id="dca55-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="dca55-117">Представляет SDDL-форму идентификатора безопасности ([SID](sid.md)), представляющего группу.</span><span class="sxs-lookup"><span data-stu-id="dca55-117">Represents the security descriptor definition language (SDDL) form of a security identifier ([SID](sid.md)) that represents the group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dca55-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dca55-118">Parent elements</span></span>

|<span data-ttu-id="dca55-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dca55-119">**Element**</span></span>|<span data-ttu-id="dca55-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dca55-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dca55-121">граупсидс</span><span class="sxs-lookup"><span data-stu-id="dca55-121">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="dca55-122">Представляет коллекцию идентификаторов безопасности объектов группы Active Directory, которые составляют маркер учетной записи для сериализации маркеров.</span><span class="sxs-lookup"><span data-stu-id="dca55-122">Represents a collection of Active Directory group object security identifiers that make up an account token for token serialization.</span></span> <span data-ttu-id="dca55-123">Сериализация маркеров не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca55-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dca55-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="dca55-124">Remarks</span></span>

<span data-ttu-id="dca55-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dca55-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dca55-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dca55-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dca55-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dca55-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dca55-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dca55-128">Schema Name</span></span>  <br/> |<span data-ttu-id="dca55-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dca55-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="dca55-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dca55-130">Validation File</span></span>  <br/> |<span data-ttu-id="dca55-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dca55-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dca55-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dca55-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="dca55-133">False</span><span class="sxs-lookup"><span data-stu-id="dca55-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dca55-134">См. также</span><span class="sxs-lookup"><span data-stu-id="dca55-134">See also</span></span>



- [<span data-ttu-id="dca55-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dca55-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

