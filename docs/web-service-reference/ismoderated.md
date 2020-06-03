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
ms.openlocfilehash: 930d5a7e09712f35d22850a93462d051a34785a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435487"
---
# <a name="ismoderated"></a><span data-ttu-id="33875-103">Модератор</span><span class="sxs-lookup"><span data-stu-id="33875-103">IsModerated</span></span>

<span data-ttu-id="33875-104">Элемент "с **модератором** " указывает, является ли почтовый ящик получателя ведущим.</span><span class="sxs-lookup"><span data-stu-id="33875-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="33875-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="33875-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33875-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33875-106">Attributes and elements</span></span>

<span data-ttu-id="33875-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="33875-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33875-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33875-108">Attributes</span></span>

<span data-ttu-id="33875-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33875-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33875-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33875-110">Child elements</span></span>

<span data-ttu-id="33875-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33875-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33875-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33875-112">Parent elements</span></span>

|<span data-ttu-id="33875-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33875-113">**Element**</span></span>|<span data-ttu-id="33875-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33875-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33875-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="33875-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="33875-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="33875-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33875-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33875-117">Text value</span></span>

<span data-ttu-id="33875-118">Текстовое значение этого элемента имеет значение true, если для почтового ящика получателя выбрано **значение** "Модератор".</span><span class="sxs-lookup"><span data-stu-id="33875-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="33875-119">Значение **false** , если почтовый ящик получателя не является ведущим.</span><span class="sxs-lookup"><span data-stu-id="33875-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="33875-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="33875-120">Remarks</span></span>

<span data-ttu-id="33875-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="33875-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33875-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33875-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33875-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33875-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33875-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33875-124">Schema Name</span></span>  <br/> |<span data-ttu-id="33875-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="33875-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="33875-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33875-126">Validation File</span></span>  <br/> |<span data-ttu-id="33875-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="33875-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33875-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33875-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="33875-129">False</span><span class="sxs-lookup"><span data-stu-id="33875-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33875-130">См. также</span><span class="sxs-lookup"><span data-stu-id="33875-130">See also</span></span>



- [<span data-ttu-id="33875-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="33875-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

