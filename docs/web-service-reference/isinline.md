---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: Элемент IsInline указывает, отображается ли вложение встроенным в элементе.
ms.openlocfilehash: 2b3b6392fe8867ae9782dcb7211c17f4f4d9becd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464212"
---
# <a name="isinline"></a><span data-ttu-id="61c26-103">IsInline</span><span class="sxs-lookup"><span data-stu-id="61c26-103">IsInline</span></span>

<span data-ttu-id="61c26-104">Элемент **IsInline** указывает, отображается ли вложение встроенным в элементе.</span><span class="sxs-lookup"><span data-stu-id="61c26-104">The **IsInline** element represents whether the attachment appears inline within an item.</span></span> 
  
```xml
<IsInline>true or false</IsInline>
```

 <span data-ttu-id="61c26-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="61c26-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61c26-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="61c26-106">Attributes and elements</span></span>

<span data-ttu-id="61c26-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="61c26-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61c26-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="61c26-108">Attributes</span></span>

<span data-ttu-id="61c26-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="61c26-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61c26-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="61c26-110">Child elements</span></span>

<span data-ttu-id="61c26-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="61c26-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61c26-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="61c26-112">Parent elements</span></span>

|<span data-ttu-id="61c26-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="61c26-113">**Element**</span></span>|<span data-ttu-id="61c26-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="61c26-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61c26-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="61c26-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="61c26-116">Представляет файл, присоединенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="61c26-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="61c26-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="61c26-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="61c26-118">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="61c26-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61c26-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="61c26-119">Text value</span></span>

<span data-ttu-id="61c26-120">Этот элемент может иметь **значение true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="61c26-120">This element can be either **true** or **false**.</span></span> <span data-ttu-id="61c26-121">Значение по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="61c26-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="61c26-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="61c26-122">Remarks</span></span>

<span data-ttu-id="61c26-123">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="61c26-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61c26-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="61c26-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61c26-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="61c26-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61c26-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="61c26-126">Schema Name</span></span>  <br/> |<span data-ttu-id="61c26-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="61c26-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="61c26-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="61c26-128">Validation File</span></span>  <br/> |<span data-ttu-id="61c26-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="61c26-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61c26-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="61c26-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="61c26-131">False</span><span class="sxs-lookup"><span data-stu-id="61c26-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61c26-132">См. также</span><span class="sxs-lookup"><span data-stu-id="61c26-132">See also</span></span>



- [<span data-ttu-id="61c26-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="61c26-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

