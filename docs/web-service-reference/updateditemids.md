---
title: упдатедитемидс
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: Элемент Упдатедитемидс указывает идентификаторы обновленных элементов напоминания.
ms.openlocfilehash: 4a87bf50f90e80c0c887ee3a66b9f201ea1c8440
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465038"
---
# <a name="updateditemids"></a><span data-ttu-id="e8538-103">упдатедитемидс</span><span class="sxs-lookup"><span data-stu-id="e8538-103">UpdatedItemIds</span></span>

<span data-ttu-id="e8538-104">Элемент **упдатедитемидс** указывает идентификаторы обновленных элементов напоминания.</span><span class="sxs-lookup"><span data-stu-id="e8538-104">The **UpdatedItemIds** element specifies the identifiers of updated reminder items.</span></span> 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 <span data-ttu-id="e8538-105">**нонемптяррайофитемидстипе**</span><span class="sxs-lookup"><span data-stu-id="e8538-105">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8538-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8538-106">Attributes and elements</span></span>

<span data-ttu-id="e8538-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e8538-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8538-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8538-108">Attributes</span></span>

<span data-ttu-id="e8538-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e8538-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8538-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8538-110">Child elements</span></span>

[<span data-ttu-id="e8538-111">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="e8538-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="e8538-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8538-112">Parent elements</span></span>

[<span data-ttu-id="e8538-113">перформреминдерактионреспонсе</span><span class="sxs-lookup"><span data-stu-id="e8538-113">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="e8538-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="e8538-114">Remarks</span></span>

<span data-ttu-id="e8538-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e8538-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e8538-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8538-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="e8538-117">Если операция [PerformReminderAction](performreminderaction-operation.md) завершилась неудачно или на сервере не было внесено изменений, элемент **упдатедитемидс** возвращается как пустое значение.</span><span class="sxs-lookup"><span data-stu-id="e8538-117">If the [PerformReminderAction](performreminderaction-operation.md) operation did not complete successfully, or no changes were made on the server, the **UpdatedItemIds** element is returned as an empty value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e8538-118">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e8538-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8538-119">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e8538-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8538-120">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e8538-120">Schema Name</span></span>  <br/> |<span data-ttu-id="e8538-121">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e8538-121">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8538-122">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e8538-122">Validation File</span></span>  <br/> |<span data-ttu-id="e8538-123">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e8538-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8538-124">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e8538-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8538-125">True</span><span class="sxs-lookup"><span data-stu-id="e8538-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8538-126">См. также</span><span class="sxs-lookup"><span data-stu-id="e8538-126">See also</span></span>



[<span data-ttu-id="e8538-127">перформреминдерактионреспонсе</span><span class="sxs-lookup"><span data-stu-id="e8538-127">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)


- [<span data-ttu-id="e8538-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e8538-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

