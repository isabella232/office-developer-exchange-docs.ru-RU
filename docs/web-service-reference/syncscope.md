---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: Элемент SyncScope указывает ли только что элементов или элементы и сведения, папки, связанной возвращаются в ответ синхронизации.
ms.openlocfilehash: 847c0244a8847364e29ea584b0c0b721f00d3064
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840130"
---
# <a name="syncscope"></a><span data-ttu-id="a2119-103">SyncScope</span><span class="sxs-lookup"><span data-stu-id="a2119-103">SyncScope</span></span>

<span data-ttu-id="a2119-104">Элемент **SyncScope** указывает ли только что элементов или элементы и сведения, папки, связанной возвращаются в ответ синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a2119-104">The **SyncScope** element specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 <span data-ttu-id="a2119-105">**SyncFolderItemsScopeType**</span><span class="sxs-lookup"><span data-stu-id="a2119-105">**SyncFolderItemsScopeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2119-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2119-106">Attributes and elements</span></span>

<span data-ttu-id="a2119-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a2119-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2119-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2119-108">Attributes</span></span>

<span data-ttu-id="a2119-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2119-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2119-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2119-110">Child elements</span></span>

<span data-ttu-id="a2119-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2119-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2119-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2119-112">Parent elements</span></span>

|<span data-ttu-id="a2119-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2119-113">**Element**</span></span>|<span data-ttu-id="a2119-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2119-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2119-115">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="a2119-115">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="a2119-116">Элемент, который определяет запрос для синхронизации элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2119-116">The element that defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="a2119-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a2119-117">The following is the XPath expression to this element:</span></span>  <br/> <span data-ttu-id="a2119-118">/ SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="a2119-118">/SyncFolderItems</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2119-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a2119-119">Text value</span></span>

<span data-ttu-id="a2119-120">В следующей таблице приведены возможные значения для элемента **SyncScope** .</span><span class="sxs-lookup"><span data-stu-id="a2119-120">The following table lists the possible values for the **SyncScope** element.</span></span> 
  
<span data-ttu-id="a2119-121">**Значения элементов SyncScope**</span><span class="sxs-lookup"><span data-stu-id="a2119-121">**SyncScope element values**</span></span>

|<span data-ttu-id="a2119-122">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a2119-122">**Value**</span></span>|<span data-ttu-id="a2119-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2119-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2119-124">NormalItems</span><span class="sxs-lookup"><span data-stu-id="a2119-124">NormalItems</span></span>  <br/> |<span data-ttu-id="a2119-125">Указывает, что возвращаются только элементов в папке в ответ синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a2119-125">Specifies that only items in the folder are returned in a synchronization response.</span></span>  <br/> |
|<span data-ttu-id="a2119-126">NormalAndAssociatedItems</span><span class="sxs-lookup"><span data-stu-id="a2119-126">NormalAndAssociatedItems</span></span>  <br/> |<span data-ttu-id="a2119-127">Указывает, что оба элементов в папке и сведений о папке связанного возвращаются в ответ синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a2119-127">Specifies that both items in the folder and folder associated information are returned in a synchronization response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2119-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="a2119-128">Remarks</span></span>

<span data-ttu-id="a2119-129">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a2119-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2119-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2119-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2119-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2119-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a2119-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2119-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a2119-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a2119-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a2119-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2119-134">Validation File</span></span>  <br/> |<span data-ttu-id="a2119-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a2119-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2119-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2119-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2119-137">False</span><span class="sxs-lookup"><span data-stu-id="a2119-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2119-138">См. также</span><span class="sxs-lookup"><span data-stu-id="a2119-138">See also</span></span>



[<span data-ttu-id="a2119-139">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="a2119-139">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="a2119-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2119-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

