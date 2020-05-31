---
title: Модератор
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsModerated
api_type:
- schema
ms.assetid: a7562256-feb9-41a1-857e-b5d41cbed680
description: Элемент "с модератором" указывает, является ли почтовый ящик получателя ведущим.
ms.openlocfilehash: 8db234f9706bb8187978a76f745323749d7a640a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834055"
---
# <a name="ismoderated"></a><span data-ttu-id="a1de4-103">Модератор</span><span class="sxs-lookup"><span data-stu-id="a1de4-103">IsModerated</span></span>

<span data-ttu-id="a1de4-104">Элемент "с **модератором** " указывает, является ли почтовый ящик получателя ведущим.</span><span class="sxs-lookup"><span data-stu-id="a1de4-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="a1de4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a1de4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1de4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a1de4-106">Attributes and elements</span></span>

<span data-ttu-id="a1de4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a1de4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1de4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a1de4-108">Attributes</span></span>

<span data-ttu-id="a1de4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a1de4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1de4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a1de4-110">Child elements</span></span>

<span data-ttu-id="a1de4-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a1de4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a1de4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a1de4-112">Parent elements</span></span>

|<span data-ttu-id="a1de4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1de4-113">**Element**</span></span>|<span data-ttu-id="a1de4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1de4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1de4-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="a1de4-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="a1de4-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a1de4-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a1de4-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a1de4-117">Text value</span></span>

<span data-ttu-id="a1de4-118">Текстовое значение этого элемента имеет значение true, если для почтового ящика получателя выбрано **значение** "Модератор".</span><span class="sxs-lookup"><span data-stu-id="a1de4-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="a1de4-119">Значение **false** , если почтовый ящик получателя не является ведущим.</span><span class="sxs-lookup"><span data-stu-id="a1de4-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a1de4-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="a1de4-120">Remarks</span></span>

<span data-ttu-id="a1de4-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1de4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1de4-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a1de4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1de4-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a1de4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1de4-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a1de4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a1de4-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a1de4-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1de4-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a1de4-126">Validation File</span></span>  <br/> |<span data-ttu-id="a1de4-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a1de4-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1de4-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a1de4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1de4-129">False</span><span class="sxs-lookup"><span data-stu-id="a1de4-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1de4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="a1de4-130">See also</span></span>



- [<span data-ttu-id="a1de4-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a1de4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

