---
title: MailboxFull
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxFull
api_type:
- schema
ms.assetid: 38b28c9b-9da2-4d6a-9cda-9c393986575b
description: Элемент MailboxFull указывает, является ли полный почтовый ящик получателя.
ms.openlocfilehash: 8e2c9e01b93af03e875834724a942cd9b17a73f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834286"
---
# <a name="mailboxfull"></a><span data-ttu-id="4d225-103">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="4d225-103">MailboxFull</span></span>

<span data-ttu-id="4d225-104">Элемент **MailboxFull** указывает, является ли полный почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="4d225-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="4d225-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4d225-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4d225-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4d225-106">Attributes and elements</span></span>

<span data-ttu-id="4d225-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4d225-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d225-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4d225-108">Attributes</span></span>

<span data-ttu-id="4d225-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4d225-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d225-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4d225-110">Child elements</span></span>

<span data-ttu-id="4d225-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="4d225-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d225-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4d225-112">Parent elements</span></span>

|<span data-ttu-id="4d225-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d225-113">**Element**</span></span>|<span data-ttu-id="4d225-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d225-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d225-115">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="4d225-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="4d225-116">Представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="4d225-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4d225-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4d225-117">Text value</span></span>

<span data-ttu-id="4d225-118">Этот элемент может быть значение **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="4d225-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="4d225-119">Значение **true** указывает, что почтовый ящик достиг ее объем; значение **false** указывает, что она не используются все ресурсы.</span><span class="sxs-lookup"><span data-stu-id="4d225-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4d225-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="4d225-120">Remarks</span></span>

<span data-ttu-id="4d225-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d225-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d225-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4d225-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d225-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4d225-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d225-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4d225-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4d225-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4d225-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d225-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4d225-126">Validation File</span></span>  <br/> |<span data-ttu-id="4d225-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4d225-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d225-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4d225-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d225-129">False</span><span class="sxs-lookup"><span data-stu-id="4d225-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d225-130">См. также</span><span class="sxs-lookup"><span data-stu-id="4d225-130">See also</span></span>

- [<span data-ttu-id="4d225-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4d225-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

