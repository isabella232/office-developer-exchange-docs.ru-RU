---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: Элемент MarkAsJunk указывает запрос на перемещение элемента в папку нежелательной почты и Добавление отправителя в список заблокированных отправителей.
ms.openlocfilehash: fbb3eee7ce350954888931ca55b27f596656b161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834350"
---
# <a name="markasjunk"></a><span data-ttu-id="29088-103">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="29088-103">MarkAsJunk</span></span>

<span data-ttu-id="29088-104">Элемент **MarkAsJunk** указывает запрос на перемещение элемента в папку нежелательной почты и Добавление отправителя в список заблокированных отправителей.</span><span class="sxs-lookup"><span data-stu-id="29088-104">The **MarkAsJunk** element specifies the request to move an item to the junk mail folder and to add the sender to the blocked sender list.</span></span> 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 <span data-ttu-id="29088-105">**маркасжунктипе**</span><span class="sxs-lookup"><span data-stu-id="29088-105">**MarkAsJunkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29088-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="29088-106">Attributes and elements</span></span>

<span data-ttu-id="29088-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="29088-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29088-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="29088-108">Attributes</span></span>

|<span data-ttu-id="29088-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="29088-109">**Attribute**</span></span>|<span data-ttu-id="29088-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="29088-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29088-111">Нежелательная почта</span><span class="sxs-lookup"><span data-stu-id="29088-111">IsJunk</span></span>  <br/> |<span data-ttu-id="29088-112">Текстовое значение **true** **для атрибута InAttribute** указывает, что отправитель электронной почты добавляется в список заблокированных отправителей.</span><span class="sxs-lookup"><span data-stu-id="29088-112">A text value of **true** for the **IsJunk** attribute indicates that the email sender is added to the blocked sender list.</span></span> <span data-ttu-id="29088-113">Значение **false** указывает, что отправитель электронной почты удаляется из списка заблокированных отправителей, если он уже есть в списке.</span><span class="sxs-lookup"><span data-stu-id="29088-113">A value of **false** indicates that the email sender is removed from the blocked sender list, if the email sender is already on the list.</span></span>  <br/> |
|<span data-ttu-id="29088-114">MoveItem</span><span class="sxs-lookup"><span data-stu-id="29088-114">MoveItem</span></span>  <br/> |<span data-ttu-id="29088-115">Текстовое значение **true** для атрибута **MoveItem** указывает на то, что элемент перемещается в папку нежелательной почты по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29088-115">A text value of **true** for the **MoveItem** attribute indicates that the item is moved to the default junk mail folder.</span></span> <span data-ttu-id="29088-116">Значение **false** указывает на то, что элемент не перемещается в папку нежелательной почты по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29088-116">A value of **false** indicates that the item is not moved to the default junk mail folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="29088-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="29088-117">Child elements</span></span>

[<span data-ttu-id="29088-118">итемидс</span><span class="sxs-lookup"><span data-stu-id="29088-118">ItemIds</span></span>](itemids.md)
  
### <a name="parent-elements"></a><span data-ttu-id="29088-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="29088-119">Parent elements</span></span>

<span data-ttu-id="29088-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="29088-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="29088-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="29088-121">Remarks</span></span>

<span data-ttu-id="29088-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="29088-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="29088-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="29088-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29088-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="29088-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29088-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="29088-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29088-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="29088-126">Schema name</span></span>  <br/> |<span data-ttu-id="29088-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="29088-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="29088-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="29088-128">Validation file</span></span>  <br/> |<span data-ttu-id="29088-129">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="29088-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29088-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="29088-130">Can be empty</span></span>  <br/> ||
   

