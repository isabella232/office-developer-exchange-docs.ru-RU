---
title: Дети
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Children
api_type:
- schema
ms.assetid: ceaffddd-f9bc-43ea-b348-a20fdade738f
description: Дочерний элемент содержит имена потомков контакта.
ms.openlocfilehash: de398c93590a4a9ae93b6aa46994c9295d051b84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460227"
---
# <a name="children"></a><span data-ttu-id="1372a-103">Дети</span><span class="sxs-lookup"><span data-stu-id="1372a-103">Children</span></span>

<span data-ttu-id="1372a-104">**Дочерний** элемент содержит имена потомков контакта.</span><span class="sxs-lookup"><span data-stu-id="1372a-104">The **Children** element contains the names of a contact's children.</span></span> 
  
```xml
<Children>
   <String/>
</Children>
```

 <span data-ttu-id="1372a-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="1372a-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1372a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1372a-106">Attributes and elements</span></span>

<span data-ttu-id="1372a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1372a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1372a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1372a-108">Attributes</span></span>

<span data-ttu-id="1372a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1372a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1372a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1372a-110">Child elements</span></span>

|<span data-ttu-id="1372a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1372a-111">**Element**</span></span>|<span data-ttu-id="1372a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1372a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1372a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1372a-113">String</span></span>](string.md) <br/> |<span data-ttu-id="1372a-114">Содержит имя ребенка контакта.</span><span class="sxs-lookup"><span data-stu-id="1372a-114">Contains the name of a contact's child.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1372a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1372a-115">Parent elements</span></span>

|<span data-ttu-id="1372a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1372a-116">**Element**</span></span>|<span data-ttu-id="1372a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1372a-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1372a-118">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="1372a-118">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="1372a-119">Представляет контакт в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="1372a-119">Represents a contact in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1372a-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="1372a-120">Remarks</span></span>

<span data-ttu-id="1372a-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1372a-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1372a-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1372a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1372a-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1372a-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1372a-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1372a-124">Schema name</span></span>  <br/> |<span data-ttu-id="1372a-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1372a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1372a-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1372a-126">Validation file</span></span>  <br/> |<span data-ttu-id="1372a-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1372a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1372a-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1372a-128">Can be empty</span></span>  <br/> |<span data-ttu-id="1372a-129">False</span><span class="sxs-lookup"><span data-stu-id="1372a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1372a-130">См. также</span><span class="sxs-lookup"><span data-stu-id="1372a-130">See also</span></span>



- [<span data-ttu-id="1372a-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1372a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

