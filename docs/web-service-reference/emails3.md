---
title: Emails3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f4dc589-4530-4a35-b2a6-0c83cac23637
description: Элемент Emails3 указывает массив значений EmailAddressAttributedValue и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 1d174000d59883446bb7f61af90278d197ef5ed9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762300"
---
# <a name="emails3"></a><span data-ttu-id="2fffe-103">Emails3</span><span class="sxs-lookup"><span data-stu-id="2fffe-103">Emails3</span></span>

<span data-ttu-id="2fffe-104">Элемент **Emails3** указывает массив значений **EmailAddressAttributedValue** и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="2fffe-104">The **Emails3** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails3>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails3>
```

 <span data-ttu-id="2fffe-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2fffe-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2fffe-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2fffe-106">Attributes and elements</span></span>

<span data-ttu-id="2fffe-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2fffe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fffe-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2fffe-108">Attributes</span></span>

<span data-ttu-id="2fffe-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2fffe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2fffe-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2fffe-110">Child elements</span></span>

|<span data-ttu-id="2fffe-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2fffe-111">**Element**</span></span>|<span data-ttu-id="2fffe-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2fffe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fffe-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="2fffe-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="2fffe-114">Указывает экземпляр массив адресов электронной почты и их связанные атрибуты.</span><span class="sxs-lookup"><span data-stu-id="2fffe-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2fffe-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2fffe-115">Parent elements</span></span>

|<span data-ttu-id="2fffe-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2fffe-116">**Element**</span></span>|<span data-ttu-id="2fffe-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2fffe-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fffe-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="2fffe-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2fffe-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="2fffe-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2fffe-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="2fffe-120">Remarks</span></span>

<span data-ttu-id="2fffe-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2fffe-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2fffe-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2fffe-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2fffe-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2fffe-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fffe-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2fffe-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2fffe-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2fffe-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2fffe-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="2fffe-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2fffe-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2fffe-127">Validation File</span></span>  <br/> |<span data-ttu-id="2fffe-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2fffe-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2fffe-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2fffe-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2fffe-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2fffe-130">See also</span></span>



- [<span data-ttu-id="2fffe-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2fffe-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

