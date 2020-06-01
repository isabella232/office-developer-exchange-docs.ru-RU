---
title: Контент
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
description: Элемент ContentType описывает тип MIME для содержимого вложения в многоцелевом формате.
ms.openlocfilehash: cb326bb761ea28e0e9f77501bf754c7c1f0318fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455228"
---
# <a name="contenttype"></a><span data-ttu-id="2f341-103">Контент</span><span class="sxs-lookup"><span data-stu-id="2f341-103">ContentType</span></span>

<span data-ttu-id="2f341-104">Элемент **ContentType** описывает тип MIME для содержимого вложения в многоцелевом формате.</span><span class="sxs-lookup"><span data-stu-id="2f341-104">The **ContentType** element describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span> 
  
```xml
<ContentType/>
```

 <span data-ttu-id="2f341-105">**String**</span><span class="sxs-lookup"><span data-stu-id="2f341-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f341-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2f341-106">Attributes and elements</span></span>

<span data-ttu-id="2f341-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2f341-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f341-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2f341-108">Attributes</span></span>

<span data-ttu-id="2f341-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2f341-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f341-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2f341-110">Child elements</span></span>

<span data-ttu-id="2f341-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2f341-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f341-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2f341-112">Parent elements</span></span>

|<span data-ttu-id="2f341-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2f341-113">**Element**</span></span>|<span data-ttu-id="2f341-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f341-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f341-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="2f341-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="2f341-116">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f341-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="2f341-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="2f341-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="2f341-118">Представляет файл, присоединенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f341-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2f341-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2f341-119">Text value</span></span>

<span data-ttu-id="2f341-120">Текстовое значение — это строковое значение, представляющее тип контента вложения.</span><span class="sxs-lookup"><span data-stu-id="2f341-120">The text value is a string value that represents the content type of the attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2f341-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="2f341-121">Remarks</span></span>

<span data-ttu-id="2f341-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2f341-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f341-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2f341-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f341-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2f341-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f341-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2f341-125">Schema name</span></span>  <br/> |<span data-ttu-id="2f341-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2f341-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f341-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2f341-127">Validation file</span></span>  <br/> |<span data-ttu-id="2f341-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2f341-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f341-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2f341-129">Can be empty</span></span>  <br/> |<span data-ttu-id="2f341-130">False</span><span class="sxs-lookup"><span data-stu-id="2f341-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f341-131">См. также</span><span class="sxs-lookup"><span data-stu-id="2f341-131">See also</span></span>



- [<span data-ttu-id="2f341-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2f341-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

