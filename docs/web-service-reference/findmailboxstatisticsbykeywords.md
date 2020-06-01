---
title: финдмаилбоксстатистиксбикэйвордс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: Элемент Финдмаилбоксстатистиксбикэйвордс указывает запрос на поиск статистики почтовых ящиков по ключевому слову.
ms.openlocfilehash: e22c7d8dc849d3fd45d6cb158030cbd82119437e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462530"
---
# <a name="findmailboxstatisticsbykeywords"></a><span data-ttu-id="02892-103">финдмаилбоксстатистиксбикэйвордс</span><span class="sxs-lookup"><span data-stu-id="02892-103">FindMailboxStatisticsByKeywords</span></span>

<span data-ttu-id="02892-104">Элемент **финдмаилбоксстатистиксбикэйвордс** указывает запрос на поиск статистики почтовых ящиков по ключевому слову.</span><span class="sxs-lookup"><span data-stu-id="02892-104">The **FindMailboxStatisticsByKeywords** element specifies a request to search for mailbox statistics by keyword.</span></span> 
  
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

 <span data-ttu-id="02892-105">**финдмаилбоксстатистиксбикэйвордстипе**</span><span class="sxs-lookup"><span data-stu-id="02892-105">**FindMailboxStatisticsByKeywordsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02892-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02892-106">Attributes and elements</span></span>

<span data-ttu-id="02892-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="02892-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02892-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02892-108">Attributes</span></span>

<span data-ttu-id="02892-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="02892-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02892-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02892-110">Child elements</span></span>

|<span data-ttu-id="02892-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02892-111">**Element**</span></span>|<span data-ttu-id="02892-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02892-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02892-113">Почтовые ящики (Аррайофусермаилбоксестипе)</span><span class="sxs-lookup"><span data-stu-id="02892-113">Mailboxes (ArrayOfUserMailboxesType)</span></span>](mailboxes-arrayofusermailboxestype.md) <br/> |<span data-ttu-id="02892-114">Содержит массив почтовых ящиков, на которые влияет удержание.</span><span class="sxs-lookup"><span data-stu-id="02892-114">Contains an array of mailboxes affected by the hold.</span></span>  <br/> |
|[<span data-ttu-id="02892-115">Keywords</span><span class="sxs-lookup"><span data-stu-id="02892-115">Keywords</span></span>](keywords-ex15websvcsotherref.md) <br/> |<span data-ttu-id="02892-116">Задает ключевые слова для поиска.</span><span class="sxs-lookup"><span data-stu-id="02892-116">Specifies keywords for a search.</span></span>  <br/> |
|[<span data-ttu-id="02892-117">Language</span><span class="sxs-lookup"><span data-stu-id="02892-117">Language</span></span>](language.md) <br/> |<span data-ttu-id="02892-118">Содержит язык, используемый для поискового запроса.</span><span class="sxs-lookup"><span data-stu-id="02892-118">Contains the language used for the search query.</span></span>  <br/> |
|[<span data-ttu-id="02892-119">Отправители</span><span class="sxs-lookup"><span data-stu-id="02892-119">Senders</span></span>](senders.md) <br/> |<span data-ttu-id="02892-120">Указывает массив SMTP-адресов.</span><span class="sxs-lookup"><span data-stu-id="02892-120">Specifies an array of SMTP addresses.</span></span>  <br/> |
|[<span data-ttu-id="02892-121">Получатели (Аррайофсмтпаддресстипе)</span><span class="sxs-lookup"><span data-stu-id="02892-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="02892-122">Указывает массив получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="02892-122">Specifies an array of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="02892-123">фромдате</span><span class="sxs-lookup"><span data-stu-id="02892-123">FromDate</span></span>](fromdate.md) <br/> |<span data-ttu-id="02892-124">Указывает дату отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="02892-124">Specifies the date that the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="02892-125">тодате</span><span class="sxs-lookup"><span data-stu-id="02892-125">ToDate</span></span>](todate.md) <br/> |<span data-ttu-id="02892-126">Указывает дату получения сообщения.</span><span class="sxs-lookup"><span data-stu-id="02892-126">Specifies the date that the message was received.</span></span>  <br/> |
|[<span data-ttu-id="02892-127">мессажетипес</span><span class="sxs-lookup"><span data-stu-id="02892-127">MessageTypes</span></span>](messagetypes.md) <br/> |<span data-ttu-id="02892-128">Указывает массив сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="02892-128">Specifies an array of messages to search.</span></span>  <br/> |
|[<span data-ttu-id="02892-129">сеарчдумпстер</span><span class="sxs-lookup"><span data-stu-id="02892-129">SearchDumpster</span></span>](searchdumpster.md) <br/> |<span data-ttu-id="02892-130">Указывает, следует ли выполнять поиск в удаленных элементах.</span><span class="sxs-lookup"><span data-stu-id="02892-130">Specifies whether to search in deleted items.</span></span>  <br/> |
|[<span data-ttu-id="02892-131">инклудеперсоналарчиве</span><span class="sxs-lookup"><span data-stu-id="02892-131">IncludePersonalArchive</span></span>](includepersonalarchive.md) <br/> |<span data-ttu-id="02892-132">Указывает, следует ли включать в поиск личный архив.</span><span class="sxs-lookup"><span data-stu-id="02892-132">Specifies whether to include the personal archive in the search.</span></span>  <br/> |
|[<span data-ttu-id="02892-133">инклудеунсеарчаблеитемс</span><span class="sxs-lookup"><span data-stu-id="02892-133">IncludeUnsearchableItems</span></span>](includeunsearchableitems.md) <br/> |<span data-ttu-id="02892-134">Указывает, следует ли включать элементы, поиск которых невозможен.</span><span class="sxs-lookup"><span data-stu-id="02892-134">Specifies whether to include items that cannot be searched.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02892-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02892-135">Parent elements</span></span>

<span data-ttu-id="02892-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="02892-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="02892-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="02892-137">Remarks</span></span>

<span data-ttu-id="02892-138">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02892-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02892-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02892-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02892-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02892-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02892-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02892-141">Schema Name</span></span>  <br/> |<span data-ttu-id="02892-142">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="02892-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="02892-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02892-143">Validation File</span></span>  <br/> |<span data-ttu-id="02892-144">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="02892-144">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02892-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02892-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="02892-146">См. также</span><span class="sxs-lookup"><span data-stu-id="02892-146">See also</span></span>



- [<span data-ttu-id="02892-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="02892-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

