---
title: GroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: Элемент GroupSids представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.
ms.openlocfilehash: c24c8ea3c3b7d37f41986997ed924c951b4a48ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833790"
---
# <a name="groupsids"></a><span data-ttu-id="e8038-103">GroupSids</span><span class="sxs-lookup"><span data-stu-id="e8038-103">GroupSids</span></span>

<span data-ttu-id="e8038-104">Элемент **GroupSids** представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8038-104">The **GroupSids** element represents a collection of Active Directory directory service group object security identifiers.</span></span> 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 <span data-ttu-id="e8038-105">**NonEmptyArrayOfGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="e8038-105">**NonEmptyArrayOfGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8038-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8038-106">Attributes and elements</span></span>

<span data-ttu-id="e8038-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e8038-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8038-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8038-108">Attributes</span></span>

<span data-ttu-id="e8038-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e8038-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8038-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8038-110">Child elements</span></span>

|<span data-ttu-id="e8038-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8038-111">**Element**</span></span>|<span data-ttu-id="e8038-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8038-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8038-113">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="e8038-113">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="e8038-114">Представляет одиночный идентификатор безопасности и атрибут, для которого учетная запись является участником группы объектов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e8038-114">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8038-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8038-115">Parent elements</span></span>

|<span data-ttu-id="e8038-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8038-116">**Element**</span></span>|<span data-ttu-id="e8038-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8038-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8038-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="e8038-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="e8038-119">Используется в заголовке Simple Object Access Protocol (SOAP) для сериализации маркера проверки подлинности сервер сервер.</span><span class="sxs-lookup"><span data-stu-id="e8038-119">Used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="e8038-120">Сериализация маркера не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8038-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e8038-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="e8038-121">Remarks</span></span>

<span data-ttu-id="e8038-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e8038-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8038-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e8038-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8038-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e8038-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8038-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e8038-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e8038-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e8038-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8038-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e8038-127">Validation File</span></span>  <br/> |<span data-ttu-id="e8038-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e8038-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8038-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e8038-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8038-130">False</span><span class="sxs-lookup"><span data-stu-id="e8038-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8038-131">См. также</span><span class="sxs-lookup"><span data-stu-id="e8038-131">See also</span></span>



- [<span data-ttu-id="e8038-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e8038-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

