---
title: жетсервертимезонесреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponse
api_type:
- schema
ms.assetid: 97c94d32-10f1-4c3e-ab20-9fd7e8257e50
description: Элемент Жетсервертимезонесреспонсе определяет ответ на запрос операции GetServerTimeZones.
ms.openlocfilehash: 5a8dbe19055e3b697149c10df610d081cb65430b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460927"
---
# <a name="getservertimezonesresponse"></a><span data-ttu-id="adf03-103">жетсервертимезонесреспонсе</span><span class="sxs-lookup"><span data-stu-id="adf03-103">GetServerTimeZonesResponse</span></span>

<span data-ttu-id="adf03-104">Элемент **жетсервертимезонесреспонсе** определяет ответ на запрос [операции GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="adf03-104">The **GetServerTimeZonesResponse** element defines a response to a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponse>
   <ResponseMessages/>
</GetServerTimeZonesResponse>
```

 <span data-ttu-id="adf03-105">**жетсервертимезонесреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="adf03-105">**GetServerTimeZonesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="adf03-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="adf03-106">Attributes and elements</span></span>

<span data-ttu-id="adf03-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="adf03-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="adf03-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="adf03-108">Attributes</span></span>

<span data-ttu-id="adf03-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="adf03-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="adf03-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="adf03-110">Child elements</span></span>

|<span data-ttu-id="adf03-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="adf03-111">**Element**</span></span>|<span data-ttu-id="adf03-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="adf03-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="adf03-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="adf03-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="adf03-114">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="adf03-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="adf03-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="adf03-115">Parent elements</span></span>

<span data-ttu-id="adf03-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="adf03-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="adf03-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="adf03-117">Remarks</span></span>

<span data-ttu-id="adf03-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="adf03-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="adf03-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="adf03-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="adf03-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="adf03-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="adf03-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="adf03-121">Schema Name</span></span>  <br/> |<span data-ttu-id="adf03-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="adf03-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="adf03-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="adf03-123">Validation File</span></span>  <br/> |<span data-ttu-id="adf03-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="adf03-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="adf03-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="adf03-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="adf03-126">False</span><span class="sxs-lookup"><span data-stu-id="adf03-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="adf03-127">См. также</span><span class="sxs-lookup"><span data-stu-id="adf03-127">See also</span></span>



- [<span data-ttu-id="adf03-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="adf03-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

