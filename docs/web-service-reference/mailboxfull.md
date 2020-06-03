---
title: маилбоксфулл
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
description: Элемент Маилбоксфулл указывает, заполнен ли почтовый ящик получателя.
ms.openlocfilehash: f336f1eda122bb170aafb22a028e3faf84f4d782
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465977"
---
# <a name="mailboxfull"></a><span data-ttu-id="bfe27-103">маилбоксфулл</span><span class="sxs-lookup"><span data-stu-id="bfe27-103">MailboxFull</span></span>

<span data-ttu-id="bfe27-104">Элемент **маилбоксфулл** указывает, заполнен ли почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="bfe27-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="bfe27-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bfe27-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bfe27-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bfe27-106">Attributes and elements</span></span>

<span data-ttu-id="bfe27-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bfe27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfe27-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bfe27-108">Attributes</span></span>

<span data-ttu-id="bfe27-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bfe27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bfe27-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bfe27-110">Child elements</span></span>

<span data-ttu-id="bfe27-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bfe27-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bfe27-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bfe27-112">Parent elements</span></span>

|<span data-ttu-id="bfe27-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bfe27-113">**Element**</span></span>|<span data-ttu-id="bfe27-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bfe27-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfe27-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="bfe27-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="bfe27-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bfe27-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bfe27-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bfe27-117">Text value</span></span>

<span data-ttu-id="bfe27-118">Этот элемент может иметь **значение true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="bfe27-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="bfe27-119">Значение **true** указывает, что размер почтового ящика достиг емкости; значение **false** указывает на то, что емкость не достигнута.</span><span class="sxs-lookup"><span data-stu-id="bfe27-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bfe27-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="bfe27-120">Remarks</span></span>

<span data-ttu-id="bfe27-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bfe27-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfe27-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bfe27-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfe27-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bfe27-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bfe27-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bfe27-124">Schema Name</span></span>  <br/> |<span data-ttu-id="bfe27-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bfe27-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="bfe27-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bfe27-126">Validation File</span></span>  <br/> |<span data-ttu-id="bfe27-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bfe27-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bfe27-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bfe27-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="bfe27-129">False</span><span class="sxs-lookup"><span data-stu-id="bfe27-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bfe27-130">См. также</span><span class="sxs-lookup"><span data-stu-id="bfe27-130">See also</span></span>

- [<span data-ttu-id="bfe27-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bfe27-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

