---
title: ReadFlagChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadFlagChange
api_type:
- schema
ms.assetid: 527bfe90-63d0-4b2f-97f7-7875b3a516b2
description: Элемент ReadFlagChange возвращается в SyncFolderItems операция ответы прочтении элемента. Это свойство доступно только для чтения.
ms.openlocfilehash: 28ef0267e8308ba58057bec01ab2672a19ee94a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834953"
---
# <a name="readflagchange"></a><span data-ttu-id="46ebe-104">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="46ebe-104">ReadFlagChange</span></span>

<span data-ttu-id="46ebe-105">Элемент **ReadFlagChange** возвращается в [операции SyncFolderItems](syncfolderitems-operation.md) ответы прочтении элемента.</span><span class="sxs-lookup"><span data-stu-id="46ebe-105">The **ReadFlagChange** element is returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="46ebe-106">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46ebe-106">This property is read-only.</span></span> 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 <span data-ttu-id="46ebe-107">**SyncFolderItemsReadFlagType**</span><span class="sxs-lookup"><span data-stu-id="46ebe-107">**SyncFolderItemsReadFlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46ebe-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46ebe-108">Attributes and elements</span></span>

<span data-ttu-id="46ebe-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="46ebe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46ebe-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46ebe-110">Attributes</span></span>

<span data-ttu-id="46ebe-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="46ebe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46ebe-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46ebe-112">Child elements</span></span>

|<span data-ttu-id="46ebe-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46ebe-113">**Element**</span></span>|<span data-ttu-id="46ebe-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46ebe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46ebe-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="46ebe-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="46ebe-116">Определяет элемент, для которого был изменен флаг чтения.</span><span class="sxs-lookup"><span data-stu-id="46ebe-116">Identifies the item for which the read-flag has been changed.</span></span>  <br/> |
|[<span data-ttu-id="46ebe-117">IsRead</span><span class="sxs-lookup"><span data-stu-id="46ebe-117">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="46ebe-118">Указывает, является ли флаг чтения имеет значение **true**.</span><span class="sxs-lookup"><span data-stu-id="46ebe-118">Indicates whether the read-flag has been set to **true**.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46ebe-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46ebe-119">Parent elements</span></span>

|<span data-ttu-id="46ebe-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46ebe-120">**Element**</span></span>|<span data-ttu-id="46ebe-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46ebe-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46ebe-122">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="46ebe-122">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="46ebe-123">Содержит массив последовательности типов изменений, которые представляют типы различия между элементами на стороне клиента и элементов на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="46ebe-123">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46ebe-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="46ebe-124">Remarks</span></span>

<span data-ttu-id="46ebe-125">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="46ebe-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46ebe-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46ebe-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46ebe-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46ebe-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46ebe-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46ebe-128">Schema Name</span></span>  <br/> |<span data-ttu-id="46ebe-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="46ebe-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="46ebe-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46ebe-130">Validation File</span></span>  <br/> |<span data-ttu-id="46ebe-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46ebe-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46ebe-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46ebe-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="46ebe-133">False</span><span class="sxs-lookup"><span data-stu-id="46ebe-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46ebe-134">См. также</span><span class="sxs-lookup"><span data-stu-id="46ebe-134">See also</span></span>



- [<span data-ttu-id="46ebe-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46ebe-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

