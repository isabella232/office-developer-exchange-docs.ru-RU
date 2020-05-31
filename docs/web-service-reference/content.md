---
title: Содержание
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Content
api_type:
- schema
ms.assetid: 24f8c54a-505f-4fc0-b7e7-93ad50b97070
description: Элемент Content содержит содержимое вложенного файла в кодировке Base64.
ms.openlocfilehash: 20afe6286d3efaa5da6cdc88e397e88fddb1d8c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761788"
---
# <a name="content"></a><span data-ttu-id="2628e-103">Контентная</span><span class="sxs-lookup"><span data-stu-id="2628e-103">Content</span></span>

<span data-ttu-id="2628e-104">Элемент **Content** содержит содержимое вложенного файла в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="2628e-104">The **Content** element contains the Base64-encoded contents of a file attachment.</span></span> 
  
```xml
<Content/>
```

 <span data-ttu-id="2628e-105">**Base64Binary**</span><span class="sxs-lookup"><span data-stu-id="2628e-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2628e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2628e-106">Attributes and elements</span></span>

<span data-ttu-id="2628e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2628e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2628e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2628e-108">Attributes</span></span>

<span data-ttu-id="2628e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2628e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2628e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2628e-110">Child elements</span></span>

<span data-ttu-id="2628e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2628e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2628e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2628e-112">Parent elements</span></span>

|<span data-ttu-id="2628e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2628e-113">**Element**</span></span>|<span data-ttu-id="2628e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2628e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2628e-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="2628e-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="2628e-116">Представляет файл t — саттачед элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2628e-116">Represents a file t is thattached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2628e-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2628e-117">Text value</span></span>

<span data-ttu-id="2628e-118">Строковое значение представляет двоичные данные вложенного файла в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="2628e-118">The string value represents the Base64-encoded binary data of the file attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2628e-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="2628e-119">Remarks</span></span>

<span data-ttu-id="2628e-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2628e-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2628e-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2628e-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2628e-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2628e-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2628e-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2628e-123">Schema name</span></span>  <br/> |<span data-ttu-id="2628e-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2628e-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="2628e-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2628e-125">Validation file</span></span>  <br/> |<span data-ttu-id="2628e-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2628e-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2628e-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2628e-127">Can be empty</span></span>  <br/> |<span data-ttu-id="2628e-128">False</span><span class="sxs-lookup"><span data-stu-id="2628e-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2628e-129">См. также</span><span class="sxs-lookup"><span data-stu-id="2628e-129">See also</span></span>



- [<span data-ttu-id="2628e-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2628e-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

