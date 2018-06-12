---
title: FailedMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f34fb6f6-057e-4ae3-8e10-bc92112eafba
description: Элемент FailedMailboxes указывает массив почтовых ящиков, которые не удалось на поиска.
ms.openlocfilehash: f68cc29dc9da3b1b74369aa21cde65866e42f3b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762521"
---
# <a name="failedmailboxes"></a><span data-ttu-id="9f380-103">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="9f380-103">FailedMailboxes</span></span>

<span data-ttu-id="9f380-104">Элемент **FailedMailboxes** указывает массив почтовых ящиков, которые не удалось на поиска.</span><span class="sxs-lookup"><span data-stu-id="9f380-104">The **FailedMailboxes** element specifies an array of mailboxes that failed on search.</span></span> 
  
```XML
<FailedMailboxes>
    <FailedMailbox/>
<FailedMailboxes>
```

 <span data-ttu-id="9f380-105">**ArrayOfFailedSearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="9f380-105">**ArrayOfFailedSearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f380-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9f380-106">Attributes and elements</span></span>

<span data-ttu-id="9f380-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9f380-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f380-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9f380-108">Attributes</span></span>

<span data-ttu-id="9f380-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9f380-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f380-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9f380-110">Child elements</span></span>

|<span data-ttu-id="9f380-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9f380-111">**Element**</span></span>|<span data-ttu-id="9f380-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f380-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f380-113">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="9f380-113">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="9f380-114">Задает сообщение об ошибке для почтового ящика, который не удалось на поиска.</span><span class="sxs-lookup"><span data-stu-id="9f380-114">Specifies the error message for a mailbox that failed on search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f380-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9f380-115">Parent elements</span></span>

|<span data-ttu-id="9f380-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9f380-116">**Element**</span></span>|<span data-ttu-id="9f380-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f380-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f380-118">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="9f380-118">SearchMailboxesResult</span></span>](searchmailboxesresult.md) <br/> |<span data-ttu-id="9f380-119">Содержит результат запроса **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="9f380-119">Contains the result of the **SearchMailboxes** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f380-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="9f380-120">Remarks</span></span>

<span data-ttu-id="9f380-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9f380-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f380-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f380-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f380-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9f380-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f380-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9f380-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f380-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9f380-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9f380-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="9f380-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9f380-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9f380-127">Validation File</span></span>  <br/> |<span data-ttu-id="9f380-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9f380-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f380-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9f380-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9f380-130">См. также</span><span class="sxs-lookup"><span data-stu-id="9f380-130">See also</span></span>



- [<span data-ttu-id="9f380-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9f380-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

