---
title: Имя (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: 98c58c53-9acc-4e89-9fcf-03f1b05abee1
description: Элемент Name представляет имя пользователя почтового ящика.
ms.openlocfilehash: b140fd46608a04f9aaba17f917cc4171c056dcf2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834504"
---
# <a name="name-emailaddresstype"></a><span data-ttu-id="bbda2-103">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="bbda2-103">Name (EmailAddressType)</span></span>

<span data-ttu-id="bbda2-104">Элемент **Name** представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bbda2-104">The **Name** element represents the name of a mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="bbda2-105">**string**</span><span class="sxs-lookup"><span data-stu-id="bbda2-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bbda2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bbda2-106">Attributes and elements</span></span>

<span data-ttu-id="bbda2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bbda2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bbda2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bbda2-108">Attributes</span></span>

<span data-ttu-id="bbda2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bbda2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bbda2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bbda2-110">Child elements</span></span>

<span data-ttu-id="bbda2-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bbda2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bbda2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bbda2-112">Parent elements</span></span>

|<span data-ttu-id="bbda2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bbda2-113">**Element**</span></span>|<span data-ttu-id="bbda2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bbda2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbda2-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="bbda2-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="bbda2-116">Определяет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="bbda2-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="bbda2-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="bbda2-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="bbda2-118">Определяет список конференц-залы.</span><span class="sxs-lookup"><span data-stu-id="bbda2-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bbda2-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bbda2-119">Text value</span></span>

<span data-ttu-id="bbda2-120">Текстовое значение, представляющее строку является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="bbda2-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bbda2-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="bbda2-121">Remarks</span></span>

<span data-ttu-id="bbda2-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bbda2-122">This element is optional.</span></span> <span data-ttu-id="bbda2-123">Элемент **Name** существует в типах **AttachmentType**, **EmailAddressType**и **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="bbda2-123">The **Name** element exists in the **AttachmentType**, **EmailAddressType**, and **EmailAddress** types.</span></span> <span data-ttu-id="bbda2-124">Элемент **имя** типа **EmailAddress** описан в разделе элемент [имя (EmailAddress)](name-emailaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="bbda2-124">The **Name** element in the **EmailAddress** type is described in the [Name (EmailAddress)](name-emailaddress.md) element topic.</span></span> 
  
<span data-ttu-id="bbda2-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bbda2-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bbda2-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bbda2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bbda2-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bbda2-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bbda2-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bbda2-128">Schema Name</span></span>  <br/> |<span data-ttu-id="bbda2-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bbda2-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="bbda2-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bbda2-130">Validation File</span></span>  <br/> |<span data-ttu-id="bbda2-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bbda2-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bbda2-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bbda2-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="bbda2-133">False</span><span class="sxs-lookup"><span data-stu-id="bbda2-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bbda2-134">См. также</span><span class="sxs-lookup"><span data-stu-id="bbda2-134">See also</span></span>

- [<span data-ttu-id="bbda2-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bbda2-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

