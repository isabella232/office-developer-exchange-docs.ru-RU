---
title: Состояние
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- State
api_type:
- schema
ms.assetid: bcce7b0e-d504-4a1f-a530-db80b207f201
description: Элемент состояния представляет состояние расположения для элемента контакта.
ms.openlocfilehash: caa9541d30eaa04cc3f2dda0ebbf687b156c4f64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835565"
---
# <a name="state"></a><span data-ttu-id="1126f-103">Состояние</span><span class="sxs-lookup"><span data-stu-id="1126f-103">State</span></span>

<span data-ttu-id="1126f-104">Элемент **состояния** представляет состояние расположения для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="1126f-104">The **State** element represents the state of residence for a contact item.</span></span> 
  
```xml
<State/>
```

<span data-ttu-id="1126f-105">**string**</span><span class="sxs-lookup"><span data-stu-id="1126f-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1126f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1126f-106">Attributes and elements</span></span>

<span data-ttu-id="1126f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1126f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1126f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1126f-108">Attributes</span></span>

<span data-ttu-id="1126f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1126f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1126f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1126f-110">Child elements</span></span>

<span data-ttu-id="1126f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1126f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1126f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1126f-112">Parent elements</span></span>

|<span data-ttu-id="1126f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1126f-113">**Element**</span></span>|<span data-ttu-id="1126f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1126f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1126f-115">Запись (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="1126f-115">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="1126f-116">Описывает один физический адрес для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="1126f-116">Describes a single physical address for a contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1126f-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1126f-117">Text value</span></span>

<span data-ttu-id="1126f-118">Строковое значение, представляющее имя состояний является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="1126f-118">A string value that represents the name of a state is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1126f-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="1126f-119">Remarks</span></span>

<span data-ttu-id="1126f-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1126f-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1126f-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1126f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1126f-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1126f-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1126f-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1126f-123">Schema name</span></span>  <br/> |<span data-ttu-id="1126f-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1126f-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="1126f-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1126f-125">Validation file</span></span>  <br/> |<span data-ttu-id="1126f-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1126f-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1126f-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1126f-127">Can be empty</span></span>  <br/> |<span data-ttu-id="1126f-128">False</span><span class="sxs-lookup"><span data-stu-id="1126f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1126f-129">См. также</span><span class="sxs-lookup"><span data-stu-id="1126f-129">See also</span></span>

- [<span data-ttu-id="1126f-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1126f-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="1126f-131">Создание контактов (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="1126f-131">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
- [<span data-ttu-id="1126f-132">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="1126f-132">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="1126f-133">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="1126f-133">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

