---
title: contentType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentType
api_type:
- schema
ms.assetid: f91ff0df-0d8a-43ea-a188-d80f0e885f19
description: Элемент ContentType описывает тип Multipurpose Internet Mail Extensions (MIME) для содержимого вложения.
ms.openlocfilehash: 489df47343051623d5b6a98557f2bd434a5dad52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761803"
---
# <a name="contenttype"></a><span data-ttu-id="511db-103">contentType</span><span class="sxs-lookup"><span data-stu-id="511db-103">ContentType</span></span>

<span data-ttu-id="511db-104">Элемент **ContentType** описывает тип Multipurpose Internet Mail Extensions (MIME) для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="511db-104">The **ContentType** element describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span> 
  
```xml
<ContentType/>
```

 <span data-ttu-id="511db-105">**Строка**</span><span class="sxs-lookup"><span data-stu-id="511db-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="511db-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="511db-106">Attributes and elements</span></span>

<span data-ttu-id="511db-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="511db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="511db-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="511db-108">Attributes</span></span>

<span data-ttu-id="511db-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="511db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="511db-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="511db-110">Child elements</span></span>

<span data-ttu-id="511db-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="511db-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="511db-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="511db-112">Parent elements</span></span>

|<span data-ttu-id="511db-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="511db-113">**Element**</span></span>|<span data-ttu-id="511db-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="511db-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="511db-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="511db-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="511db-116">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="511db-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="511db-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="511db-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="511db-118">Представляет файл, подключенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="511db-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="511db-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="511db-119">Text value</span></span>

<span data-ttu-id="511db-120">Текстовое значение является значение типа string, представляющий тип контента вложения.</span><span class="sxs-lookup"><span data-stu-id="511db-120">The text value is a string value that represents the content type of the attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="511db-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="511db-121">Remarks</span></span>

<span data-ttu-id="511db-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="511db-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="511db-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="511db-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="511db-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="511db-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="511db-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="511db-125">Schema name</span></span>  <br/> |<span data-ttu-id="511db-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="511db-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="511db-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="511db-127">Validation file</span></span>  <br/> |<span data-ttu-id="511db-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="511db-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="511db-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="511db-129">Can be empty</span></span>  <br/> |<span data-ttu-id="511db-130">False</span><span class="sxs-lookup"><span data-stu-id="511db-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="511db-131">См. также</span><span class="sxs-lookup"><span data-stu-id="511db-131">See also</span></span>



- [<span data-ttu-id="511db-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="511db-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

