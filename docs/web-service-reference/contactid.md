---
title: ContactId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86f66275-1e39-48ed-bd89-ac3bffc465a7
description: Элемент ContactId уникально идентифицирует контакт.
ms.openlocfilehash: 4fd3693ed89194c85e5f1770f1db3903d835f43e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761740"
---
# <a name="contactid"></a><span data-ttu-id="895d7-103">ContactId</span><span class="sxs-lookup"><span data-stu-id="895d7-103">ContactId</span></span>

<span data-ttu-id="895d7-104">Элемент **ContactId** уникально идентифицирует контакт.</span><span class="sxs-lookup"><span data-stu-id="895d7-104">The **ContactId** element uniquely identifies a contact.</span></span> 
  
```XML
<ContactId Id="" ChangeKey=""/>
```

 <span data-ttu-id="895d7-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="895d7-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="895d7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="895d7-106">Attributes and elements</span></span>

<span data-ttu-id="895d7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="895d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="895d7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="895d7-108">Attributes</span></span>

|<span data-ttu-id="895d7-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="895d7-109">**Attribute**</span></span>|<span data-ttu-id="895d7-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="895d7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="895d7-111">Id</span><span class="sxs-lookup"><span data-stu-id="895d7-111">Id</span></span>  <br/> |<span data-ttu-id="895d7-112">Текстовое значение атрибута **Id** — идентификатор элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="895d7-112">The text value of the **Id** attribute is the identifier of the contact item.</span></span>  <br/> |
|<span data-ttu-id="895d7-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="895d7-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="895d7-114">Текстовое значение атрибута **ChangeKey** — это ключ изменения элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="895d7-114">The text value of the **ChangeKey** attribute is the change key of the contact item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="895d7-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="895d7-115">Child elements</span></span>

<span data-ttu-id="895d7-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="895d7-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="895d7-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="895d7-117">Parent elements</span></span>

<span data-ttu-id="895d7-118">[AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md)</span><span class="sxs-lookup"><span data-stu-id="895d7-118">[AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="895d7-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="895d7-119">Remarks</span></span>

<span data-ttu-id="895d7-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="895d7-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="895d7-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="895d7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="895d7-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="895d7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="895d7-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="895d7-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="895d7-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="895d7-124">Schema name</span></span>  <br/> |<span data-ttu-id="895d7-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="895d7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="895d7-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="895d7-126">Validation file</span></span>  <br/> |<span data-ttu-id="895d7-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="895d7-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="895d7-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="895d7-128">Can be empty</span></span>  <br/> |<span data-ttu-id="895d7-129">Нет</span><span class="sxs-lookup"><span data-stu-id="895d7-129">false</span></span>  <br/> |
   
