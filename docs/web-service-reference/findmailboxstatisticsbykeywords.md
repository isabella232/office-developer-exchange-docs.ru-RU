---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: Элемент FindMailboxStatisticsByKeywords определяет запрос для поиска по ключевым словам статистики почтового ящика.
ms.openlocfilehash: e667f13b66e439dca88d73a5e05d74846183928c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762575"
---
# <a name="findmailboxstatisticsbykeywords"></a><span data-ttu-id="bafb8-103">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="bafb8-103">FindMailboxStatisticsByKeywords</span></span>

<span data-ttu-id="bafb8-104">Элемент **FindMailboxStatisticsByKeywords** определяет запрос для поиска по ключевым словам статистики почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bafb8-104">The **FindMailboxStatisticsByKeywords** element specifies a request to search for mailbox statistics by keyword.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywords>
    <Mailboxes/>
    <Keywords/>
    <Language/>
    <Senders/>
    <Recipients/>
    <FromDate/>
    <ToDate/>
    <MessageTypes/>
    <SearchDumpster/>
    <IncludePersonalArchive/>
    <IncludeUnsearchableItems/>
</FindMailboxStatisticsByKeywords>
```

 <span data-ttu-id="bafb8-105">**FindMailboxStatisticsByKeywordsType**</span><span class="sxs-lookup"><span data-stu-id="bafb8-105">**FindMailboxStatisticsByKeywordsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bafb8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bafb8-106">Attributes and elements</span></span>

<span data-ttu-id="bafb8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bafb8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bafb8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bafb8-108">Attributes</span></span>

<span data-ttu-id="bafb8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bafb8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bafb8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bafb8-110">Child elements</span></span>

|<span data-ttu-id="bafb8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bafb8-111">**Element**</span></span>|<span data-ttu-id="bafb8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bafb8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bafb8-113">Почтовые ящики (ArrayOfUserMailboxesType)</span><span class="sxs-lookup"><span data-stu-id="bafb8-113">Mailboxes (ArrayOfUserMailboxesType)</span></span>](mailboxes-arrayofusermailboxestype.md) <br/> |<span data-ttu-id="bafb8-114">Содержит массив почтовых ящиков, влияет на удержание.</span><span class="sxs-lookup"><span data-stu-id="bafb8-114">Contains an array of mailboxes affected by the hold.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-115">Ключевые слова</span><span class="sxs-lookup"><span data-stu-id="bafb8-115">Keywords</span></span>](keywords-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bafb8-116">Задает ключевые слова для поиска.</span><span class="sxs-lookup"><span data-stu-id="bafb8-116">Specifies keywords for a search.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-117">Language</span><span class="sxs-lookup"><span data-stu-id="bafb8-117">Language</span></span>](language.md) <br/> |<span data-ttu-id="bafb8-118">Содержит язык, используемый для поискового запроса.</span><span class="sxs-lookup"><span data-stu-id="bafb8-118">Contains the language used for the search query.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-119">Отправители</span><span class="sxs-lookup"><span data-stu-id="bafb8-119">Senders</span></span>](senders.md) <br/> |<span data-ttu-id="bafb8-120">Указывает массив SMTP-адреса.</span><span class="sxs-lookup"><span data-stu-id="bafb8-120">Specifies an array of SMTP addresses.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-121">Получатели (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="bafb8-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="bafb8-122">Указывает массив получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="bafb8-122">Specifies an array of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-123">FromDate</span><span class="sxs-lookup"><span data-stu-id="bafb8-123">FromDate</span></span>](fromdate.md) <br/> |<span data-ttu-id="bafb8-124">Дата отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="bafb8-124">Specifies the date that the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-125">ToDate</span><span class="sxs-lookup"><span data-stu-id="bafb8-125">ToDate</span></span>](todate.md) <br/> |<span data-ttu-id="bafb8-126">Указывает дату, которое было получено сообщение.</span><span class="sxs-lookup"><span data-stu-id="bafb8-126">Specifies the date that the message was received.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-127">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="bafb8-127">MessageTypes</span></span>](messagetypes.md) <br/> |<span data-ttu-id="bafb8-128">Указывает массив сообщения для поиска.</span><span class="sxs-lookup"><span data-stu-id="bafb8-128">Specifies an array of messages to search.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-129">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="bafb8-129">SearchDumpster</span></span>](searchdumpster.md) <br/> |<span data-ttu-id="bafb8-130">Указывает, следует ли выполнять поиск в удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="bafb8-130">Specifies whether to search in deleted items.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-131">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="bafb8-131">IncludePersonalArchive</span></span>](includepersonalarchive.md) <br/> |<span data-ttu-id="bafb8-132">Указывает, следует ли включать в поиск личного архива.</span><span class="sxs-lookup"><span data-stu-id="bafb8-132">Specifies whether to include the personal archive in the search.</span></span>  <br/> |
|[<span data-ttu-id="bafb8-133">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="bafb8-133">IncludeUnsearchableItems</span></span>](includeunsearchableitems.md) <br/> |<span data-ttu-id="bafb8-134">Указывает, следует ли включать элементы, которые не удается выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="bafb8-134">Specifies whether to include items that cannot be searched.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bafb8-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bafb8-135">Parent elements</span></span>

<span data-ttu-id="bafb8-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="bafb8-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bafb8-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="bafb8-137">Remarks</span></span>

<span data-ttu-id="bafb8-138">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bafb8-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bafb8-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bafb8-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bafb8-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bafb8-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bafb8-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bafb8-141">Schema Name</span></span>  <br/> |<span data-ttu-id="bafb8-142">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="bafb8-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="bafb8-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bafb8-143">Validation File</span></span>  <br/> |<span data-ttu-id="bafb8-144">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bafb8-144">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bafb8-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bafb8-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bafb8-146">См. также</span><span class="sxs-lookup"><span data-stu-id="bafb8-146">See also</span></span>



- [<span data-ttu-id="bafb8-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bafb8-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

