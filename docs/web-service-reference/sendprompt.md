---
title: сендпромпт
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: Элемент Сендпромпт указывает тип действия, разрешенного для параметра голосования.
ms.openlocfilehash: 98ffc69cdc94c3f7b9c325bee0c1ebaeb407ee96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462103"
---
# <a name="sendprompt"></a><span data-ttu-id="75650-103">сендпромпт</span><span class="sxs-lookup"><span data-stu-id="75650-103">SendPrompt</span></span>

<span data-ttu-id="75650-104">Элемент **сендпромпт** указывает тип действия, разрешенного для параметра голосования.</span><span class="sxs-lookup"><span data-stu-id="75650-104">The **SendPrompt** element specifies the type of action allowed for a voting option.</span></span> 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 <span data-ttu-id="75650-105">**сендпромпттипе**</span><span class="sxs-lookup"><span data-stu-id="75650-105">**SendPromptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75650-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="75650-106">Attributes and elements</span></span>

<span data-ttu-id="75650-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="75650-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75650-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="75650-108">Attributes</span></span>

<span data-ttu-id="75650-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="75650-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75650-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="75650-110">Child elements</span></span>

<span data-ttu-id="75650-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="75650-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75650-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="75650-112">Parent elements</span></span>

[<span data-ttu-id="75650-113">вотингоптиондата</span><span class="sxs-lookup"><span data-stu-id="75650-113">VotingOptionData</span></span>](votingoptiondata.md)
  
## <a name="text-value"></a><span data-ttu-id="75650-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="75650-114">Text value</span></span>

<span data-ttu-id="75650-115">Текстовое значение элемента **сендпромпт** — действие параметра голосования.</span><span class="sxs-lookup"><span data-stu-id="75650-115">The text value of the **SendPrompt** element is a voting option action.</span></span> <span data-ttu-id="75650-116">В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="75650-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="75650-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="75650-117">**Value**</span></span>|<span data-ttu-id="75650-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75650-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="75650-119">Нет</span><span class="sxs-lookup"><span data-stu-id="75650-119">None</span></span>  <br/> |<span data-ttu-id="75650-120">Действие отсутствует.</span><span class="sxs-lookup"><span data-stu-id="75650-120">No action.</span></span>  <br/> |
|<span data-ttu-id="75650-121">Отправить</span><span class="sxs-lookup"><span data-stu-id="75650-121">Send</span></span>  <br/> |<span data-ttu-id="75650-122">Ответ отправляется немедленно.</span><span class="sxs-lookup"><span data-stu-id="75650-122">The response is sent immediately.</span></span>  <br/> |
|<span data-ttu-id="75650-123">вотингоптион</span><span class="sxs-lookup"><span data-stu-id="75650-123">VotingOption</span></span>  <br/> |<span data-ttu-id="75650-124">Утверждающее лицо может вводить комментарии при утверждении или отклонении.</span><span class="sxs-lookup"><span data-stu-id="75650-124">The approver can enter comments while approving or rejecting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="75650-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="75650-125">Remarks</span></span>

<span data-ttu-id="75650-126">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="75650-126">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="75650-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="75650-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75650-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="75650-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75650-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="75650-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75650-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="75650-130">Schema Name</span></span>  <br/> |<span data-ttu-id="75650-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="75650-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="75650-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="75650-132">Validation File</span></span>  <br/> |<span data-ttu-id="75650-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="75650-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75650-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="75650-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="75650-135">True</span><span class="sxs-lookup"><span data-stu-id="75650-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75650-136">См. также</span><span class="sxs-lookup"><span data-stu-id="75650-136">See also</span></span>



[<span data-ttu-id="75650-137">вотингоптиондата</span><span class="sxs-lookup"><span data-stu-id="75650-137">VotingOptionData</span></span>](votingoptiondata.md)


- [<span data-ttu-id="75650-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="75650-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

