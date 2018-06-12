---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: Элемент ShowExternalRecipientCount указывает ли объекты-получатели GetMailTips операции для отображения почтовые подсказки, которые указывают число внешних получателей, к которым адресовано сообщение.
ms.openlocfilehash: 1fd3ceb629689c560dc60afe01f0413602f79a0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835491"
---
# <a name="showexternalrecipientcount"></a><span data-ttu-id="87740-103">ShowExternalRecipientCount</span><span class="sxs-lookup"><span data-stu-id="87740-103">ShowExternalRecipientCount</span></span>

<span data-ttu-id="87740-104">Элемент **ShowExternalRecipientCount** указывает ли объекты-получатели [GetMailTips операции](getmailtips-operation.md) для отображения почтовые подсказки, которые указывают число внешних получателей, к которым адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="87740-104">The **ShowExternalRecipientCount** element indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 <span data-ttu-id="87740-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="87740-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87740-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="87740-106">Attributes and elements</span></span>

<span data-ttu-id="87740-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="87740-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87740-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="87740-108">Attributes</span></span>

<span data-ttu-id="87740-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="87740-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87740-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="87740-110">Child elements</span></span>

<span data-ttu-id="87740-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="87740-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="87740-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="87740-112">Parent elements</span></span>

|<span data-ttu-id="87740-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="87740-113">**Element**</span></span>|<span data-ttu-id="87740-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87740-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87740-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="87740-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="87740-116">Содержит сведения о конфигурации службы для службы советы почты.</span><span class="sxs-lookup"><span data-stu-id="87740-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="87740-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="87740-117">Text value</span></span>

<span data-ttu-id="87740-118">Текстовое значение этого элемента равно **true** , если у потребителей [GetMailTips операции](getmailtips-operation.md) для отображения почтовые подсказки, которые указывают число внешних получателей, к которым адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="87740-118">The text value of this element is **true** if consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="87740-119">Значение равно **false** , если объекты-получатели [GetMailTips операция](getmailtips-operation.md) не нужно показать почтовые подсказки, которые указывают число внешних получателей, к которым адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="87740-119">The value is **false** if consumers of the [GetMailTips operation](getmailtips-operation.md) do not have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="87740-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="87740-120">Remarks</span></span>

<span data-ttu-id="87740-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="87740-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87740-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="87740-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87740-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="87740-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="87740-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="87740-124">Schema Name</span></span>  <br/> |<span data-ttu-id="87740-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="87740-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="87740-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="87740-126">Validation File</span></span>  <br/> |<span data-ttu-id="87740-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="87740-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="87740-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="87740-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="87740-129">False</span><span class="sxs-lookup"><span data-stu-id="87740-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87740-130">См. также</span><span class="sxs-lookup"><span data-stu-id="87740-130">See also</span></span>



[<span data-ttu-id="87740-131">Операция GetMailTips</span><span class="sxs-lookup"><span data-stu-id="87740-131">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="87740-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="87740-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

