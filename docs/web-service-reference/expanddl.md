---
title: ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: affe84a5-ad98-4aba-83f4-8732938b763d
description: Элемент ExpandDL определяет запрос на расширение списка рассылки.
ms.openlocfilehash: ef93ed4684427a74a4fd2c38b4020ecb743fbaaf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762427"
---
# <a name="expanddl"></a><span data-ttu-id="ed0c3-103">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="ed0c3-103">ExpandDL</span></span>

<span data-ttu-id="ed0c3-104">Элемент **ExpandDL** определяет запрос на расширение списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="ed0c3-104">The **ExpandDL** element defines a request to expand a distribution list.</span></span> 
  
```xml
<ExpandDL>
   <Mailbox/>
</ExpandDL>
```

 <span data-ttu-id="ed0c3-105">**експанддлтипе**</span><span class="sxs-lookup"><span data-stu-id="ed0c3-105">**ExpandDLType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed0c3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ed0c3-106">Attributes and elements</span></span>

<span data-ttu-id="ed0c3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ed0c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed0c3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ed0c3-108">Attributes</span></span>

<span data-ttu-id="ed0c3-109">Нет</span><span class="sxs-lookup"><span data-stu-id="ed0c3-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed0c3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ed0c3-110">Child elements</span></span>

|<span data-ttu-id="ed0c3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ed0c3-111">**Element**</span></span>|<span data-ttu-id="ed0c3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ed0c3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed0c3-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="ed0c3-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ed0c3-114">Определяет полностью разрешенный адрес электронной почты или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="ed0c3-114">Identifies a fully resolved e-mail address or a distribution list.</span></span> <span data-ttu-id="ed0c3-115">Этот почтовый ящик представляет список рассылки, который требуется развернуть.</span><span class="sxs-lookup"><span data-stu-id="ed0c3-115">This mailbox represents the distribution list to expand.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed0c3-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ed0c3-116">Parent elements</span></span>

<span data-ttu-id="ed0c3-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="ed0c3-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed0c3-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="ed0c3-118">Remarks</span></span>

<span data-ttu-id="ed0c3-119">Расширение списка рассылки будет выполняться только для одного списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="ed0c3-119">A distribution list expansion will only be performed for a single distribution list.</span></span> <span data-ttu-id="ed0c3-120">Расширение списка рассылки не является рекурсивным.</span><span class="sxs-lookup"><span data-stu-id="ed0c3-120">A distribution list expansion is not recursive.</span></span>
  
<span data-ttu-id="ed0c3-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ed0c3-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed0c3-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ed0c3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed0c3-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ed0c3-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ed0c3-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ed0c3-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ed0c3-125">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="ed0c3-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="ed0c3-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ed0c3-126">Validation File</span></span>  <br/> |<span data-ttu-id="ed0c3-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ed0c3-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ed0c3-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ed0c3-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed0c3-129">False</span><span class="sxs-lookup"><span data-stu-id="ed0c3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed0c3-130">См. также</span><span class="sxs-lookup"><span data-stu-id="ed0c3-130">See also</span></span>



[<span data-ttu-id="ed0c3-131">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="ed0c3-131">ExpandDL operation</span></span>](expanddl-operation.md)

