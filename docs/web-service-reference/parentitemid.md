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
ms.openlocfilehash: 4f3e33da0af2438948313f0e335cd03e076d135a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465746"
---
# <a name="parentitemid"></a><span data-ttu-id="d968d-103">парентитемид</span><span class="sxs-lookup"><span data-stu-id="d968d-103">ParentItemId</span></span>

<span data-ttu-id="d968d-104">Элемент **парентитемид** определяет родительский элемент, ссылающийся на связанное вложение.</span><span class="sxs-lookup"><span data-stu-id="d968d-104">The **ParentItemId** element identifies the parent item that links to an associated attachment.</span></span> 
  
- [<span data-ttu-id="d968d-105">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d968d-105">CreateAttachment</span></span>](createattachment.md)
  
- [<span data-ttu-id="d968d-106">парентитемид</span><span class="sxs-lookup"><span data-stu-id="d968d-106">ParentItemId</span></span>](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

<span data-ttu-id="d968d-107">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="d968d-107">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d968d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d968d-108">Attributes and elements</span></span>

<span data-ttu-id="d968d-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d968d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d968d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d968d-110">Attributes</span></span>

|<span data-ttu-id="d968d-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d968d-111">**Attribute**</span></span>|<span data-ttu-id="d968d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d968d-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d968d-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="d968d-113">**Id**</span></span> <br/> |<span data-ttu-id="d968d-114">Определяет один элемент в хранилище Exchange, связываемый с вложением.</span><span class="sxs-lookup"><span data-stu-id="d968d-114">Identifies a single item in the Exchange store to associate with an attachment.</span></span> <span data-ttu-id="d968d-115">Это значение является строкой.</span><span class="sxs-lookup"><span data-stu-id="d968d-115">This value is a string.</span></span> <span data-ttu-id="d968d-116">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d968d-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d968d-117">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="d968d-117">**ChangeKey**</span></span> <br/> |<span data-ttu-id="d968d-118">Определяет неопределенную версию элемента, определяемого атрибутом **ID** в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d968d-118">Identifies an unspecified version of an item that is identified by the **Id** attribute in the Exchange store.</span></span> <span data-ttu-id="d968d-119">Это используется, чтобы убедиться, что текущий элемент используется при обновлении с вложением.</span><span class="sxs-lookup"><span data-stu-id="d968d-119">This is used to make sure that a current item is used when it is updated with an attachment.</span></span> <span data-ttu-id="d968d-120">Это значение является строкой.</span><span class="sxs-lookup"><span data-stu-id="d968d-120">This value is a string.</span></span> <span data-ttu-id="d968d-121">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d968d-121">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d968d-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d968d-122">Child elements</span></span>

<span data-ttu-id="d968d-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d968d-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d968d-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d968d-124">Parent elements</span></span>

|<span data-ttu-id="d968d-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d968d-125">**Element**</span></span>|<span data-ttu-id="d968d-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d968d-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d968d-127">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d968d-127">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="d968d-128">Определяет запрос на создание вложения для элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d968d-128">Defines a request to create an attachment to an item in a mailbox.</span></span>  <br/> <span data-ttu-id="d968d-129">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d968d-129">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d968d-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="d968d-130">Remarks</span></span>

<span data-ttu-id="d968d-131">Этот элемент является обязательным в [операции CreateAttachment](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d968d-131">This element is required in the [CreateAttachment operation](createattachment-operation.md).</span></span> <span data-ttu-id="d968d-132">Этот элемент в основном совпадает с элементом [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="d968d-132">This element is basically the same as the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="d968d-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d968d-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d968d-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d968d-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d968d-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d968d-135">Namespace</span></span>  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|<span data-ttu-id="d968d-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d968d-136">Schema Name</span></span>  <br/> |<span data-ttu-id="d968d-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d968d-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d968d-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d968d-138">Validation File</span></span>  <br/> |<span data-ttu-id="d968d-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d968d-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d968d-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d968d-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="d968d-141">False</span><span class="sxs-lookup"><span data-stu-id="d968d-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d968d-142">См. также</span><span class="sxs-lookup"><span data-stu-id="d968d-142">See also</span></span>

- [<span data-ttu-id="d968d-143">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d968d-143">CreateAttachment operation</span></span>](createattachment-operation.md)

