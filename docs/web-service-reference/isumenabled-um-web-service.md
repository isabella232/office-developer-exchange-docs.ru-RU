---
title: IsUMEnabled (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: Элемент IsUMEnabled указывает, включен ли для почтового ящика единая система обмена сообщениями.
ms.openlocfilehash: 5f4d59c5497158e5afbc8bb5db4900bd129df50b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834113"
---
# <a name="isumenabled-um-web-service"></a><span data-ttu-id="f2dc9-103">IsUMEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f2dc9-103">IsUMEnabled (UM web service)</span></span>

<span data-ttu-id="f2dc9-104">Элемент **IsUMEnabled** указывает, включен ли для почтового ящика единая система обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-104">The **IsUMEnabled** element indicates whether a mailbox is enabled for Unified Messaging.</span></span> 
  
```xml
<IsUMEnabled/>
```

 <span data-ttu-id="f2dc9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f2dc9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2dc9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f2dc9-106">Attributes and elements</span></span>

<span data-ttu-id="f2dc9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2dc9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f2dc9-108">Attributes</span></span>

<span data-ttu-id="f2dc9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2dc9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f2dc9-110">Child elements</span></span>

<span data-ttu-id="f2dc9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2dc9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f2dc9-112">Parent elements</span></span>

<span data-ttu-id="f2dc9-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-113">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f2dc9-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f2dc9-114">Text value</span></span>

<span data-ttu-id="f2dc9-115">Если этот элемент включен, необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-115">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="f2dc9-116">Значение **true** указывает на то, что для почтового ящика включена поддержка единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-116">A value of **true** indicates that the mailbox is enabled for Unified Messaging.</span></span> <span data-ttu-id="f2dc9-117">Значение **false** означает, что для почтового ящика не включена поддержка единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="f2dc9-117">A value of **false** means that the mailbox is not enabled for Unified Messaging.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f2dc9-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="f2dc9-118">Remarks</span></span>

<span data-ttu-id="f2dc9-119">Чтобы определить, включен ли для почтового ящика единая система обмена сообщениями, используйте [операцию IsUMEnabled (веб-служба единой системы обмена](isumenabled-operation-um-web-service.md)сообщениями).</span><span class="sxs-lookup"><span data-stu-id="f2dc9-119">To determine whether a mailbox is enabled for Unified Messaging, use the [IsUMEnabled operation (UM web service)](isumenabled-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2dc9-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f2dc9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2dc9-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f2dc9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f2dc9-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f2dc9-122">Schema Name</span></span>  <br/> |<span data-ttu-id="f2dc9-123">Сообщения</span><span class="sxs-lookup"><span data-stu-id="f2dc9-123">Messages</span></span>  <br/> |
|<span data-ttu-id="f2dc9-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f2dc9-124">Validation File</span></span>  <br/> |<span data-ttu-id="f2dc9-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f2dc9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f2dc9-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f2dc9-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2dc9-127">False</span><span class="sxs-lookup"><span data-stu-id="f2dc9-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2dc9-128">См. также</span><span class="sxs-lookup"><span data-stu-id="f2dc9-128">See also</span></span>



[<span data-ttu-id="f2dc9-129">Операция IsUMEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f2dc9-129">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)


[<span data-ttu-id="f2dc9-130">XML-элементы веб-службы единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="f2dc9-130">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

