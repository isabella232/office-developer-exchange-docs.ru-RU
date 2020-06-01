---
title: полицитаг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: Элемент Полицитаг указывает идентификатор хранения для элемента или папки.
ms.openlocfilehash: ddc4d890d1e514586ba5ea7f6a8b541b2e4786c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460899"
---
# <a name="policytag"></a><span data-ttu-id="f9289-103">полицитаг</span><span class="sxs-lookup"><span data-stu-id="f9289-103">PolicyTag</span></span>

<span data-ttu-id="f9289-104">Элемент **полицитаг** указывает идентификатор хранения для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="f9289-104">The **PolicyTag** element specifies the retention identifier on an item or folder.</span></span> 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 <span data-ttu-id="f9289-105">**ретентионтагтипе**</span><span class="sxs-lookup"><span data-stu-id="f9289-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9289-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f9289-106">Attributes and elements</span></span>

<span data-ttu-id="f9289-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f9289-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9289-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f9289-108">Attributes</span></span>

|<span data-ttu-id="f9289-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f9289-109">**Attribute**</span></span>|<span data-ttu-id="f9289-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f9289-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9289-111">Явный</span><span class="sxs-lookup"><span data-stu-id="f9289-111">IsExplicit</span></span>  <br/> |<span data-ttu-id="f9289-112">Указывает, был ли явно задан тег политики для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="f9289-112">Indicates whether a policy tag was explicitly set on an item or folder.</span></span>  <br/> <span data-ttu-id="f9289-113">Текстовое значение **true** для атрибута **explicit** указывает на то, что тег политики был явно задан для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="f9289-113">A text value of **true** for the **IsExplicit** attribute indicates that the policy tag was explicitly set on the item or folder.</span></span> <span data-ttu-id="f9289-114">Текстовое значение **false** указывает на то, что тег политики неявно задан для элемента или папки на основе тега политики родительской папки.</span><span class="sxs-lookup"><span data-stu-id="f9289-114">A text value of **false** indicates that the policy tag was implicitly set on the item or folder based on the parent folder policy tag.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f9289-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f9289-115">Child elements</span></span>

<span data-ttu-id="f9289-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f9289-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f9289-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f9289-117">Parent elements</span></span>

<span data-ttu-id="f9289-118">[Сеарчпревиевитем](searchpreviewitem.md)  |  [Элемент](item.md)  |  [Contact (контакт](contact.md)  |  ) [Message (сообщение](message-ex15websvcsotherref.md)  |  ) [Дистрибутионлист](distributionlist.md)  |  [Календаритем](calendaritem.md)  |  [Элемент](postitem.md)  |  i [Task (задача](task.md) )</span><span class="sxs-lookup"><span data-stu-id="f9289-118">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f9289-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f9289-119">Text value</span></span>

<span data-ttu-id="f9289-120">Текстовое значение элемента **полицитаг** — идентификатор тега политики.</span><span class="sxs-lookup"><span data-stu-id="f9289-120">The text value of the **PolicyTag** element is the policy tag identifier.</span></span> <span data-ttu-id="f9289-121">Идентификатор тега политики — GUID.</span><span class="sxs-lookup"><span data-stu-id="f9289-121">The policy tag identifier is a GUID.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f9289-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="f9289-122">Remarks</span></span>

<span data-ttu-id="f9289-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f9289-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f9289-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9289-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9289-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f9289-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9289-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f9289-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9289-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f9289-127">Schema name</span></span>  <br/> |<span data-ttu-id="f9289-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f9289-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9289-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f9289-129">Validation file</span></span>  <br/> |<span data-ttu-id="f9289-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f9289-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9289-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f9289-131">Can be empty</span></span>  <br/> ||
   

