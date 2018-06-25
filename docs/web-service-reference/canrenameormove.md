---
title: CanRenameOrMove
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanRenameOrMove
api_type:
- schema
ms.assetid: fe0cdb04-5f2b-4f1d-9d12-7ace0883cd86
description: Элемент CanRenameOrMove указывает, переименованы или перемещены клиентом управляемых папок.
ms.openlocfilehash: 0303499f5cd54d4a52222e43c2c5f0b389fbcf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761671"
---
# <a name="canrenameormove"></a><span data-ttu-id="c692c-103">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="c692c-103">CanRenameOrMove</span></span>

<span data-ttu-id="c692c-104">Элемент **CanRenameOrMove** указывает, переименованы или перемещены клиентом управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="c692c-104">The **CanRenameOrMove** element indicates whether a managed folder can be renamed or moved by the customer.</span></span> 
  
```xml
<CanRenameOrMove/>
```

 <span data-ttu-id="c692c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c692c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c692c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c692c-106">Attributes and elements</span></span>

<span data-ttu-id="c692c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c692c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c692c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c692c-108">Attributes</span></span>

<span data-ttu-id="c692c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c692c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c692c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c692c-110">Child elements</span></span>

<span data-ttu-id="c692c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c692c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c692c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c692c-112">Parent elements</span></span>

|<span data-ttu-id="c692c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c692c-113">**Element**</span></span>|<span data-ttu-id="c692c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c692c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c692c-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="c692c-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="c692c-116">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="c692c-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c692c-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c692c-117">Text value</span></span>

<span data-ttu-id="c692c-118">Текстовое значение представляет значение типа Boolean.</span><span class="sxs-lookup"><span data-stu-id="c692c-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="c692c-119">Значение **true** показывает, что папка может быть переименованным или перемещенным; значение **false** указывает на папку переименованы или перемещены.</span><span class="sxs-lookup"><span data-stu-id="c692c-119">A value of **true** indicates that the folder can be renamed or moved; a value of **false** indicates that the folder cannot be renamed or moved.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c692c-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="c692c-120">Remarks</span></span>

<span data-ttu-id="c692c-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c692c-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c692c-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c692c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c692c-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c692c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c692c-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c692c-124">Schema name</span></span>  <br/> |<span data-ttu-id="c692c-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c692c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c692c-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c692c-126">Validation file</span></span>  <br/> |<span data-ttu-id="c692c-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c692c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c692c-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c692c-128">Can be empty</span></span>  <br/> |<span data-ttu-id="c692c-129">False</span><span class="sxs-lookup"><span data-stu-id="c692c-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c692c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c692c-130">See also</span></span>



- [<span data-ttu-id="c692c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c692c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

