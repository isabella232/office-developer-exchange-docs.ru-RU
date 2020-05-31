---
title: канренамеормове
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
description: Элемент Канренамеормове указывает, можно ли переименовать или переместить управляемую папку клиентом.
ms.openlocfilehash: 0303499f5cd54d4a52222e43c2c5f0b389fbcf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761671"
---
# <a name="canrenameormove"></a><span data-ttu-id="fd877-103">канренамеормове</span><span class="sxs-lookup"><span data-stu-id="fd877-103">CanRenameOrMove</span></span>

<span data-ttu-id="fd877-104">Элемент **канренамеормове** указывает, можно ли переименовать или переместить управляемую папку клиентом.</span><span class="sxs-lookup"><span data-stu-id="fd877-104">The **CanRenameOrMove** element indicates whether a managed folder can be renamed or moved by the customer.</span></span> 
  
```xml
<CanRenameOrMove/>
```

 <span data-ttu-id="fd877-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fd877-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd877-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fd877-106">Attributes and elements</span></span>

<span data-ttu-id="fd877-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fd877-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd877-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fd877-108">Attributes</span></span>

<span data-ttu-id="fd877-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd877-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd877-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fd877-110">Child elements</span></span>

<span data-ttu-id="fd877-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd877-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd877-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fd877-112">Parent elements</span></span>

|<span data-ttu-id="fd877-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fd877-113">**Element**</span></span>|<span data-ttu-id="fd877-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd877-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd877-115">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="fd877-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="fd877-116">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="fd877-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd877-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fd877-117">Text value</span></span>

<span data-ttu-id="fd877-118">Текстовое значение представляет логическое значение.</span><span class="sxs-lookup"><span data-stu-id="fd877-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="fd877-119">Значение **true** указывает, что папка может быть переименована или перемещена; значение **false** указывает, что папка не может быть переименована или перемещена.</span><span class="sxs-lookup"><span data-stu-id="fd877-119">A value of **true** indicates that the folder can be renamed or moved; a value of **false** indicates that the folder cannot be renamed or moved.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fd877-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="fd877-120">Remarks</span></span>

<span data-ttu-id="fd877-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fd877-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd877-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fd877-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd877-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fd877-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd877-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fd877-124">Schema name</span></span>  <br/> |<span data-ttu-id="fd877-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fd877-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd877-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fd877-126">Validation file</span></span>  <br/> |<span data-ttu-id="fd877-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fd877-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd877-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fd877-128">Can be empty</span></span>  <br/> |<span data-ttu-id="fd877-129">False</span><span class="sxs-lookup"><span data-stu-id="fd877-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd877-130">См. также</span><span class="sxs-lookup"><span data-stu-id="fd877-130">See also</span></span>



- [<span data-ttu-id="fd877-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fd877-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

