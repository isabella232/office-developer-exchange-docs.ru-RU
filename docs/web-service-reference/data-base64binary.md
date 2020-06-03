---
title: Data (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: Элемент Data содержит данные одного экспортированного элемента или элемента для отправки в почтовый ящик.
ms.openlocfilehash: 43ee16ca7caf634756ca00a88715d9834adad92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526972"
---
# <a name="data-base64binary"></a><span data-ttu-id="33023-103">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="33023-103">Data (base64Binary)</span></span>

<span data-ttu-id="33023-104">Элемент **Data** содержит данные одного экспортированного элемента или элемента для отправки в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="33023-104">The **Data** element contains the data of a single exported item or an item to upload into a mailbox.</span></span> 
  
```XML
<Data/>
```

<span data-ttu-id="33023-105">**xs: base64Binary**</span><span class="sxs-lookup"><span data-stu-id="33023-105">**xs:base64Binary**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="33023-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33023-106">Attributes and elements</span></span>

<span data-ttu-id="33023-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="33023-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33023-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33023-108">Attributes</span></span>

<span data-ttu-id="33023-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33023-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33023-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33023-110">Child elements</span></span>

<span data-ttu-id="33023-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33023-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33023-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33023-112">Parent elements</span></span>

|<span data-ttu-id="33023-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33023-113">**Element**</span></span>|<span data-ttu-id="33023-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33023-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33023-115">експортитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="33023-115">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="33023-116">Содержит состояние и результаты запроса на экспорт одного элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="33023-116">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="33023-117">Элемент (Уплоадитемтипе)</span><span class="sxs-lookup"><span data-stu-id="33023-117">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="33023-118">Представляет отдельный элемент для отправки в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="33023-118">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33023-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33023-119">Text value</span></span>

<span data-ttu-id="33023-120">Элемент **Data** содержит имена и значения свойств для экспортированного элемента или элемента, которые будут отправлены в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="33023-120">The **Data** element contains the property names and values for an exported item or an item that will be uploaded into a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="33023-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="33023-121">Remarks</span></span>

<span data-ttu-id="33023-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="33023-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33023-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33023-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33023-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33023-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="33023-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33023-125">Schema Name</span></span>  <br/> |<span data-ttu-id="33023-126">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="33023-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="33023-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33023-127">Validation File</span></span>  <br/> |<span data-ttu-id="33023-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="33023-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33023-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33023-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="33023-130">False</span><span class="sxs-lookup"><span data-stu-id="33023-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33023-131">См. также</span><span class="sxs-lookup"><span data-stu-id="33023-131">See also</span></span>

- [<span data-ttu-id="33023-132">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="33023-132">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="33023-133">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="33023-133">UploadItems operation</span></span>](uploaditems-operation.md)

