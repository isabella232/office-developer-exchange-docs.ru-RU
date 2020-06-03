---
title: DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 42d2a888-fa62-4970-8306-9ddde4eeb1f0
description: Элемент DisableApp указывает запрос на отключение приложения.
ms.openlocfilehash: e99464677dc34e011e45548083fb830b819649fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457825"
---
# <a name="disableapp"></a><span data-ttu-id="c9886-103">DisableApp</span><span class="sxs-lookup"><span data-stu-id="c9886-103">DisableApp</span></span>

<span data-ttu-id="c9886-104">Элемент **DisableApp** указывает запрос на отключение приложения.</span><span class="sxs-lookup"><span data-stu-id="c9886-104">The **DisableApp** element specifies a request to disable an app.</span></span> 
  
```XML
<DisableApp>
    <ID></ID>
    <DisableReason></DisableReason>
</DisableApp>
```

 <span data-ttu-id="c9886-105">**дисаблеапптипе**</span><span class="sxs-lookup"><span data-stu-id="c9886-105">**DisableAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9886-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c9886-106">Attributes and elements</span></span>

<span data-ttu-id="c9886-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c9886-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9886-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c9886-108">Attributes</span></span>

<span data-ttu-id="c9886-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c9886-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9886-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c9886-110">Child elements</span></span>

|<span data-ttu-id="c9886-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9886-111">**Element**</span></span>|<span data-ttu-id="c9886-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9886-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9886-113">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="c9886-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="c9886-114">Указывает идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="c9886-114">Specifies the identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="c9886-115">дисаблереасон</span><span class="sxs-lookup"><span data-stu-id="c9886-115">DisableReason</span></span>](disablereason.md) <br/> |<span data-ttu-id="c9886-116">Указывает причину отключения приложения.</span><span class="sxs-lookup"><span data-stu-id="c9886-116">Specifies the reason for disabling an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9886-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c9886-117">Parent elements</span></span>

<span data-ttu-id="c9886-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9886-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c9886-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="c9886-119">Remarks</span></span>

<span data-ttu-id="c9886-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c9886-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c9886-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9886-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9886-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c9886-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9886-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c9886-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c9886-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c9886-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c9886-125">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="c9886-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="c9886-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c9886-126">Validation File</span></span>  <br/> |<span data-ttu-id="c9886-127">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c9886-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9886-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c9886-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c9886-129">См. также</span><span class="sxs-lookup"><span data-stu-id="c9886-129">See also</span></span>

- [<span data-ttu-id="c9886-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c9886-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

