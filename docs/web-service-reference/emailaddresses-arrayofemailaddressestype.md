---
title: EmailAddresses (ArrayOfEmailAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95084659-aa5a-4bac-8977-00db3b87883e
description: Элемент EmailAddresses указывает массив всех адресов электронной почты, связанного пользователя.
ms.openlocfilehash: 292d4c3f12b01f25fd094b2ab6d9c2d484d37694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762292"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="aef50-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="aef50-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="aef50-104">Элемент **EmailAddresses** указывает массив всех адресов электронной почты, связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="aef50-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="aef50-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="aef50-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aef50-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aef50-106">Attributes and elements</span></span>

<span data-ttu-id="aef50-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="aef50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aef50-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aef50-108">Attributes</span></span>

<span data-ttu-id="aef50-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="aef50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aef50-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aef50-110">Child elements</span></span>

|<span data-ttu-id="aef50-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aef50-111">**Element**</span></span>|<span data-ttu-id="aef50-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aef50-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aef50-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="aef50-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="aef50-114">Представляет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="aef50-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aef50-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aef50-115">Parent elements</span></span>

|<span data-ttu-id="aef50-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aef50-116">**Element**</span></span>|<span data-ttu-id="aef50-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aef50-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aef50-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="aef50-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="aef50-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="aef50-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aef50-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="aef50-120">Remarks</span></span>

<span data-ttu-id="aef50-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="aef50-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aef50-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="aef50-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aef50-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aef50-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aef50-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aef50-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aef50-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aef50-125">Schema Name</span></span>  <br/> |<span data-ttu-id="aef50-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="aef50-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="aef50-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aef50-127">Validation File</span></span>  <br/> |<span data-ttu-id="aef50-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aef50-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="aef50-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aef50-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="aef50-130">См. также</span><span class="sxs-lookup"><span data-stu-id="aef50-130">See also</span></span>



- [<span data-ttu-id="aef50-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aef50-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

