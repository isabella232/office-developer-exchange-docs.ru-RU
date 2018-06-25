---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: Элемент ParentItemId определяет родительский элемент, ссылки на связанные вложения.
ms.openlocfilehash: 9bd875ee5ead8b87996288a640e1bb14e3a5e8b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834703"
---
# <a name="parentitemid"></a><span data-ttu-id="d77b2-103">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="d77b2-103">ParentItemId</span></span>

<span data-ttu-id="d77b2-104">Элемент **ParentItemId** определяет родительский элемент, ссылки на связанные вложения.</span><span class="sxs-lookup"><span data-stu-id="d77b2-104">The **ParentItemId** element identifies the parent item that links to an associated attachment.</span></span> 
  
- [<span data-ttu-id="d77b2-105">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d77b2-105">CreateAttachment</span></span>](createattachment.md)
  
- [<span data-ttu-id="d77b2-106">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="d77b2-106">ParentItemId</span></span>](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

<span data-ttu-id="d77b2-107">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="d77b2-107">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d77b2-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d77b2-108">Attributes and elements</span></span>

<span data-ttu-id="d77b2-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d77b2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d77b2-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d77b2-110">Attributes</span></span>

|<span data-ttu-id="d77b2-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d77b2-111">**Attribute**</span></span>|<span data-ttu-id="d77b2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d77b2-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d77b2-113">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="d77b2-113">**Id**</span></span> <br/> |<span data-ttu-id="d77b2-114">Определяет один элемент в хранилище Exchange для связи с вложением.</span><span class="sxs-lookup"><span data-stu-id="d77b2-114">Identifies a single item in the Exchange store to associate with an attachment.</span></span> <span data-ttu-id="d77b2-115">Это значение является строкой.</span><span class="sxs-lookup"><span data-stu-id="d77b2-115">This value is a string.</span></span> <span data-ttu-id="d77b2-116">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d77b2-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d77b2-117">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d77b2-117">**ChangeKey**</span></span> <br/> |<span data-ttu-id="d77b2-118">Определяет не указан версию элемента, который идентифицируется с помощью атрибута **Id** в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d77b2-118">Identifies an unspecified version of an item that is identified by the **Id** attribute in the Exchange store.</span></span> <span data-ttu-id="d77b2-119">Здесь указывается убедитесь в том, что текущего элемента используется при обновлении с вложением.</span><span class="sxs-lookup"><span data-stu-id="d77b2-119">This is used to make sure that a current item is used when it is updated with an attachment.</span></span> <span data-ttu-id="d77b2-120">Это значение является строкой.</span><span class="sxs-lookup"><span data-stu-id="d77b2-120">This value is a string.</span></span> <span data-ttu-id="d77b2-121">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d77b2-121">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d77b2-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d77b2-122">Child elements</span></span>

<span data-ttu-id="d77b2-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="d77b2-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d77b2-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d77b2-124">Parent elements</span></span>

|<span data-ttu-id="d77b2-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d77b2-125">**Element**</span></span>|<span data-ttu-id="d77b2-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d77b2-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d77b2-127">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d77b2-127">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="d77b2-128">Определяет запрос на создание вложения в элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d77b2-128">Defines a request to create an attachment to an item in a mailbox.</span></span>  <br/> <span data-ttu-id="d77b2-129">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d77b2-129">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d77b2-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="d77b2-130">Remarks</span></span>

<span data-ttu-id="d77b2-131">Этот элемент является обязательным в [CreateAttachment операции](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d77b2-131">This element is required in the [CreateAttachment operation](createattachment-operation.md).</span></span> <span data-ttu-id="d77b2-132">Этот элемент по сути является то же, что элемент [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="d77b2-132">This element is basically the same as the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="d77b2-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d77b2-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d77b2-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d77b2-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d77b2-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d77b2-135">Namespace</span></span>  <br/> |[http://schemas.microsoft.com/exchange/services/2006/messages](http://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|<span data-ttu-id="d77b2-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d77b2-136">Schema Name</span></span>  <br/> |<span data-ttu-id="d77b2-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d77b2-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d77b2-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d77b2-138">Validation File</span></span>  <br/> |<span data-ttu-id="d77b2-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d77b2-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d77b2-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d77b2-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="d77b2-141">False</span><span class="sxs-lookup"><span data-stu-id="d77b2-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d77b2-142">См. также</span><span class="sxs-lookup"><span data-stu-id="d77b2-142">See also</span></span>

- [<span data-ttu-id="d77b2-143">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d77b2-143">CreateAttachment operation</span></span>](createattachment-operation.md)

