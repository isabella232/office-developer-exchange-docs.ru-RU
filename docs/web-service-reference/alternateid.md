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
description: Элемент AlternateId описывает идентификатор для преобразования в запросе и результаты преобразованного идентификатора в отклике.
ms.openlocfilehash: 26df68bd814c2d323630c6bb40b4c31745017c71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527455"
---
# <a name="alternateid"></a><span data-ttu-id="d20cc-103">AlternateId</span><span class="sxs-lookup"><span data-stu-id="d20cc-103">AlternateId</span></span>

<span data-ttu-id="d20cc-104">Элемент **AlternateId** описывает идентификатор для преобразования в запросе и результаты преобразованного идентификатора в отклике.</span><span class="sxs-lookup"><span data-stu-id="d20cc-104">The **AlternateId** element describes an identifier to convert in a request and the results of a converted identifier in the response.</span></span> 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 <span data-ttu-id="d20cc-105">**алтернатеидтипе**</span><span class="sxs-lookup"><span data-stu-id="d20cc-105">**AlternateIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d20cc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d20cc-106">Attributes and elements</span></span>

<span data-ttu-id="d20cc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d20cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d20cc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d20cc-108">Attributes</span></span>

|<span data-ttu-id="d20cc-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d20cc-109">**Attribute**</span></span>|<span data-ttu-id="d20cc-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d20cc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d20cc-111">Id</span><span class="sxs-lookup"><span data-stu-id="d20cc-111">Id</span></span>  <br/> |<span data-ttu-id="d20cc-112">Описывает идентификатор источника в запросе [операции ConvertId](convertid-operation.md) и описывает идентификатор назначения в ответе [операции ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d20cc-112">Describes the source identifier in a [ConvertId operation](convertid-operation.md) request and describes the destination identifier in a [ConvertId operation](convertid-operation.md) response.</span></span>  <br/> |
|<span data-ttu-id="d20cc-113">Format</span><span class="sxs-lookup"><span data-stu-id="d20cc-113">Format</span></span>  <br/> |<span data-ttu-id="d20cc-114">Описывает исходный формат в запросе [операции ConvertId](convertid-operation.md) и описывает формат назначения в ответе [операции ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d20cc-114">Describes the source format in a [ConvertId operation](convertid-operation.md) request and describes the destination format in a [ConvertId operation](convertid-operation.md) response.</span></span> <span data-ttu-id="d20cc-115">Формат назначения описывается атрибутом **дестинатионформат** элемента [ConvertId](convertid.md) в запросе.</span><span class="sxs-lookup"><span data-stu-id="d20cc-115">The destination format is described by the **DestinationFormat** attribute of the [ConvertId](convertid.md) element in the request.</span></span> <span data-ttu-id="d20cc-116">Этот атрибут относится к типу **идформаттипе**.</span><span class="sxs-lookup"><span data-stu-id="d20cc-116">This attribute is of type **IdFormatType**.</span></span>  <br/> |
|<span data-ttu-id="d20cc-117">Почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="d20cc-117">Mailbox</span></span>  <br/> |<span data-ttu-id="d20cc-118">Описывает основной SMTP-адрес почтового ящика, который содержит идентификаторы для преобразования.</span><span class="sxs-lookup"><span data-stu-id="d20cc-118">Describes the mailbox primary Simple Mail Transfer Protocol (SMTP) address that contains the identifiers to translate.</span></span>  <br/> |
|<span data-ttu-id="d20cc-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="d20cc-119">IsArchive</span></span>  <br/> |<span data-ttu-id="d20cc-120">Указывает, представляет ли идентификатор архивированный элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="d20cc-120">Indicates whether the identifier represents an archived item or folder.</span></span> <span data-ttu-id="d20cc-121">Значение **true** указывает, что идентификатор представляет архивный элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="d20cc-121">A value of **true** indicates that the identifier represents an archived item or folder.</span></span> <span data-ttu-id="d20cc-122">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d20cc-122">This attribute is optional.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="d20cc-123">Форматирование значений атрибутов</span><span class="sxs-lookup"><span data-stu-id="d20cc-123">Format attribute values</span></span>

|<span data-ttu-id="d20cc-124">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d20cc-124">**Value**</span></span>|<span data-ttu-id="d20cc-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d20cc-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d20cc-126">евслегациид</span><span class="sxs-lookup"><span data-stu-id="d20cc-126">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="d20cc-127">Описывает идентификаторы, созданные веб-службами Exchange в исходной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="d20cc-127">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="d20cc-128">евсид</span><span class="sxs-lookup"><span data-stu-id="d20cc-128">EwsId</span></span>  <br/> |<span data-ttu-id="d20cc-129">Описание идентификаторов, создаваемых веб-службами Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d20cc-129">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="d20cc-130">Код</span><span class="sxs-lookup"><span data-stu-id="d20cc-130">EntryId</span></span>  <br/> |<span data-ttu-id="d20cc-131">Описывает идентификаторы MAPI, как в свойстве **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="d20cc-131">Describes MAPI identifiers, as in the **PR_ENTRYID** property.</span></span>  <br/> |
|<span data-ttu-id="d20cc-132">хексентрид</span><span class="sxs-lookup"><span data-stu-id="d20cc-132">HexEntryId</span></span>  <br/> |<span data-ttu-id="d20cc-133">Описывает представление свойства **PR_ENTRYID** в шестнадцатеричном формате.</span><span class="sxs-lookup"><span data-stu-id="d20cc-133">Describes a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="d20cc-134">Это формат идентификаторов событий календаря доступности.</span><span class="sxs-lookup"><span data-stu-id="d20cc-134">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="d20cc-135">StoreId</span><span class="sxs-lookup"><span data-stu-id="d20cc-135">StoreId</span></span>  <br/> |<span data-ttu-id="d20cc-136">Описывает идентификаторы хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="d20cc-136">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="d20cc-137">оваид</span><span class="sxs-lookup"><span data-stu-id="d20cc-137">OwaId</span></span>  <br/> |<span data-ttu-id="d20cc-138">Описывает идентификатор Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="d20cc-138">Describes an Outlook Web App identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d20cc-139">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d20cc-139">Child elements</span></span>

<span data-ttu-id="d20cc-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d20cc-140">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d20cc-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d20cc-141">Parent elements</span></span>

|<span data-ttu-id="d20cc-142">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d20cc-142">**Element**</span></span>|<span data-ttu-id="d20cc-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d20cc-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d20cc-144">конвертидреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="d20cc-144">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="d20cc-145">Содержит состояние и результат запроса [операции ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d20cc-145">Contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d20cc-146">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="d20cc-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="d20cc-147">Содержит идентификаторы источников для преобразования.</span><span class="sxs-lookup"><span data-stu-id="d20cc-147">Contains the source identifiers to convert.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d20cc-148">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d20cc-148">Text value</span></span>

<span data-ttu-id="d20cc-149">Нет.</span><span class="sxs-lookup"><span data-stu-id="d20cc-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d20cc-150">Примечания</span><span class="sxs-lookup"><span data-stu-id="d20cc-150">Remarks</span></span>

<span data-ttu-id="d20cc-151">Элемент **AlternateId** описывает два идентификатора, идентификатор источника, который необходимо преобразовать в запрос [операции ConvertId](convertid-operation.md) , и преобразованный идентификатор в элементе [конвертидреспонсе](convertidresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="d20cc-151">The **AlternateId** element describes two identifiers, the source identifier that is to be converted in the [ConvertId operation](convertid-operation.md) request, and the converted identifier in the [ConvertIdResponse](convertidresponse.md) element.</span></span> 
  
<span data-ttu-id="d20cc-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d20cc-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d20cc-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d20cc-153">Element information</span></span>

||||
|:-----|:-----|:-----|
|<span data-ttu-id="d20cc-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d20cc-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d20cc-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d20cc-155">Schema Name</span></span>  <br/> |<span data-ttu-id="d20cc-156">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d20cc-156">Messages schema</span></span>  <br/> |<span data-ttu-id="d20cc-157">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d20cc-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="d20cc-158">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d20cc-158">Validation File</span></span>  <br/> |<span data-ttu-id="d20cc-159">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d20cc-159">Messages.xsd</span></span>  <br/> |<span data-ttu-id="d20cc-160">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d20cc-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d20cc-161">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d20cc-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="d20cc-162">False</span><span class="sxs-lookup"><span data-stu-id="d20cc-162">False</span></span>  <br/> |<span data-ttu-id="d20cc-163">False</span><span class="sxs-lookup"><span data-stu-id="d20cc-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d20cc-164">См. также</span><span class="sxs-lookup"><span data-stu-id="d20cc-164">See also</span></span>

- [<span data-ttu-id="d20cc-165">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="d20cc-165">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="d20cc-166">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d20cc-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="d20cc-167">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="d20cc-167">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

