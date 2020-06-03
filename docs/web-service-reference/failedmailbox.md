---
title: фаиледмаилбокс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: Элемент Фаиледмаилбокс указывает сообщение об ошибке для почтового ящика, на который произошел сбой поиска.
ms.openlocfilehash: 404084bc342eb555db61c4216e936bee6ced9c36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461963"
---
# <a name="failedmailbox"></a><span data-ttu-id="58e60-103">фаиледмаилбокс</span><span class="sxs-lookup"><span data-stu-id="58e60-103">FailedMailbox</span></span>

<span data-ttu-id="58e60-104">Элемент **фаиледмаилбокс** указывает сообщение об ошибке для почтового ящика, на который произошел сбой поиска.</span><span class="sxs-lookup"><span data-stu-id="58e60-104">The **FailedMailbox** element specifies the error message for a mailbox that failed on search.</span></span> 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 <span data-ttu-id="58e60-105">**фаиледсеарчмаилбокстипе**</span><span class="sxs-lookup"><span data-stu-id="58e60-105">**FailedSearchMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58e60-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="58e60-106">Attributes and elements</span></span>

<span data-ttu-id="58e60-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="58e60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58e60-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="58e60-108">Attributes</span></span>

<span data-ttu-id="58e60-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="58e60-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58e60-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="58e60-110">Child elements</span></span>

|<span data-ttu-id="58e60-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="58e60-111">**Element**</span></span>|<span data-ttu-id="58e60-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58e60-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58e60-113">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="58e60-113">Mailbox (string)</span></span>](mailbox-string.md) <br/> |<span data-ttu-id="58e60-114">Содержит идентификатор для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="58e60-114">Contains an identifier for the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="58e60-115">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="58e60-115">ErrorCode (int)</span></span>](errorcode-int.md) <br/> |<span data-ttu-id="58e60-116">Указывает код ошибки почтового ящика, в котором произошел сбой поиска.</span><span class="sxs-lookup"><span data-stu-id="58e60-116">Specifies the error code of the mailbox that failed the search.</span></span>  <br/> |
|[<span data-ttu-id="58e60-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="58e60-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="58e60-118">Представляет причину ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="58e60-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="58e60-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="58e60-119">IsArchive</span></span>](isarchive.md) <br/> |<span data-ttu-id="58e60-120">Задает логическое значение, указывающее, является ли почтовый ящик архивным.</span><span class="sxs-lookup"><span data-stu-id="58e60-120">Specifies a Boolean value that indicates whether the mailbox is an archive.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58e60-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="58e60-121">Parent elements</span></span>

|<span data-ttu-id="58e60-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="58e60-122">**Element**</span></span>|<span data-ttu-id="58e60-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58e60-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58e60-124">фаиледмаилбоксес</span><span class="sxs-lookup"><span data-stu-id="58e60-124">FailedMailboxes</span></span>](failedmailboxes.md) <br/> |<span data-ttu-id="58e60-125">Указывает массив неудачных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="58e60-125">Specifies an array of failed mailboxes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="58e60-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="58e60-126">Remarks</span></span>

<span data-ttu-id="58e60-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="58e60-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="58e60-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="58e60-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58e60-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="58e60-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58e60-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="58e60-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58e60-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="58e60-131">Schema Name</span></span>  <br/> |<span data-ttu-id="58e60-132">Схема типа</span><span class="sxs-lookup"><span data-stu-id="58e60-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="58e60-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="58e60-133">Validation File</span></span>  <br/> |<span data-ttu-id="58e60-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="58e60-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="58e60-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="58e60-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="58e60-136">См. также</span><span class="sxs-lookup"><span data-stu-id="58e60-136">See also</span></span>



- [<span data-ttu-id="58e60-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="58e60-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

