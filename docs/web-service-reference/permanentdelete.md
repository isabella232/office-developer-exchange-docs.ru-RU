---
title: перманентделете
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermanentDelete
api_type:
- schema
ms.assetid: 1a0e0f46-1472-4eb7-bb54-f193a2603587
description: Элемент Перманентделете указывает, следует ли окончательно удалять сообщения и не сохранять их в папке "Удаленные".
ms.openlocfilehash: da7680eefca9ad359948af38eac49d18e9055988
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467769"
---
# <a name="permanentdelete"></a><span data-ttu-id="034a2-103">перманентделете</span><span class="sxs-lookup"><span data-stu-id="034a2-103">PermanentDelete</span></span>

<span data-ttu-id="034a2-104">Элемент **перманентделете** указывает, следует ли окончательно удалять сообщения и не сохранять их в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="034a2-104">The **PermanentDelete** element indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span> 
  
```XML
<PermanentDelete>true | false</PermanentDelete>
```

 <span data-ttu-id="034a2-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="034a2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="034a2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="034a2-106">Attributes and elements</span></span>

<span data-ttu-id="034a2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="034a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="034a2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="034a2-108">Attributes</span></span>

<span data-ttu-id="034a2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="034a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="034a2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="034a2-110">Child elements</span></span>

<span data-ttu-id="034a2-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="034a2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="034a2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="034a2-112">Parent elements</span></span>

|<span data-ttu-id="034a2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="034a2-113">**Element**</span></span>|<span data-ttu-id="034a2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="034a2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="034a2-115">Действия</span><span class="sxs-lookup"><span data-stu-id="034a2-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="034a2-116">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="034a2-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="034a2-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="034a2-117">Text value</span></span>

<span data-ttu-id="034a2-118">Текстовое значение **true** указывает на то, что сообщение должно быть помечено для окончательного удаления.</span><span class="sxs-lookup"><span data-stu-id="034a2-118">A text value of **true** indicates that the message must be marked to be permanently deleted.</span></span> <span data-ttu-id="034a2-119">Значение **false** указывает, что сообщение не должно быть помечено для окончательного удаления.</span><span class="sxs-lookup"><span data-stu-id="034a2-119">A value of **false** indicates that the message must not be marked to be permanently deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="034a2-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="034a2-120">Remarks</span></span>

<span data-ttu-id="034a2-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="034a2-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="034a2-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="034a2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="034a2-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="034a2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="034a2-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="034a2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="034a2-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="034a2-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="034a2-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="034a2-126">Validation File</span></span>  <br/> |<span data-ttu-id="034a2-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="034a2-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="034a2-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="034a2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="034a2-129">True</span><span class="sxs-lookup"><span data-stu-id="034a2-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="034a2-130">См. также</span><span class="sxs-lookup"><span data-stu-id="034a2-130">See also</span></span>



- [<span data-ttu-id="034a2-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="034a2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

