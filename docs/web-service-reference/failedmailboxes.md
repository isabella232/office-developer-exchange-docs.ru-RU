---
title: фаиледмаилбоксес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f34fb6f6-057e-4ae3-8e10-bc92112eafba
description: Элемент Фаиледмаилбоксес указывает массив почтовых ящиков, которые не удалось найти.
ms.openlocfilehash: f68cc29dc9da3b1b74369aa21cde65866e42f3b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762521"
---
# <a name="failedmailboxes"></a><span data-ttu-id="4be2c-103">фаиледмаилбоксес</span><span class="sxs-lookup"><span data-stu-id="4be2c-103">FailedMailboxes</span></span>

<span data-ttu-id="4be2c-104">Элемент **фаиледмаилбоксес** указывает массив почтовых ящиков, которые не удалось найти.</span><span class="sxs-lookup"><span data-stu-id="4be2c-104">The **FailedMailboxes** element specifies an array of mailboxes that failed on search.</span></span> 
  
```XML
<FailedMailboxes>
    <FailedMailbox/>
<FailedMailboxes>
```

 <span data-ttu-id="4be2c-105">**аррайоффаиледсеарчмаилбоксестипе**</span><span class="sxs-lookup"><span data-stu-id="4be2c-105">**ArrayOfFailedSearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4be2c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4be2c-106">Attributes and elements</span></span>

<span data-ttu-id="4be2c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4be2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4be2c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4be2c-108">Attributes</span></span>

<span data-ttu-id="4be2c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4be2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4be2c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4be2c-110">Child elements</span></span>

|<span data-ttu-id="4be2c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4be2c-111">**Element**</span></span>|<span data-ttu-id="4be2c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4be2c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4be2c-113">фаиледмаилбокс</span><span class="sxs-lookup"><span data-stu-id="4be2c-113">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="4be2c-114">Указывает сообщение об ошибке для почтового ящика, на который произошел сбой поиска.</span><span class="sxs-lookup"><span data-stu-id="4be2c-114">Specifies the error message for a mailbox that failed on search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4be2c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4be2c-115">Parent elements</span></span>

|<span data-ttu-id="4be2c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4be2c-116">**Element**</span></span>|<span data-ttu-id="4be2c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4be2c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4be2c-118">сеарчмаилбоксесресулт</span><span class="sxs-lookup"><span data-stu-id="4be2c-118">SearchMailboxesResult</span></span>](searchmailboxesresult.md) <br/> |<span data-ttu-id="4be2c-119">Содержит результат запроса **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="4be2c-119">Contains the result of the **SearchMailboxes** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4be2c-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="4be2c-120">Remarks</span></span>

<span data-ttu-id="4be2c-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4be2c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4be2c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4be2c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4be2c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4be2c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4be2c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4be2c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4be2c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4be2c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4be2c-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4be2c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4be2c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4be2c-127">Validation File</span></span>  <br/> |<span data-ttu-id="4be2c-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4be2c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4be2c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4be2c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4be2c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="4be2c-130">See also</span></span>



- [<span data-ttu-id="4be2c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4be2c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

