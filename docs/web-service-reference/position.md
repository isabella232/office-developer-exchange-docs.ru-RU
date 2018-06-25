---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: Элемент позиции указывает положение сущности, извлеченные из сообщения.
ms.openlocfilehash: 4bd8f3088891e918e13d5ef1ec8e3e5217cb3fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834853"
---
# <a name="position"></a><span data-ttu-id="f39af-103">Position</span><span class="sxs-lookup"><span data-stu-id="f39af-103">Position</span></span>

<span data-ttu-id="f39af-104">Элемент **позиции** указывает положение сущности, извлеченные из сообщения.</span><span class="sxs-lookup"><span data-stu-id="f39af-104">The **Position** element specifies the position of an entity extracted from a message.</span></span> 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 <span data-ttu-id="f39af-105">**EmailPositionType**</span><span class="sxs-lookup"><span data-stu-id="f39af-105">**EmailPositionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f39af-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f39af-106">Attributes and elements</span></span>

<span data-ttu-id="f39af-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f39af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f39af-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f39af-108">Attributes</span></span>

<span data-ttu-id="f39af-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f39af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f39af-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f39af-110">Child elements</span></span>

<span data-ttu-id="f39af-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f39af-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f39af-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f39af-112">Parent elements</span></span>

<span data-ttu-id="f39af-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [контакт (ContactType)](contact-contacttype.md) | [Телефон (PhoneEntityType)](phone-phoneentitytype.md)  |  [ TaskSuggestion](tasksuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="f39af-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (ContactType)](contact-contacttype.md) | [Phone (PhoneEntityType)](phone-phoneentitytype.md) | [TaskSuggestion](tasksuggestion.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f39af-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f39af-114">Text value</span></span>

<span data-ttu-id="f39af-115">Текстовое значение элемента **положение** — расположение источник извлеченный объект в исходного сообщения.</span><span class="sxs-lookup"><span data-stu-id="f39af-115">The text value of the **Position** element is the location where an extracted entity originated in the source message.</span></span> <span data-ttu-id="f39af-116">Приведены значения параметра текст для элемента **положение** .</span><span class="sxs-lookup"><span data-stu-id="f39af-116">The text values for the **Position** element are:</span></span> 
  
- <span data-ttu-id="f39af-117">**LatestReply** - извлеченный объект исходит от последнего ответа на сообщение.</span><span class="sxs-lookup"><span data-stu-id="f39af-117">**LatestReply** - the extracted entity originates from the latest reply to the message.</span></span> 
    
- <span data-ttu-id="f39af-118">**Другие** - извлеченный объект исходит от undefined часть сообщения.</span><span class="sxs-lookup"><span data-stu-id="f39af-118">**Other** - the extracted entity originates from an undefined part of the message.</span></span> 
    
- <span data-ttu-id="f39af-119">**Тема** - извлеченный объект исходит от теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="f39af-119">**Subject** - the extracted entity originates from the message subject.</span></span> 
    
- <span data-ttu-id="f39af-120">**Подпись** - извлеченный объект исходит от подпись сообщения.</span><span class="sxs-lookup"><span data-stu-id="f39af-120">**Signature** - the extracted entity originates from the message signature.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="f39af-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="f39af-121">Remarks</span></span>

<span data-ttu-id="f39af-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f39af-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f39af-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f39af-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f39af-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f39af-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f39af-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f39af-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f39af-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f39af-126">Schema name</span></span>  <br/> |<span data-ttu-id="f39af-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f39af-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="f39af-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f39af-128">Validation file</span></span>  <br/> |<span data-ttu-id="f39af-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f39af-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f39af-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f39af-130">Can be empty</span></span>  <br/> ||
   

