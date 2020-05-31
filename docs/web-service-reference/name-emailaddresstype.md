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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834504"
---
# <a name="name-emailaddresstype"></a><span data-ttu-id="63ae5-103">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="63ae5-103">Name (EmailAddressType)</span></span>

<span data-ttu-id="63ae5-104">Элемент **Name** представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="63ae5-104">The **Name** element represents the name of a mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="63ae5-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="63ae5-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="63ae5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="63ae5-106">Attributes and elements</span></span>

<span data-ttu-id="63ae5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="63ae5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63ae5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="63ae5-108">Attributes</span></span>

<span data-ttu-id="63ae5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="63ae5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63ae5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="63ae5-110">Child elements</span></span>

<span data-ttu-id="63ae5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="63ae5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63ae5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="63ae5-112">Parent elements</span></span>

|<span data-ttu-id="63ae5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="63ae5-113">**Element**</span></span>|<span data-ttu-id="63ae5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="63ae5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63ae5-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="63ae5-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="63ae5-116">Определяет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="63ae5-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="63ae5-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="63ae5-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="63ae5-118">Определяет список комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="63ae5-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63ae5-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="63ae5-119">Text value</span></span>

<span data-ttu-id="63ae5-120">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="63ae5-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63ae5-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="63ae5-121">Remarks</span></span>

<span data-ttu-id="63ae5-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="63ae5-122">This element is optional.</span></span> <span data-ttu-id="63ae5-123">Элемент **Name** существует в типах **AttachmentType**, **EmailAddressType**и **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="63ae5-123">The **Name** element exists in the **AttachmentType**, **EmailAddressType**, and **EmailAddress** types.</span></span> <span data-ttu-id="63ae5-124">Элемент **Name** в типе **EmailAddress** описывается в разделе [Name (EmailAddress)](name-emailaddress.md) element.</span><span class="sxs-lookup"><span data-stu-id="63ae5-124">The **Name** element in the **EmailAddress** type is described in the [Name (EmailAddress)](name-emailaddress.md) element topic.</span></span> 
  
<span data-ttu-id="63ae5-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="63ae5-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63ae5-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="63ae5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63ae5-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="63ae5-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63ae5-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="63ae5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="63ae5-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="63ae5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="63ae5-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="63ae5-130">Validation File</span></span>  <br/> |<span data-ttu-id="63ae5-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="63ae5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63ae5-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="63ae5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="63ae5-133">False</span><span class="sxs-lookup"><span data-stu-id="63ae5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63ae5-134">См. также</span><span class="sxs-lookup"><span data-stu-id="63ae5-134">See also</span></span>

- [<span data-ttu-id="63ae5-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="63ae5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

