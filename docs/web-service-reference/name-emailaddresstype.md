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
ms.openlocfilehash: db6eb547b5c848dc31bbaa377692989b16771673
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466929"
---
# <a name="name-emailaddresstype"></a><span data-ttu-id="e5cfa-103">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e5cfa-103">Name (EmailAddressType)</span></span>

<span data-ttu-id="e5cfa-104">Элемент **Name** представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-104">The **Name** element represents the name of a mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="e5cfa-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="e5cfa-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e5cfa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e5cfa-106">Attributes and elements</span></span>

<span data-ttu-id="e5cfa-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5cfa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e5cfa-108">Attributes</span></span>

<span data-ttu-id="e5cfa-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5cfa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e5cfa-110">Child elements</span></span>

<span data-ttu-id="e5cfa-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e5cfa-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e5cfa-112">Parent elements</span></span>

|<span data-ttu-id="e5cfa-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5cfa-113">**Element**</span></span>|<span data-ttu-id="e5cfa-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5cfa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5cfa-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="e5cfa-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e5cfa-116">Определяет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="e5cfa-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="e5cfa-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="e5cfa-118">Определяет список комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5cfa-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e5cfa-119">Text value</span></span>

<span data-ttu-id="e5cfa-120">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e5cfa-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="e5cfa-121">Remarks</span></span>

<span data-ttu-id="e5cfa-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-122">This element is optional.</span></span> <span data-ttu-id="e5cfa-123">Элемент **Name** существует в типах **AttachmentType**, **EmailAddressType**и **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="e5cfa-123">The **Name** element exists in the **AttachmentType**, **EmailAddressType**, and **EmailAddress** types.</span></span> <span data-ttu-id="e5cfa-124">Элемент **Name** в типе **EmailAddress** описывается в разделе [Name (EmailAddress)](name-emailaddress.md) element.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-124">The **Name** element in the **EmailAddress** type is described in the [Name (EmailAddress)](name-emailaddress.md) element topic.</span></span> 
  
<span data-ttu-id="e5cfa-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5cfa-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5cfa-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e5cfa-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5cfa-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e5cfa-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5cfa-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e5cfa-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e5cfa-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e5cfa-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="e5cfa-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e5cfa-130">Validation File</span></span>  <br/> |<span data-ttu-id="e5cfa-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e5cfa-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5cfa-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e5cfa-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5cfa-133">False</span><span class="sxs-lookup"><span data-stu-id="e5cfa-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5cfa-134">См. также</span><span class="sxs-lookup"><span data-stu-id="e5cfa-134">See also</span></span>

- [<span data-ttu-id="e5cfa-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e5cfa-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

