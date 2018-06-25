---
title: Тип данных
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DataType
api_type:
- schema
ms.assetid: 267fe5aa-f9b1-4d4c-ac11-0f2e50ec2627
description: Тип данных элемент описывает тип данных, общий для общей папки.
ms.openlocfilehash: b1adac8e3029abd64df96ab1560706babe4b12f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761978"
---
# <a name="datatype"></a><span data-ttu-id="516d9-103">Тип данных</span><span class="sxs-lookup"><span data-stu-id="516d9-103">DataType</span></span>

<span data-ttu-id="516d9-104">**Тип данных** элемент описывает тип данных, общий для общей папки.</span><span class="sxs-lookup"><span data-stu-id="516d9-104">The **DataType** element describes the type of data that is shared by a shared folder.</span></span> 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

<span data-ttu-id="516d9-105">**SharingDataType**</span><span class="sxs-lookup"><span data-stu-id="516d9-105">**SharingDataType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="516d9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="516d9-106">Attributes and elements</span></span>

<span data-ttu-id="516d9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="516d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="516d9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="516d9-108">Attributes</span></span>

<span data-ttu-id="516d9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="516d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="516d9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="516d9-110">Child elements</span></span>

<span data-ttu-id="516d9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="516d9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="516d9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="516d9-112">Parent elements</span></span>

|<span data-ttu-id="516d9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="516d9-113">**Element**</span></span>|<span data-ttu-id="516d9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="516d9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="516d9-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="516d9-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="516d9-116">Определяет запрос на получение идентификатора локальной папки указанной общей папке.</span><span class="sxs-lookup"><span data-stu-id="516d9-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="516d9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="516d9-117">Text value</span></span>

<span data-ttu-id="516d9-118">В следующей таблице перечислены возможные значения для элемента **типа данных** .</span><span class="sxs-lookup"><span data-stu-id="516d9-118">The following table lists the possible values for the **DataType** element.</span></span> 
  
<span data-ttu-id="516d9-119">**Тип данных значения элементов**</span><span class="sxs-lookup"><span data-stu-id="516d9-119">**DataType element values**</span></span>

|<span data-ttu-id="516d9-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="516d9-120">**Value**</span></span>|<span data-ttu-id="516d9-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="516d9-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="516d9-122">Календарь</span><span class="sxs-lookup"><span data-stu-id="516d9-122">Calendar</span></span>  <br/> |<span data-ttu-id="516d9-123">Указывает, что общей папке содержит данные календаря.</span><span class="sxs-lookup"><span data-stu-id="516d9-123">Indicates that the shared folder contains calendar information.</span></span>  <br/> |
|<span data-ttu-id="516d9-124">Контакты</span><span class="sxs-lookup"><span data-stu-id="516d9-124">Contacts</span></span>  <br/> |<span data-ttu-id="516d9-125">Указывает, что общей папке содержит контактные сведения.</span><span class="sxs-lookup"><span data-stu-id="516d9-125">Indicates that the shared folder contains contact information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="516d9-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="516d9-126">Remarks</span></span>

<span data-ttu-id="516d9-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="516d9-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="516d9-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="516d9-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="516d9-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="516d9-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="516d9-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="516d9-130">Schema Name</span></span>  <br/> |<span data-ttu-id="516d9-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="516d9-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="516d9-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="516d9-132">Validation File</span></span>  <br/> |<span data-ttu-id="516d9-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="516d9-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="516d9-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="516d9-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="516d9-135">False</span><span class="sxs-lookup"><span data-stu-id="516d9-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="516d9-136">См. также</span><span class="sxs-lookup"><span data-stu-id="516d9-136">See also</span></span>

- [<span data-ttu-id="516d9-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="516d9-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

