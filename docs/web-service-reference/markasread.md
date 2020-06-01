---
title: MarkAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkAsRead
api_type:
- schema
ms.assetid: 404842e1-fbdb-480d-a1d8-ba1ab2c9fb1e
description: Элемент Маркасреад указывает, следует ли помечать сообщения как прочтенные.
ms.openlocfilehash: 691409a4eace8885d36f4b30b8eef1aca8c332a6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461767"
---
# <a name="markasread"></a><span data-ttu-id="99d56-103">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="99d56-103">MarkAsRead</span></span>

<span data-ttu-id="99d56-104">Элемент **маркасреад** указывает, следует ли помечать сообщения как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="99d56-104">The **MarkAsRead** element indicates whether messages are to be marked as read.</span></span> 
  
```XML
<MarkAsRead>true | false</MarkAsRead>
```

 <span data-ttu-id="99d56-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="99d56-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99d56-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="99d56-106">Attributes and elements</span></span>

<span data-ttu-id="99d56-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="99d56-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99d56-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="99d56-108">Attributes</span></span>

<span data-ttu-id="99d56-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="99d56-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99d56-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="99d56-110">Child elements</span></span>

<span data-ttu-id="99d56-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="99d56-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99d56-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="99d56-112">Parent elements</span></span>

|<span data-ttu-id="99d56-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99d56-113">**Element**</span></span>|<span data-ttu-id="99d56-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99d56-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99d56-115">Действия</span><span class="sxs-lookup"><span data-stu-id="99d56-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="99d56-116">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="99d56-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="99d56-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="99d56-117">Text value</span></span>

<span data-ttu-id="99d56-118">Текстовое значение **true** указывает, что сообщение должно быть помечено как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="99d56-118">A text value of **true** indicates that the message must be marked as read.</span></span> <span data-ttu-id="99d56-119">Значение **false** указывает, что сообщения не должны помечаться как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="99d56-119">A value of **false** indicates that messages must not be marked as read.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="99d56-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="99d56-120">Remarks</span></span>

<span data-ttu-id="99d56-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="99d56-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99d56-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="99d56-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99d56-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="99d56-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="99d56-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="99d56-124">Schema Name</span></span>  <br/> |<span data-ttu-id="99d56-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="99d56-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="99d56-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="99d56-126">Validation File</span></span>  <br/> |<span data-ttu-id="99d56-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="99d56-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="99d56-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="99d56-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="99d56-129">True</span><span class="sxs-lookup"><span data-stu-id="99d56-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99d56-130">См. также</span><span class="sxs-lookup"><span data-stu-id="99d56-130">See also</span></span>



- [<span data-ttu-id="99d56-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="99d56-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

