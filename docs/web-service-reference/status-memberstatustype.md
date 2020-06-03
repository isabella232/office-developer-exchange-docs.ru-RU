---
title: Состояние (Мемберстатустипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: Элемент Status предоставляет сведения о состоянии члена списка рассылки на сервере.
ms.openlocfilehash: bfa0c349d6af51c1b2238c9749d2656541d31906
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465466"
---
# <a name="status-memberstatustype"></a><span data-ttu-id="73077-103">Состояние (Мемберстатустипе)</span><span class="sxs-lookup"><span data-stu-id="73077-103">Status (MemberStatusType)</span></span>

<span data-ttu-id="73077-104">Элемент **Status** предоставляет сведения о состоянии члена списка рассылки на сервере.</span><span class="sxs-lookup"><span data-stu-id="73077-104">The **Status** element provides information about the status of a distribution list member on the server.</span></span> 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 <span data-ttu-id="73077-105">**мемберстатустипе**</span><span class="sxs-lookup"><span data-stu-id="73077-105">**MemberStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73077-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="73077-106">Attributes and elements</span></span>

<span data-ttu-id="73077-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="73077-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73077-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="73077-108">Attributes</span></span>

<span data-ttu-id="73077-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73077-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73077-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="73077-110">Child elements</span></span>

<span data-ttu-id="73077-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73077-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73077-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="73077-112">Parent elements</span></span>

|<span data-ttu-id="73077-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="73077-113">**Element**</span></span>|<span data-ttu-id="73077-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="73077-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73077-115">Элемент</span><span class="sxs-lookup"><span data-stu-id="73077-115">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="73077-116">Представляет члена списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="73077-116">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73077-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="73077-117">Text value</span></span>

<span data-ttu-id="73077-118">В следующей таблице приведены возможные значения для элемента **Status** .</span><span class="sxs-lookup"><span data-stu-id="73077-118">The following table lists the possible values for the **Status** element.</span></span> 
  
<span data-ttu-id="73077-119">**Значения элементов Status**</span><span class="sxs-lookup"><span data-stu-id="73077-119">**Status element values**</span></span>

|<span data-ttu-id="73077-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="73077-120">**Value**</span></span>|<span data-ttu-id="73077-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="73077-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="73077-122">Нераспознанный</span><span class="sxs-lookup"><span data-stu-id="73077-122">Unrecognized</span></span>  <br/> |<span data-ttu-id="73077-123">Сведения об участниках являются недопустимыми или неопознанными.</span><span class="sxs-lookup"><span data-stu-id="73077-123">Member information is invalid or unrecognized.</span></span>  <br/> |
|<span data-ttu-id="73077-124">Normal</span><span class="sxs-lookup"><span data-stu-id="73077-124">Normal</span></span>  <br/> |<span data-ttu-id="73077-125">Сведения об участниках в списке рассылки синхронизируются с объектом, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="73077-125">Member information in a distribution list is in sync with the referenced object.</span></span>  <br/> |
|<span data-ttu-id="73077-126">Понижения</span><span class="sxs-lookup"><span data-stu-id="73077-126">Demoted</span></span>  <br/> |<span data-ttu-id="73077-127">Объект, на который указывает ссылка, недоступен.</span><span class="sxs-lookup"><span data-stu-id="73077-127">Referenced object is not available.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="73077-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="73077-128">Remarks</span></span>

<span data-ttu-id="73077-129">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="73077-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73077-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="73077-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73077-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="73077-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73077-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="73077-132">Schema Name</span></span>  <br/> |<span data-ttu-id="73077-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="73077-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="73077-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="73077-134">Validation File</span></span>  <br/> |<span data-ttu-id="73077-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="73077-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73077-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="73077-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="73077-137">False</span><span class="sxs-lookup"><span data-stu-id="73077-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73077-138">См. также</span><span class="sxs-lookup"><span data-stu-id="73077-138">See also</span></span>



- [<span data-ttu-id="73077-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="73077-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

