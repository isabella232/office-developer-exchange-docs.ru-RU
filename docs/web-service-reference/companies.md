---
title: Компании
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Companies
api_type:
- schema
ms.assetid: 5d9ea76f-e14d-4424-8842-0c3cc3305119
description: Элемент "компании" представляет коллекцию компаний, связанных с контактом или задачей.
ms.openlocfilehash: eda2b92f3ca874aeeceef6a0935a49a98af0ec39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461452"
---
# <a name="companies"></a><span data-ttu-id="e81e8-103">Компании</span><span class="sxs-lookup"><span data-stu-id="e81e8-103">Companies</span></span>

<span data-ttu-id="e81e8-104">Элемент " **компании** " представляет коллекцию компаний, связанных с контактом или задачей.</span><span class="sxs-lookup"><span data-stu-id="e81e8-104">The **Companies** element represents the collection of companies that are associated with a contact or task.</span></span> 
  
```xml
<Companies>
   <String/>
</Companies>
```

 <span data-ttu-id="e81e8-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="e81e8-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e81e8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e81e8-106">Attributes and elements</span></span>

<span data-ttu-id="e81e8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e81e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e81e8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e81e8-108">Attributes</span></span>

<span data-ttu-id="e81e8-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e81e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e81e8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e81e8-110">Child elements</span></span>

|<span data-ttu-id="e81e8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e81e8-111">**Element**</span></span>|<span data-ttu-id="e81e8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e81e8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e81e8-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e81e8-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e81e8-114">Представляет название компании.</span><span class="sxs-lookup"><span data-stu-id="e81e8-114">Represents the name of a company.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e81e8-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e81e8-115">Parent elements</span></span>

|<span data-ttu-id="e81e8-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e81e8-116">**Element**</span></span>|<span data-ttu-id="e81e8-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e81e8-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e81e8-118">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="e81e8-118">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="e81e8-119">Представляет контакт в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e81e8-119">Represents a contact in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e81e8-120">Задача</span><span class="sxs-lookup"><span data-stu-id="e81e8-120">Task</span></span>](task.md) <br/> |<span data-ttu-id="e81e8-121">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e81e8-121">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e81e8-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="e81e8-122">Remarks</span></span>

<span data-ttu-id="e81e8-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e81e8-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e81e8-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e81e8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e81e8-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e81e8-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e81e8-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e81e8-126">Schema name</span></span>  <br/> |<span data-ttu-id="e81e8-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e81e8-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e81e8-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e81e8-128">Validation file</span></span>  <br/> |<span data-ttu-id="e81e8-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e81e8-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e81e8-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e81e8-130">Can be empty</span></span>  <br/> |<span data-ttu-id="e81e8-131">False</span><span class="sxs-lookup"><span data-stu-id="e81e8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e81e8-132">См. также</span><span class="sxs-lookup"><span data-stu-id="e81e8-132">See also</span></span>



- [<span data-ttu-id="e81e8-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e81e8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

