---
title: Контакты
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contacts
api_type:
- schema
ms.assetid: 0cc67cdf-9707-45e7-92c6-fa83a016cdbe
description: Элемент Contacts содержит список контактов, связанных с задачей.
ms.openlocfilehash: da7963d30f58f7da52e76e3f7f1d0f7fd68abf74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761730"
---
# <a name="contacts"></a><span data-ttu-id="7ffa0-103">Контакты</span><span class="sxs-lookup"><span data-stu-id="7ffa0-103">Contacts</span></span>

<span data-ttu-id="7ffa0-104">Элемент **Contacts** содержит список контактов, связанных с задачей.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-104">The **Contacts** element contains a list of contacts that are associated with a task.</span></span> 
  
```xml
<Contacts>
   <String/>
</Contacts>
```

 <span data-ttu-id="7ffa0-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ffa0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7ffa0-106">Attributes and elements</span></span>

<span data-ttu-id="7ffa0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ffa0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7ffa0-108">Attributes</span></span>

<span data-ttu-id="7ffa0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ffa0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7ffa0-110">Child elements</span></span>

|<span data-ttu-id="7ffa0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-111">**Element**</span></span>|<span data-ttu-id="7ffa0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ffa0-113">Строка</span><span class="sxs-lookup"><span data-stu-id="7ffa0-113">String</span></span>](string.md) <br/> |<span data-ttu-id="7ffa0-114">Представляет разделенный запятыми список имен контактов.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-114">Represents a comma-separated list of contact names.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ffa0-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7ffa0-115">Parent elements</span></span>

|<span data-ttu-id="7ffa0-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-116">**Element**</span></span>|<span data-ttu-id="7ffa0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ffa0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ffa0-118">Задача</span><span class="sxs-lookup"><span data-stu-id="7ffa0-118">Task</span></span>](task.md) <br/> |<span data-ttu-id="7ffa0-119">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-119">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ffa0-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="7ffa0-120">Remarks</span></span>

<span data-ttu-id="7ffa0-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7ffa0-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ffa0-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7ffa0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ffa0-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7ffa0-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ffa0-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7ffa0-124">Schema name</span></span>  <br/> |<span data-ttu-id="7ffa0-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7ffa0-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ffa0-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7ffa0-126">Validation file</span></span>  <br/> |<span data-ttu-id="7ffa0-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7ffa0-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ffa0-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7ffa0-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7ffa0-129">False</span><span class="sxs-lookup"><span data-stu-id="7ffa0-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ffa0-130">См. также</span><span class="sxs-lookup"><span data-stu-id="7ffa0-130">See also</span></span>



- [<span data-ttu-id="7ffa0-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7ffa0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

