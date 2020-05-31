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
ms.openlocfilehash: ef062433c80f0cca413c33012e1164b17e226faf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835580"
---
# <a name="status-memberstatustype"></a><span data-ttu-id="2fd3b-103">Состояние (Мемберстатустипе)</span><span class="sxs-lookup"><span data-stu-id="2fd3b-103">Status (MemberStatusType)</span></span>

<span data-ttu-id="2fd3b-104">Элемент **Status** предоставляет сведения о состоянии члена списка рассылки на сервере.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-104">The **Status** element provides information about the status of a distribution list member on the server.</span></span> 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 <span data-ttu-id="2fd3b-105">**мемберстатустипе**</span><span class="sxs-lookup"><span data-stu-id="2fd3b-105">**MemberStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2fd3b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2fd3b-106">Attributes and elements</span></span>

<span data-ttu-id="2fd3b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fd3b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2fd3b-108">Attributes</span></span>

<span data-ttu-id="2fd3b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2fd3b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2fd3b-110">Child elements</span></span>

<span data-ttu-id="2fd3b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2fd3b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2fd3b-112">Parent elements</span></span>

|<span data-ttu-id="2fd3b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2fd3b-113">**Element**</span></span>|<span data-ttu-id="2fd3b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2fd3b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fd3b-115">Элемент</span><span class="sxs-lookup"><span data-stu-id="2fd3b-115">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2fd3b-116">Представляет члена списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-116">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2fd3b-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2fd3b-117">Text value</span></span>

<span data-ttu-id="2fd3b-118">В следующей таблице приведены возможные значения для элемента **Status** .</span><span class="sxs-lookup"><span data-stu-id="2fd3b-118">The following table lists the possible values for the **Status** element.</span></span> 
  
<span data-ttu-id="2fd3b-119">**Значения элементов Status**</span><span class="sxs-lookup"><span data-stu-id="2fd3b-119">**Status element values**</span></span>

|<span data-ttu-id="2fd3b-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="2fd3b-120">**Value**</span></span>|<span data-ttu-id="2fd3b-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2fd3b-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2fd3b-122">Нераспознанный</span><span class="sxs-lookup"><span data-stu-id="2fd3b-122">Unrecognized</span></span>  <br/> |<span data-ttu-id="2fd3b-123">Сведения об участниках являются недопустимыми или неопознанными.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-123">Member information is invalid or unrecognized.</span></span>  <br/> |
|<span data-ttu-id="2fd3b-124">Normal</span><span class="sxs-lookup"><span data-stu-id="2fd3b-124">Normal</span></span>  <br/> |<span data-ttu-id="2fd3b-125">Сведения об участниках в списке рассылки синхронизируются с объектом, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-125">Member information in a distribution list is in sync with the referenced object.</span></span>  <br/> |
|<span data-ttu-id="2fd3b-126">Понижения</span><span class="sxs-lookup"><span data-stu-id="2fd3b-126">Demoted</span></span>  <br/> |<span data-ttu-id="2fd3b-127">Объект, на который указывает ссылка, недоступен.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-127">Referenced object is not available.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2fd3b-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="2fd3b-128">Remarks</span></span>

<span data-ttu-id="2fd3b-129">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2fd3b-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2fd3b-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2fd3b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fd3b-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2fd3b-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2fd3b-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2fd3b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="2fd3b-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2fd3b-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="2fd3b-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2fd3b-134">Validation File</span></span>  <br/> |<span data-ttu-id="2fd3b-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2fd3b-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2fd3b-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2fd3b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="2fd3b-137">False</span><span class="sxs-lookup"><span data-stu-id="2fd3b-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2fd3b-138">См. также</span><span class="sxs-lookup"><span data-stu-id="2fd3b-138">See also</span></span>



- [<span data-ttu-id="2fd3b-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2fd3b-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

