---
title: Класс SecurityIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SecurityIdentifier
api_type:
- schema
ms.assetid: f7656729-f2c9-41cc-b1ec-60f480fc4dab
description: Класс SecurityIdentifier элемент представляет формы языке SDDL определения дескриптора безопасности идентификатор безопасности (SID).
ms.openlocfilehash: c18d7d4505c618792497c32c7499eab9ac82989e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835314"
---
# <a name="securityidentifier"></a><span data-ttu-id="c5c74-103">Класс SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="c5c74-103">SecurityIdentifier</span></span>

<span data-ttu-id="c5c74-104">**Класс SecurityIdentifier** элемент представляет формы языке SDDL определения дескриптора безопасности идентификатор безопасности ( [SID](sid.md)).</span><span class="sxs-lookup"><span data-stu-id="c5c74-104">The **SecurityIdentifier** element represents the security descriptor definition language (SDDL) form of a security identifier ( [SID](sid.md)).</span></span>
  
```xml
<SecurityIdentifier/>
```

 <span data-ttu-id="c5c74-105">**string**</span><span class="sxs-lookup"><span data-stu-id="c5c74-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5c74-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c5c74-106">Attributes and elements</span></span>

<span data-ttu-id="c5c74-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c5c74-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5c74-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c5c74-108">Attributes</span></span>

<span data-ttu-id="c5c74-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c5c74-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5c74-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c5c74-110">Child elements</span></span>

<span data-ttu-id="c5c74-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c5c74-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5c74-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c5c74-112">Parent elements</span></span>

|<span data-ttu-id="c5c74-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c5c74-113">**Element**</span></span>|<span data-ttu-id="c5c74-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5c74-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5c74-115">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="c5c74-115">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="c5c74-116">Представляет одиночный идентификатор безопасности и атрибут, для которого учетная запись является участником группы объектов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c5c74-116">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> <span data-ttu-id="c5c74-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="c5c74-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[<span data-ttu-id="c5c74-118">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="c5c74-118">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="c5c74-119">Представляет идентификатор группы безопасности и атрибуты, используемые для группа с ограниченным доступом в рамках маркера пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5c74-119">Represents the group security identifier and attributes for a restricted group within a user token.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5c74-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="c5c74-120">Remarks</span></span>

<span data-ttu-id="c5c74-121">Данный элемент используется в заголовке Simple Object Access Protocol (SOAP).</span><span class="sxs-lookup"><span data-stu-id="c5c74-121">This element is used in the Simple Object Access Protocol (SOAP) header.</span></span>
  
<span data-ttu-id="c5c74-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c5c74-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5c74-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c5c74-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5c74-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c5c74-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5c74-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c5c74-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c5c74-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c5c74-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5c74-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c5c74-127">Validation File</span></span>  <br/> |<span data-ttu-id="c5c74-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c5c74-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5c74-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c5c74-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5c74-130">False</span><span class="sxs-lookup"><span data-stu-id="c5c74-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5c74-131">См. также</span><span class="sxs-lookup"><span data-stu-id="c5c74-131">See also</span></span>



- [<span data-ttu-id="c5c74-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c5c74-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

