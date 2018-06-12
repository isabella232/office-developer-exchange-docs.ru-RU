---
title: MaxChangesReturned
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
description: Элемент MaxChangesReturned описывает максимальное число изменений, которые могут возвращаться в ответ синхронизации.
ms.openlocfilehash: c3719b12b7e3e2f83a9454c7b68432b375d78614
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834395"
---
# <a name="maxchangesreturned"></a><span data-ttu-id="78ed7-103">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="78ed7-103">MaxChangesReturned</span></span>

<span data-ttu-id="78ed7-104">Элемент **MaxChangesReturned** описывает максимальное число изменений, которые могут возвращаться в ответ синхронизации.</span><span class="sxs-lookup"><span data-stu-id="78ed7-104">The **MaxChangesReturned** element describes the maximum number of changes that can be returned in a synchronization response.</span></span> 
  
[<span data-ttu-id="78ed7-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="78ed7-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="78ed7-106">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="78ed7-106">MaxChangesReturned</span></span>](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 <span data-ttu-id="78ed7-107">**int**</span><span class="sxs-lookup"><span data-stu-id="78ed7-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78ed7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="78ed7-108">Attributes and elements</span></span>

<span data-ttu-id="78ed7-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="78ed7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78ed7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="78ed7-110">Attributes</span></span>

<span data-ttu-id="78ed7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="78ed7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78ed7-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="78ed7-112">Child elements</span></span>

<span data-ttu-id="78ed7-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="78ed7-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78ed7-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="78ed7-114">Parent elements</span></span>

|<span data-ttu-id="78ed7-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="78ed7-115">**Element**</span></span>|<span data-ttu-id="78ed7-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="78ed7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78ed7-117">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="78ed7-117">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="78ed7-118">Определяет запрос для синхронизации элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="78ed7-118">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78ed7-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="78ed7-119">Text value</span></span>

<span data-ttu-id="78ed7-120">Текстовое значение представляет целое число, которое описывает максимальное число элементов, возвращаемых в ходе вызова одного синхронизации.</span><span class="sxs-lookup"><span data-stu-id="78ed7-120">The text value represents an integer that describes the maximum number of items that are returned in a single synchronization call.</span></span> <span data-ttu-id="78ed7-121">Значение должно быть в диапазоне от 1 до 512, включительно.</span><span class="sxs-lookup"><span data-stu-id="78ed7-121">The value must be between 1 and 512, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="78ed7-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="78ed7-122">Remarks</span></span>

<span data-ttu-id="78ed7-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="78ed7-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78ed7-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="78ed7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78ed7-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="78ed7-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78ed7-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="78ed7-126">Schema name</span></span>  <br/> |<span data-ttu-id="78ed7-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="78ed7-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="78ed7-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="78ed7-128">Validation file</span></span>  <br/> |<span data-ttu-id="78ed7-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78ed7-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78ed7-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="78ed7-130">Can be empty</span></span>  <br/> |<span data-ttu-id="78ed7-131">False</span><span class="sxs-lookup"><span data-stu-id="78ed7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78ed7-132">См. также</span><span class="sxs-lookup"><span data-stu-id="78ed7-132">See also</span></span>



[<span data-ttu-id="78ed7-133">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="78ed7-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="78ed7-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="78ed7-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

