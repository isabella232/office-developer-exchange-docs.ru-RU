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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466929"
---
# <a name="name-emailaddresstype"></a><span data-ttu-id="7a505-103">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7a505-103">Name (EmailAddressType)</span></span>

<span data-ttu-id="7a505-104">Элемент **Name** представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7a505-104">The **Name** element represents the name of a mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="7a505-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="7a505-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7a505-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7a505-106">Attributes and elements</span></span>

<span data-ttu-id="7a505-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7a505-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a505-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7a505-108">Attributes</span></span>

<span data-ttu-id="7a505-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7a505-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a505-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7a505-110">Child elements</span></span>

<span data-ttu-id="7a505-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7a505-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a505-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7a505-112">Parent elements</span></span>

|<span data-ttu-id="7a505-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a505-113">**Element**</span></span>|<span data-ttu-id="7a505-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a505-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a505-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="7a505-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="7a505-116">Определяет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7a505-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="7a505-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="7a505-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="7a505-118">Определяет список комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="7a505-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a505-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7a505-119">Text value</span></span>

<span data-ttu-id="7a505-120">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="7a505-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a505-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="7a505-121">Remarks</span></span>

<span data-ttu-id="7a505-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7a505-122">This element is optional.</span></span> <span data-ttu-id="7a505-123">Элемент **Name** существует в типах **AttachmentType**, **EmailAddressType**и **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="7a505-123">The **Name** element exists in the **AttachmentType**, **EmailAddressType**, and **EmailAddress** types.</span></span> <span data-ttu-id="7a505-124">Элемент **Name** в типе **EmailAddress** описывается в разделе [Name (EmailAddress)](name-emailaddress.md) element.</span><span class="sxs-lookup"><span data-stu-id="7a505-124">The **Name** element in the **EmailAddress** type is described in the [Name (EmailAddress)](name-emailaddress.md) element topic.</span></span> 
  
<span data-ttu-id="7a505-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a505-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a505-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7a505-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a505-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7a505-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a505-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7a505-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7a505-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7a505-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a505-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7a505-130">Validation File</span></span>  <br/> |<span data-ttu-id="7a505-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7a505-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a505-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7a505-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a505-133">False</span><span class="sxs-lookup"><span data-stu-id="7a505-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a505-134">См. также</span><span class="sxs-lookup"><span data-stu-id="7a505-134">See also</span></span>

- [<span data-ttu-id="7a505-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7a505-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

