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
ms.openlocfilehash: caf96b6e95f2e63d0e544ead26fbea18cd637861
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460087"
---
# <a name="maxchangesreturned"></a><span data-ttu-id="1030b-103">максчанжесретурнед</span><span class="sxs-lookup"><span data-stu-id="1030b-103">MaxChangesReturned</span></span>

<span data-ttu-id="1030b-104">Элемент **максчанжесретурнед** описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1030b-104">The **MaxChangesReturned** element describes the maximum number of changes that can be returned in a synchronization response.</span></span> 
  
[<span data-ttu-id="1030b-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="1030b-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="1030b-106">максчанжесретурнед</span><span class="sxs-lookup"><span data-stu-id="1030b-106">MaxChangesReturned</span></span>](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 <span data-ttu-id="1030b-107">**int**</span><span class="sxs-lookup"><span data-stu-id="1030b-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1030b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1030b-108">Attributes and elements</span></span>

<span data-ttu-id="1030b-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1030b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1030b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1030b-110">Attributes</span></span>

<span data-ttu-id="1030b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1030b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1030b-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1030b-112">Child elements</span></span>

<span data-ttu-id="1030b-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1030b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1030b-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1030b-114">Parent elements</span></span>

|<span data-ttu-id="1030b-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1030b-115">**Element**</span></span>|<span data-ttu-id="1030b-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1030b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1030b-117">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="1030b-117">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="1030b-118">Определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="1030b-118">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1030b-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1030b-119">Text value</span></span>

<span data-ttu-id="1030b-120">Текстовое значение представляет целое число, которое описывает максимальное количество элементов, возвращаемых при каждом вызове синхронизации.</span><span class="sxs-lookup"><span data-stu-id="1030b-120">The text value represents an integer that describes the maximum number of items that are returned in a single synchronization call.</span></span> <span data-ttu-id="1030b-121">Значение должно находиться в диапазоне от 1 до 512 включительно.</span><span class="sxs-lookup"><span data-stu-id="1030b-121">The value must be between 1 and 512, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1030b-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="1030b-122">Remarks</span></span>

<span data-ttu-id="1030b-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1030b-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1030b-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1030b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1030b-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1030b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1030b-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1030b-126">Schema name</span></span>  <br/> |<span data-ttu-id="1030b-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1030b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="1030b-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1030b-128">Validation file</span></span>  <br/> |<span data-ttu-id="1030b-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1030b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1030b-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1030b-130">Can be empty</span></span>  <br/> |<span data-ttu-id="1030b-131">False</span><span class="sxs-lookup"><span data-stu-id="1030b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1030b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="1030b-132">See also</span></span>



[<span data-ttu-id="1030b-133">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="1030b-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="1030b-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1030b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

