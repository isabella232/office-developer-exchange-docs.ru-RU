---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: Элемент Position указывает позицию объекта, извлеченного из сообщения.
ms.openlocfilehash: 9acd965c3e0c29f3fa91df338c0671749192b38b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465424"
---
# <a name="position"></a><span data-ttu-id="fbf8f-103">Position</span><span class="sxs-lookup"><span data-stu-id="fbf8f-103">Position</span></span>

<span data-ttu-id="fbf8f-104">Элемент **position** указывает позицию объекта, извлеченного из сообщения.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-104">The **Position** element specifies the position of an entity extracted from a message.</span></span> 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 <span data-ttu-id="fbf8f-105">**емаилпоситионтипе**</span><span class="sxs-lookup"><span data-stu-id="fbf8f-105">**EmailPositionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbf8f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fbf8f-106">Attributes and elements</span></span>

<span data-ttu-id="fbf8f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbf8f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fbf8f-108">Attributes</span></span>

<span data-ttu-id="fbf8f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbf8f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fbf8f-110">Child elements</span></span>

<span data-ttu-id="fbf8f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fbf8f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fbf8f-112">Parent elements</span></span>

<span data-ttu-id="fbf8f-113">[Урлентити](urlentity.md)  |  [Аддрессентити](addressentity.md)  |  [Емаиладдрессентити](emailaddressentity.md)  |  [Свойства meetingsuggestion](meetingsuggestion.md)  |  [Контактное лицо (контакттипе)](contact-contacttype.md)  |  [Телефон (фонинтититипе)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="fbf8f-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (ContactType)](contact-contacttype.md) | [Phone (PhoneEntityType)](phone-phoneentitytype.md) | [TaskSuggestion](tasksuggestion.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="fbf8f-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fbf8f-114">Text value</span></span>

<span data-ttu-id="fbf8f-115">Текстовое значение элемента **position** — это место, в котором извлеченная сущность была создана в исходном сообщении.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-115">The text value of the **Position** element is the location where an extracted entity originated in the source message.</span></span> <span data-ttu-id="fbf8f-116">Текстовые значения для элемента **position** :</span><span class="sxs-lookup"><span data-stu-id="fbf8f-116">The text values for the **Position** element are:</span></span> 
  
- <span data-ttu-id="fbf8f-117">**Латестрепли** — извлеченная сущность поступает из последнего ответа на сообщение.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-117">**LatestReply** - the extracted entity originates from the latest reply to the message.</span></span> 
    
- <span data-ttu-id="fbf8f-118">**Другой** — извлеченная сущность поступает из неопределенной части сообщения.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-118">**Other** - the extracted entity originates from an undefined part of the message.</span></span> 
    
- <span data-ttu-id="fbf8f-119">**Subject** — извлеченная сущность поступает из темы сообщения.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-119">**Subject** - the extracted entity originates from the message subject.</span></span> 
    
- <span data-ttu-id="fbf8f-120">**Подпись** — извлеченная сущность берется из подписи сообщения.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-120">**Signature** - the extracted entity originates from the message signature.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="fbf8f-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="fbf8f-121">Remarks</span></span>

<span data-ttu-id="fbf8f-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fbf8f-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fbf8f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbf8f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fbf8f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbf8f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fbf8f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fbf8f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fbf8f-126">Schema name</span></span>  <br/> |<span data-ttu-id="fbf8f-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fbf8f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="fbf8f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fbf8f-128">Validation file</span></span>  <br/> |<span data-ttu-id="fbf8f-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fbf8f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fbf8f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fbf8f-130">Can be empty</span></span>  <br/> ||
   

