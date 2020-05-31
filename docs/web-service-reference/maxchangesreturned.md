---
title: максчанжесретурнед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxChangesReturned
api_type:
- schema
ms.assetid: f471db84-a666-4dfa-9993-8ca9113a0384
description: Элемент Максчанжесретурнед описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации.
ms.openlocfilehash: c3719b12b7e3e2f83a9454c7b68432b375d78614
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834395"
---
# <a name="maxchangesreturned"></a><span data-ttu-id="51b54-103">максчанжесретурнед</span><span class="sxs-lookup"><span data-stu-id="51b54-103">MaxChangesReturned</span></span>

<span data-ttu-id="51b54-104">Элемент **максчанжесретурнед** описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="51b54-104">The **MaxChangesReturned** element describes the maximum number of changes that can be returned in a synchronization response.</span></span> 
  
[<span data-ttu-id="51b54-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="51b54-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="51b54-106">максчанжесретурнед</span><span class="sxs-lookup"><span data-stu-id="51b54-106">MaxChangesReturned</span></span>](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 <span data-ttu-id="51b54-107">**int**</span><span class="sxs-lookup"><span data-stu-id="51b54-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51b54-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="51b54-108">Attributes and elements</span></span>

<span data-ttu-id="51b54-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="51b54-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51b54-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="51b54-110">Attributes</span></span>

<span data-ttu-id="51b54-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="51b54-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51b54-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="51b54-112">Child elements</span></span>

<span data-ttu-id="51b54-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="51b54-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="51b54-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="51b54-114">Parent elements</span></span>

|<span data-ttu-id="51b54-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="51b54-115">**Element**</span></span>|<span data-ttu-id="51b54-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51b54-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51b54-117">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="51b54-117">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="51b54-118">Определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="51b54-118">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="51b54-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="51b54-119">Text value</span></span>

<span data-ttu-id="51b54-120">Текстовое значение представляет целое число, которое описывает максимальное количество элементов, возвращаемых при каждом вызове синхронизации.</span><span class="sxs-lookup"><span data-stu-id="51b54-120">The text value represents an integer that describes the maximum number of items that are returned in a single synchronization call.</span></span> <span data-ttu-id="51b54-121">Значение должно находиться в диапазоне от 1 до 512 включительно.</span><span class="sxs-lookup"><span data-stu-id="51b54-121">The value must be between 1 and 512, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="51b54-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="51b54-122">Remarks</span></span>

<span data-ttu-id="51b54-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="51b54-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51b54-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="51b54-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51b54-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="51b54-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="51b54-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="51b54-126">Schema name</span></span>  <br/> |<span data-ttu-id="51b54-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="51b54-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="51b54-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="51b54-128">Validation file</span></span>  <br/> |<span data-ttu-id="51b54-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="51b54-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="51b54-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="51b54-130">Can be empty</span></span>  <br/> |<span data-ttu-id="51b54-131">False</span><span class="sxs-lookup"><span data-stu-id="51b54-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51b54-132">См. также</span><span class="sxs-lookup"><span data-stu-id="51b54-132">See also</span></span>



[<span data-ttu-id="51b54-133">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="51b54-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="51b54-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="51b54-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

