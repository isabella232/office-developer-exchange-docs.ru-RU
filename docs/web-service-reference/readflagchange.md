---
title: реадфлагчанже
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
description: Элемент Реадфлагчанже возвращается в ответах операции SyncFolderItems, когда был прочитан элемент. Это свойство доступно только для чтения.
ms.openlocfilehash: 354f8085a6ea5b738d8619e2ffeb0fbccefd51da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468308"
---
# <a name="readflagchange"></a><span data-ttu-id="cce9a-104">реадфлагчанже</span><span class="sxs-lookup"><span data-stu-id="cce9a-104">ReadFlagChange</span></span>

<span data-ttu-id="cce9a-105">Элемент **реадфлагчанже** возвращается в ответах [операции SyncFolderItems](syncfolderitems-operation.md) , когда был прочитан элемент.</span><span class="sxs-lookup"><span data-stu-id="cce9a-105">The **ReadFlagChange** element is returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="cce9a-106">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cce9a-106">This property is read-only.</span></span> 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 <span data-ttu-id="cce9a-107">**синкфолдеритемсреадфлагтипе**</span><span class="sxs-lookup"><span data-stu-id="cce9a-107">**SyncFolderItemsReadFlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cce9a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cce9a-108">Attributes and elements</span></span>

<span data-ttu-id="cce9a-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cce9a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cce9a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cce9a-110">Attributes</span></span>

<span data-ttu-id="cce9a-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cce9a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cce9a-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cce9a-112">Child elements</span></span>

|<span data-ttu-id="cce9a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cce9a-113">**Element**</span></span>|<span data-ttu-id="cce9a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cce9a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cce9a-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="cce9a-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="cce9a-116">Определяет элемент, для которого был изменен флаг чтения.</span><span class="sxs-lookup"><span data-stu-id="cce9a-116">Identifies the item for which the read-flag has been changed.</span></span>  <br/> |
|[<span data-ttu-id="cce9a-117">IsRead</span><span class="sxs-lookup"><span data-stu-id="cce9a-117">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="cce9a-118">Указывает, задан ли для флага Read флаг **значение true**.</span><span class="sxs-lookup"><span data-stu-id="cce9a-118">Indicates whether the read-flag has been set to **true**.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cce9a-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cce9a-119">Parent elements</span></span>

|<span data-ttu-id="cce9a-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cce9a-120">**Element**</span></span>|<span data-ttu-id="cce9a-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cce9a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cce9a-122">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="cce9a-122">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="cce9a-123">Содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="cce9a-123">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cce9a-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="cce9a-124">Remarks</span></span>

<span data-ttu-id="cce9a-125">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cce9a-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cce9a-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cce9a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cce9a-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cce9a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cce9a-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cce9a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cce9a-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cce9a-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="cce9a-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cce9a-130">Validation File</span></span>  <br/> |<span data-ttu-id="cce9a-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cce9a-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cce9a-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cce9a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cce9a-133">False</span><span class="sxs-lookup"><span data-stu-id="cce9a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cce9a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="cce9a-134">See also</span></span>



- [<span data-ttu-id="cce9a-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cce9a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

