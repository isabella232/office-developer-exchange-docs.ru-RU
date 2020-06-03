---
title: GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dd16d1fb-d82d-42e5-b64a-bc6c19c48fa8
description: Элемент GetNonIndexableItemStatistics указывает запрос на получение статистики неиндексируемых элементов.
ms.openlocfilehash: 4b605379f20f5558566f1cfbad9ef1aa33b6fce6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452792"
---
# <a name="getnonindexableitemstatistics"></a><span data-ttu-id="012c8-103">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="012c8-103">GetNonIndexableItemStatistics</span></span>

<span data-ttu-id="012c8-104">Элемент **GetNonIndexableItemStatistics** указывает запрос на получение статистики неиндексируемых элементов.</span><span class="sxs-lookup"><span data-stu-id="012c8-104">The **GetNonIndexableItemStatistics** element specifies a request to retrieve nonindexable item statistics.</span></span> 
  
```XML
<GetNonIndexableItemStatistics>
    <Mailboxes/>
</GetNonIndexableItemStatistics>
```

 <span data-ttu-id="012c8-105">**жетнониндексаблеитемстатистикстипе**</span><span class="sxs-lookup"><span data-stu-id="012c8-105">**GetNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="012c8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="012c8-106">Attributes and elements</span></span>

<span data-ttu-id="012c8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="012c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="012c8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="012c8-108">Attributes</span></span>

<span data-ttu-id="012c8-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="012c8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="012c8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="012c8-110">Child elements</span></span>

|<span data-ttu-id="012c8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="012c8-111">**Element**</span></span>|<span data-ttu-id="012c8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="012c8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="012c8-113">Почтовые ящики (Нонемптяррайофлегациднстипе)</span><span class="sxs-lookup"><span data-stu-id="012c8-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="012c8-114">Указывает массив элементов **почтового ящика** .</span><span class="sxs-lookup"><span data-stu-id="012c8-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="012c8-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="012c8-115">Parent elements</span></span>

<span data-ttu-id="012c8-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="012c8-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="012c8-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="012c8-117">Remarks</span></span>

<span data-ttu-id="012c8-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="012c8-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="012c8-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="012c8-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="012c8-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="012c8-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="012c8-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="012c8-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="012c8-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="012c8-122">Schema Name</span></span>  <br/> |<span data-ttu-id="012c8-123">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="012c8-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="012c8-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="012c8-124">Validation File</span></span>  <br/> |<span data-ttu-id="012c8-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="012c8-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="012c8-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="012c8-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="012c8-127">См. также</span><span class="sxs-lookup"><span data-stu-id="012c8-127">See also</span></span>



- [<span data-ttu-id="012c8-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="012c8-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

