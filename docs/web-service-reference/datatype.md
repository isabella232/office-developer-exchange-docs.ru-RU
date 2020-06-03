---
title: DataType
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
description: Элемент DataType описывает тип данных, к которым общий доступ предоставляется в общей папке.
ms.openlocfilehash: a7df8d38e10f0ab31038d790d8f35208d1be66d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458833"
---
# <a name="datatype"></a><span data-ttu-id="f06f2-103">DataType</span><span class="sxs-lookup"><span data-stu-id="f06f2-103">DataType</span></span>

<span data-ttu-id="f06f2-104">Элемент **DataType** описывает тип данных, к которым общий доступ предоставляется в общей папке.</span><span class="sxs-lookup"><span data-stu-id="f06f2-104">The **DataType** element describes the type of data that is shared by a shared folder.</span></span> 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

<span data-ttu-id="f06f2-105">**шарингдататипе**</span><span class="sxs-lookup"><span data-stu-id="f06f2-105">**SharingDataType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f06f2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f06f2-106">Attributes and elements</span></span>

<span data-ttu-id="f06f2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f06f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f06f2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f06f2-108">Attributes</span></span>

<span data-ttu-id="f06f2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f06f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f06f2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f06f2-110">Child elements</span></span>

<span data-ttu-id="f06f2-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f06f2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f06f2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f06f2-112">Parent elements</span></span>

|<span data-ttu-id="f06f2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f06f2-113">**Element**</span></span>|<span data-ttu-id="f06f2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f06f2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f06f2-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="f06f2-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="f06f2-116">Определяет запрос на получение идентификатора локальной папки указанной общей папки.</span><span class="sxs-lookup"><span data-stu-id="f06f2-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f06f2-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f06f2-117">Text value</span></span>

<span data-ttu-id="f06f2-118">В следующей таблице приведены возможные значения для элемента **DataType** .</span><span class="sxs-lookup"><span data-stu-id="f06f2-118">The following table lists the possible values for the **DataType** element.</span></span> 
  
<span data-ttu-id="f06f2-119">**Значения элементов DataType**</span><span class="sxs-lookup"><span data-stu-id="f06f2-119">**DataType element values**</span></span>

|<span data-ttu-id="f06f2-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f06f2-120">**Value**</span></span>|<span data-ttu-id="f06f2-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f06f2-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f06f2-122">Календарь</span><span class="sxs-lookup"><span data-stu-id="f06f2-122">Calendar</span></span>  <br/> |<span data-ttu-id="f06f2-123">Указывает, что общая папка содержит данные календаря.</span><span class="sxs-lookup"><span data-stu-id="f06f2-123">Indicates that the shared folder contains calendar information.</span></span>  <br/> |
|<span data-ttu-id="f06f2-124">Контакты</span><span class="sxs-lookup"><span data-stu-id="f06f2-124">Contacts</span></span>  <br/> |<span data-ttu-id="f06f2-125">Указывает, что общая папка содержит контактные данные.</span><span class="sxs-lookup"><span data-stu-id="f06f2-125">Indicates that the shared folder contains contact information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f06f2-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="f06f2-126">Remarks</span></span>

<span data-ttu-id="f06f2-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f06f2-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f06f2-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f06f2-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f06f2-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f06f2-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f06f2-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f06f2-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f06f2-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f06f2-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f06f2-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f06f2-132">Validation File</span></span>  <br/> |<span data-ttu-id="f06f2-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f06f2-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f06f2-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f06f2-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f06f2-135">False</span><span class="sxs-lookup"><span data-stu-id="f06f2-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f06f2-136">См. также</span><span class="sxs-lookup"><span data-stu-id="f06f2-136">See also</span></span>

- [<span data-ttu-id="f06f2-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f06f2-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

