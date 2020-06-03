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
ms.openlocfilehash: 81f6acf69ff702bd0645663cb2e499ee5b45ea78
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458952"
---
# <a name="content"></a><span data-ttu-id="e7515-103">Контент</span><span class="sxs-lookup"><span data-stu-id="e7515-103">Content</span></span>

<span data-ttu-id="e7515-104">Элемент **Content** содержит содержимое вложенного файла в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="e7515-104">The **Content** element contains the Base64-encoded contents of a file attachment.</span></span> 
  
```xml
<Content/>
```

 <span data-ttu-id="e7515-105">**Base64Binary**</span><span class="sxs-lookup"><span data-stu-id="e7515-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7515-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e7515-106">Attributes and elements</span></span>

<span data-ttu-id="e7515-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e7515-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7515-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e7515-108">Attributes</span></span>

<span data-ttu-id="e7515-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e7515-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7515-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e7515-110">Child elements</span></span>

<span data-ttu-id="e7515-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e7515-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7515-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e7515-112">Parent elements</span></span>

|<span data-ttu-id="e7515-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e7515-113">**Element**</span></span>|<span data-ttu-id="e7515-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7515-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7515-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="e7515-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="e7515-116">Представляет файл t — саттачед элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7515-116">Represents a file t is thattached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7515-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e7515-117">Text value</span></span>

<span data-ttu-id="e7515-118">Строковое значение представляет двоичные данные вложенного файла в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="e7515-118">The string value represents the Base64-encoded binary data of the file attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7515-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="e7515-119">Remarks</span></span>

<span data-ttu-id="e7515-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e7515-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7515-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e7515-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7515-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e7515-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7515-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e7515-123">Schema name</span></span>  <br/> |<span data-ttu-id="e7515-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e7515-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="e7515-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e7515-125">Validation file</span></span>  <br/> |<span data-ttu-id="e7515-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e7515-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7515-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e7515-127">Can be empty</span></span>  <br/> |<span data-ttu-id="e7515-128">False</span><span class="sxs-lookup"><span data-stu-id="e7515-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7515-129">См. также</span><span class="sxs-lookup"><span data-stu-id="e7515-129">See also</span></span>



- [<span data-ttu-id="e7515-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e7515-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

