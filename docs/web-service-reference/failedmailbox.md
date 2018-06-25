---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: Элемент FailedMailbox указывает сообщение об ошибке для почтового ящика, который не удалось на поиска.
ms.openlocfilehash: a4f5cd975eba121dd1d8d918b638d34f907588a8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762522"
---
# <a name="failedmailbox"></a><span data-ttu-id="534dd-103">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="534dd-103">FailedMailbox</span></span>

<span data-ttu-id="534dd-104">Элемент **FailedMailbox** указывает сообщение об ошибке для почтового ящика, который не удалось на поиска.</span><span class="sxs-lookup"><span data-stu-id="534dd-104">The **FailedMailbox** element specifies the error message for a mailbox that failed on search.</span></span> 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 <span data-ttu-id="534dd-105">**FailedSearchMailboxType**</span><span class="sxs-lookup"><span data-stu-id="534dd-105">**FailedSearchMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="534dd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="534dd-106">Attributes and elements</span></span>

<span data-ttu-id="534dd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="534dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="534dd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="534dd-108">Attributes</span></span>

<span data-ttu-id="534dd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="534dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="534dd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="534dd-110">Child elements</span></span>

|<span data-ttu-id="534dd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="534dd-111">**Element**</span></span>|<span data-ttu-id="534dd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="534dd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="534dd-113">Почтовый ящик (строка)</span><span class="sxs-lookup"><span data-stu-id="534dd-113">Mailbox (string)</span></span>](mailbox-string.md) <br/> |<span data-ttu-id="534dd-114">Содержит идентификатор для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="534dd-114">Contains an identifier for the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="534dd-115">Код ошибки (int)</span><span class="sxs-lookup"><span data-stu-id="534dd-115">ErrorCode (int)</span></span>](errorcode-int.md) <br/> |<span data-ttu-id="534dd-116">Задает код ошибки для почтового ящика, который не удалось выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="534dd-116">Specifies the error code of the mailbox that failed the search.</span></span>  <br/> |
|[<span data-ttu-id="534dd-117">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="534dd-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="534dd-118">Представляет причину ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="534dd-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="534dd-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="534dd-119">IsArchive</span></span>](isarchive.md) <br/> |<span data-ttu-id="534dd-120">Задает логическое значение, указывающее, является ли почтовом ящике архив.</span><span class="sxs-lookup"><span data-stu-id="534dd-120">Specifies a Boolean value that indicates whether the mailbox is an archive.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="534dd-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="534dd-121">Parent elements</span></span>

|<span data-ttu-id="534dd-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="534dd-122">**Element**</span></span>|<span data-ttu-id="534dd-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="534dd-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="534dd-124">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="534dd-124">FailedMailboxes</span></span>](failedmailboxes.md) <br/> |<span data-ttu-id="534dd-125">Указывает массив неудачных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="534dd-125">Specifies an array of failed mailboxes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="534dd-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="534dd-126">Remarks</span></span>

<span data-ttu-id="534dd-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="534dd-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="534dd-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="534dd-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="534dd-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="534dd-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="534dd-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="534dd-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="534dd-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="534dd-131">Schema Name</span></span>  <br/> |<span data-ttu-id="534dd-132">Схема типа</span><span class="sxs-lookup"><span data-stu-id="534dd-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="534dd-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="534dd-133">Validation File</span></span>  <br/> |<span data-ttu-id="534dd-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="534dd-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="534dd-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="534dd-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="534dd-136">См. также</span><span class="sxs-lookup"><span data-stu-id="534dd-136">See also</span></span>



- [<span data-ttu-id="534dd-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="534dd-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

