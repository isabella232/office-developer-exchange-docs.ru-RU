---
title: парентитемид
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
description: Элемент Парентитемид определяет родительский элемент, ссылающийся на связанное вложение.
ms.openlocfilehash: 9bd875ee5ead8b87996288a640e1bb14e3a5e8b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834703"
---
# <a name="parentitemid"></a><span data-ttu-id="bba77-103">парентитемид</span><span class="sxs-lookup"><span data-stu-id="bba77-103">ParentItemId</span></span>

<span data-ttu-id="bba77-104">Элемент **парентитемид** определяет родительский элемент, ссылающийся на связанное вложение.</span><span class="sxs-lookup"><span data-stu-id="bba77-104">The **ParentItemId** element identifies the parent item that links to an associated attachment.</span></span> 
  
- [<span data-ttu-id="bba77-105">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="bba77-105">CreateAttachment</span></span>](createattachment.md)
  
- [<span data-ttu-id="bba77-106">парентитемид</span><span class="sxs-lookup"><span data-stu-id="bba77-106">ParentItemId</span></span>](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

<span data-ttu-id="bba77-107">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="bba77-107">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bba77-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bba77-108">Attributes and elements</span></span>

<span data-ttu-id="bba77-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bba77-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bba77-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bba77-110">Attributes</span></span>

|<span data-ttu-id="bba77-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bba77-111">**Attribute**</span></span>|<span data-ttu-id="bba77-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba77-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bba77-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="bba77-113">**Id**</span></span> <br/> |<span data-ttu-id="bba77-114">Определяет один элемент в хранилище Exchange, связываемый с вложением.</span><span class="sxs-lookup"><span data-stu-id="bba77-114">Identifies a single item in the Exchange store to associate with an attachment.</span></span> <span data-ttu-id="bba77-115">Это значение является строкой.</span><span class="sxs-lookup"><span data-stu-id="bba77-115">This value is a string.</span></span> <span data-ttu-id="bba77-116">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bba77-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="bba77-117">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="bba77-117">**ChangeKey**</span></span> <br/> |<span data-ttu-id="bba77-118">Определяет неопределенную версию элемента, определяемого атрибутом **ID** в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bba77-118">Identifies an unspecified version of an item that is identified by the **Id** attribute in the Exchange store.</span></span> <span data-ttu-id="bba77-119">Это используется, чтобы убедиться, что текущий элемент используется при обновлении с вложением.</span><span class="sxs-lookup"><span data-stu-id="bba77-119">This is used to make sure that a current item is used when it is updated with an attachment.</span></span> <span data-ttu-id="bba77-120">Это значение является строкой.</span><span class="sxs-lookup"><span data-stu-id="bba77-120">This value is a string.</span></span> <span data-ttu-id="bba77-121">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bba77-121">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bba77-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bba77-122">Child elements</span></span>

<span data-ttu-id="bba77-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="bba77-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bba77-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bba77-124">Parent elements</span></span>

|<span data-ttu-id="bba77-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bba77-125">**Element**</span></span>|<span data-ttu-id="bba77-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba77-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bba77-127">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="bba77-127">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="bba77-128">Определяет запрос на создание вложения для элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bba77-128">Defines a request to create an attachment to an item in a mailbox.</span></span>  <br/> <span data-ttu-id="bba77-129">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="bba77-129">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bba77-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="bba77-130">Remarks</span></span>

<span data-ttu-id="bba77-131">Этот элемент является обязательным в [операции CreateAttachment](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bba77-131">This element is required in the [CreateAttachment operation](createattachment-operation.md).</span></span> <span data-ttu-id="bba77-132">Этот элемент в основном совпадает с элементом [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="bba77-132">This element is basically the same as the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="bba77-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bba77-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bba77-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bba77-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bba77-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bba77-135">Namespace</span></span>  <br/> |[http://schemas.microsoft.com/exchange/services/2006/messages](http://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|<span data-ttu-id="bba77-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bba77-136">Schema Name</span></span>  <br/> |<span data-ttu-id="bba77-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bba77-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bba77-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bba77-138">Validation File</span></span>  <br/> |<span data-ttu-id="bba77-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bba77-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bba77-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bba77-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="bba77-141">False</span><span class="sxs-lookup"><span data-stu-id="bba77-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bba77-142">См. также</span><span class="sxs-lookup"><span data-stu-id="bba77-142">See also</span></span>

- [<span data-ttu-id="bba77-143">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="bba77-143">CreateAttachment operation</span></span>](createattachment-operation.md)

