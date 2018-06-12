---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: Элемент AlternateId описание идентификатора для преобразования в запрос и результаты преобразованных идентификатор в ответе.
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761370"
---
# <a name="alternateid"></a><span data-ttu-id="d8aff-103">AlternateId</span><span class="sxs-lookup"><span data-stu-id="d8aff-103">AlternateId</span></span>

<span data-ttu-id="d8aff-104">Элемент **AlternateId** описание идентификатора для преобразования в запрос и результаты преобразованных идентификатор в ответе.</span><span class="sxs-lookup"><span data-stu-id="d8aff-104">The **AlternateId** element describes an identifier to convert in a request and the results of a converted identifier in the response.</span></span> 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 <span data-ttu-id="d8aff-105">**AlternateIdType**</span><span class="sxs-lookup"><span data-stu-id="d8aff-105">**AlternateIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8aff-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d8aff-106">Attributes and elements</span></span>

<span data-ttu-id="d8aff-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d8aff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8aff-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d8aff-108">Attributes</span></span>

|<span data-ttu-id="d8aff-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d8aff-109">**Attribute**</span></span>|<span data-ttu-id="d8aff-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8aff-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d8aff-111">Id</span><span class="sxs-lookup"><span data-stu-id="d8aff-111">Id</span></span>  <br/> |<span data-ttu-id="d8aff-112">Описывает идентификатор источника в запрос [операции ConvertId](convertid-operation.md) и идентификатор назначения в [операцию ConvertId](convertid-operation.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="d8aff-112">Describes the source identifier in a [ConvertId operation](convertid-operation.md) request and describes the destination identifier in a [ConvertId operation](convertid-operation.md) response.</span></span>  <br/> |
|<span data-ttu-id="d8aff-113">Формат</span><span class="sxs-lookup"><span data-stu-id="d8aff-113">Format</span></span>  <br/> |<span data-ttu-id="d8aff-114">Описывает формат источника в запрос [операции ConvertId](convertid-operation.md) и формат назначения в [операцию ConvertId](convertid-operation.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="d8aff-114">Describes the source format in a [ConvertId operation](convertid-operation.md) request and describes the destination format in a [ConvertId operation](convertid-operation.md) response.</span></span> <span data-ttu-id="d8aff-115">Формат назначения описывается атрибут **DestinationFormat** элемента [ConvertId](convertid.md) в запросе.</span><span class="sxs-lookup"><span data-stu-id="d8aff-115">The destination format is described by the **DestinationFormat** attribute of the [ConvertId](convertid.md) element in the request.</span></span> <span data-ttu-id="d8aff-116">Этот атрибут имеет тип **IdFormatType**.</span><span class="sxs-lookup"><span data-stu-id="d8aff-116">This attribute is of type **IdFormatType**.</span></span>  <br/> |
|<span data-ttu-id="d8aff-117">Почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="d8aff-117">Mailbox</span></span>  <br/> |<span data-ttu-id="d8aff-118">Описывает почтового ящика основной Simple Mail Transfer Protocol (SMTP) адрес, содержащий идентификаторы для перевода.</span><span class="sxs-lookup"><span data-stu-id="d8aff-118">Describes the mailbox primary Simple Mail Transfer Protocol (SMTP) address that contains the identifiers to translate.</span></span>  <br/> |
|<span data-ttu-id="d8aff-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="d8aff-119">IsArchive</span></span>  <br/> |<span data-ttu-id="d8aff-120">Указывает, представляет ли идентификатор архивных элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="d8aff-120">Indicates whether the identifier represents an archived item or folder.</span></span> <span data-ttu-id="d8aff-121">Значение **true** указывает, что идентификатор представляет архивных элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="d8aff-121">A value of **true** indicates that the identifier represents an archived item or folder.</span></span> <span data-ttu-id="d8aff-122">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d8aff-122">This attribute is optional.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="d8aff-123">Значения атрибутов формата</span><span class="sxs-lookup"><span data-stu-id="d8aff-123">Format attribute values</span></span>

|<span data-ttu-id="d8aff-124">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d8aff-124">**Value**</span></span>|<span data-ttu-id="d8aff-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8aff-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d8aff-126">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="d8aff-126">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="d8aff-127">Описываются идентификаторы, которые создаются веб-служб Exchange в первоначальной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="d8aff-127">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="d8aff-128">EwsId</span><span class="sxs-lookup"><span data-stu-id="d8aff-128">EwsId</span></span>  <br/> |<span data-ttu-id="d8aff-129">Описываются идентификаторы, которые создаются веб-служб Exchange, начиная с Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="d8aff-129">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="d8aff-130">Идентификатор записи</span><span class="sxs-lookup"><span data-stu-id="d8aff-130">EntryId</span></span>  <br/> |<span data-ttu-id="d8aff-131">Описываются идентификаторы MAPI, как и свойство **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="d8aff-131">Describes MAPI identifiers, as in the **PR_ENTRYID** property.</span></span>  <br/> |
|<span data-ttu-id="d8aff-132">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="d8aff-132">HexEntryId</span></span>  <br/> |<span data-ttu-id="d8aff-133">Описывает представление шестнадцатеричном формате **PR_ENTRYID** свойства.</span><span class="sxs-lookup"><span data-stu-id="d8aff-133">Describes a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="d8aff-134">Это формат идентификаторы событий календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="d8aff-134">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="d8aff-135">StoreId</span><span class="sxs-lookup"><span data-stu-id="d8aff-135">StoreId</span></span>  <br/> |<span data-ttu-id="d8aff-136">Описываются идентификаторы хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8aff-136">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="d8aff-137">OwaId</span><span class="sxs-lookup"><span data-stu-id="d8aff-137">OwaId</span></span>  <br/> |<span data-ttu-id="d8aff-138">Описывает идентификатор Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="d8aff-138">Describes an Outlook Web App identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d8aff-139">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d8aff-139">Child elements</span></span>

<span data-ttu-id="d8aff-140">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8aff-140">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8aff-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d8aff-141">Parent elements</span></span>

|<span data-ttu-id="d8aff-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d8aff-142">**Element**</span></span>|<span data-ttu-id="d8aff-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8aff-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8aff-144">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d8aff-144">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="d8aff-145">Содержит состояние и результат [операции ConvertId](convertid-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="d8aff-145">Contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d8aff-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="d8aff-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="d8aff-147">Содержит идентификаторы источника для преобразования.</span><span class="sxs-lookup"><span data-stu-id="d8aff-147">Contains the source identifiers to convert.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8aff-148">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d8aff-148">Text value</span></span>

<span data-ttu-id="d8aff-149">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8aff-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8aff-150">Замечания</span><span class="sxs-lookup"><span data-stu-id="d8aff-150">Remarks</span></span>

<span data-ttu-id="d8aff-151">Элемент **AlternateId** описание двух идентификаторов, идентификатор источника, который должен быть преобразован в запрос [операции ConvertId](convertid-operation.md) и преобразованные идентификатор в элементе [ConvertIdResponse](convertidresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="d8aff-151">The **AlternateId** element describes two identifiers, the source identifier that is to be converted in the [ConvertId operation](convertid-operation.md) request, and the converted identifier in the [ConvertIdResponse](convertidresponse.md) element.</span></span> 
  
<span data-ttu-id="d8aff-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8aff-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8aff-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d8aff-153">Element information</span></span>

||||
|:-----|:-----|:-----|
|<span data-ttu-id="d8aff-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d8aff-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8aff-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d8aff-155">Schema Name</span></span>  <br/> |<span data-ttu-id="d8aff-156">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d8aff-156">Messages schema</span></span>  <br/> |<span data-ttu-id="d8aff-157">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d8aff-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8aff-158">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d8aff-158">Validation File</span></span>  <br/> |<span data-ttu-id="d8aff-159">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d8aff-159">Messages.xsd</span></span>  <br/> |<span data-ttu-id="d8aff-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8aff-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8aff-161">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d8aff-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8aff-162">False</span><span class="sxs-lookup"><span data-stu-id="d8aff-162">False</span></span>  <br/> |<span data-ttu-id="d8aff-163">False</span><span class="sxs-lookup"><span data-stu-id="d8aff-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8aff-164">См. также</span><span class="sxs-lookup"><span data-stu-id="d8aff-164">See also</span></span>

- [<span data-ttu-id="d8aff-165">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="d8aff-165">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="d8aff-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d8aff-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="d8aff-167">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="d8aff-167">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

