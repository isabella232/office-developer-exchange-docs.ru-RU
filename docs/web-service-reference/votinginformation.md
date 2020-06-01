---
title: вотингинформатион
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: Элемент Вотингинформатион указывает сведения о голосовании в сообщении голосования и запросе на утверждение, Вхереаппровеандрежектаре параметры голосования.
ms.openlocfilehash: d946ba8c71d19c8cbb1befbe8c4e43e93590ccae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467748"
---
# <a name="votinginformation"></a><span data-ttu-id="ba86e-103">вотингинформатион</span><span class="sxs-lookup"><span data-stu-id="ba86e-103">VotingInformation</span></span>

<span data-ttu-id="ba86e-104">Элемент **вотингинформатион** указывает сведения о голосовании в сообщении голосования и запросе на утверждение, где "утвердить" и "отклонить" — Параметры голосования.</span><span class="sxs-lookup"><span data-stu-id="ba86e-104">The **VotingInformation** element specifies voting information on a voting message and approval request message where "Approve" and "Reject" are the voting options.</span></span> 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 <span data-ttu-id="ba86e-105">**вотингинформатионтипе**</span><span class="sxs-lookup"><span data-stu-id="ba86e-105">**VotingInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba86e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ba86e-106">Attributes and elements</span></span>

<span data-ttu-id="ba86e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ba86e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba86e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ba86e-108">Attributes</span></span>

<span data-ttu-id="ba86e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ba86e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba86e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ba86e-110">Child elements</span></span>

<span data-ttu-id="ba86e-111">[Усероптионс](useroptions.md)  |  [Вотингреспонсе](votingresponse.md)</span><span class="sxs-lookup"><span data-stu-id="ba86e-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba86e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ba86e-112">Parent elements</span></span>

[<span data-ttu-id="ba86e-113">Message</span><span class="sxs-lookup"><span data-stu-id="ba86e-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="ba86e-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="ba86e-114">Remarks</span></span>

<span data-ttu-id="ba86e-115">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ba86e-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ba86e-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba86e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba86e-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ba86e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba86e-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ba86e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba86e-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ba86e-119">Schema Name</span></span>  <br/> |<span data-ttu-id="ba86e-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ba86e-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba86e-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ba86e-121">Validation File</span></span>  <br/> |<span data-ttu-id="ba86e-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ba86e-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba86e-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ba86e-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba86e-124">True</span><span class="sxs-lookup"><span data-stu-id="ba86e-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba86e-125">См. также</span><span class="sxs-lookup"><span data-stu-id="ba86e-125">See also</span></span>



[<span data-ttu-id="ba86e-126">Message</span><span class="sxs-lookup"><span data-stu-id="ba86e-126">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="ba86e-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ba86e-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

