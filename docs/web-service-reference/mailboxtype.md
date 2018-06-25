---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: Элемент MailboxType представляет тип почтового ящика, который соответствует адресу электронной почты.
ms.openlocfilehash: d7232377951e8d9c8f191ac856058bc28467cadd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834305"
---
# <a name="mailboxtype"></a><span data-ttu-id="50291-103">MailboxType</span><span class="sxs-lookup"><span data-stu-id="50291-103">MailboxType</span></span>

<span data-ttu-id="50291-104">Элемент **MailboxType** представляет тип почтового ящика, который соответствует адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="50291-104">The **MailboxType** element represents the type of mailbox that is represented by the e-mail address.</span></span> 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

<span data-ttu-id="50291-105">**MailboxTypeType**</span><span class="sxs-lookup"><span data-stu-id="50291-105">**MailboxTypeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="50291-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="50291-106">Attributes and elements</span></span>

<span data-ttu-id="50291-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="50291-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50291-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="50291-108">Attributes</span></span>

<span data-ttu-id="50291-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="50291-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50291-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="50291-110">Child elements</span></span>

<span data-ttu-id="50291-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="50291-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="50291-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="50291-112">Parent elements</span></span>

|<span data-ttu-id="50291-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="50291-113">**Element**</span></span>|<span data-ttu-id="50291-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="50291-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50291-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="50291-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="50291-116">Определяет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="50291-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="50291-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="50291-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="50291-118">Определяет список конференц-залы.</span><span class="sxs-lookup"><span data-stu-id="50291-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="50291-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="50291-119">Text value</span></span>

<span data-ttu-id="50291-120">В следующей таблице приведены возможные значения для элемента **MailboxType** .</span><span class="sxs-lookup"><span data-stu-id="50291-120">The following table lists the possible values for the **MailboxType** element.</span></span> 
  
|<span data-ttu-id="50291-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="50291-121">**Value**</span></span>|<span data-ttu-id="50291-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="50291-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50291-123">Почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="50291-123">Mailbox</span></span>  <br/> |<span data-ttu-id="50291-124">Представляет объект Active Directory, поддержкой электронной почты.</span><span class="sxs-lookup"><span data-stu-id="50291-124">Represents a mail-enabled Active Directory object.</span></span>  <br/> |
|<span data-ttu-id="50291-125">PublicDL</span><span class="sxs-lookup"><span data-stu-id="50291-125">PublicDL</span></span>  <br/> |<span data-ttu-id="50291-126">Представляет открытый список рассылки.</span><span class="sxs-lookup"><span data-stu-id="50291-126">Represents a public distribution list.</span></span>  <br/> |
|<span data-ttu-id="50291-127">PrivateDL</span><span class="sxs-lookup"><span data-stu-id="50291-127">PrivateDL</span></span>  <br/> |<span data-ttu-id="50291-128">Представляет список рассылки закрытый в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="50291-128">Represents a private distribution list in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="50291-129">Контакт</span><span class="sxs-lookup"><span data-stu-id="50291-129">Contact</span></span>  <br/> |<span data-ttu-id="50291-130">Представляет контакт в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="50291-130">Represents a contact in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="50291-131">PublicFolder</span><span class="sxs-lookup"><span data-stu-id="50291-131">PublicFolder</span></span>  <br/> |<span data-ttu-id="50291-132">Представляет общей папки.</span><span class="sxs-lookup"><span data-stu-id="50291-132">Represents a public folder.</span></span>  <br/> |
|<span data-ttu-id="50291-133">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="50291-133">Unknown</span></span>  <br/> |<span data-ttu-id="50291-134">Представляет Неизвестный тип почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="50291-134">Represents an unknown type of mailbox.</span></span>  <br/> |
|<span data-ttu-id="50291-135">OneOff</span><span class="sxs-lookup"><span data-stu-id="50291-135">OneOff</span></span>  <br/> |<span data-ttu-id="50291-136">Представляет элемент одноразовых списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="50291-136">Represents a one-off member of a personal distribution list.</span></span>  <br/> |
|<span data-ttu-id="50291-137">GroupMailbox</span><span class="sxs-lookup"><span data-stu-id="50291-137">GroupMailbox</span></span>  <br/> |<span data-ttu-id="50291-138">Представляет почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="50291-138">Represents a group mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50291-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="50291-139">Remarks</span></span>

<span data-ttu-id="50291-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="50291-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50291-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="50291-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50291-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="50291-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50291-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="50291-143">Schema Name</span></span>  <br/> |<span data-ttu-id="50291-144">Схема Types</span><span class="sxs-lookup"><span data-stu-id="50291-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="50291-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="50291-145">Validation File</span></span>  <br/> |<span data-ttu-id="50291-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="50291-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="50291-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="50291-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="50291-148">False</span><span class="sxs-lookup"><span data-stu-id="50291-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50291-149">См. также</span><span class="sxs-lookup"><span data-stu-id="50291-149">See also</span></span>

- [<span data-ttu-id="50291-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="50291-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

