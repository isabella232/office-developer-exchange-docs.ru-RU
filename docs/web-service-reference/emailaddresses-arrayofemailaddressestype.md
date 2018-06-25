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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762292"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="ce4d7-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="ce4d7-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="ce4d7-104">Элемент **EmailAddresses** указывает массив всех адресов электронной почты, связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce4d7-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="ce4d7-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="ce4d7-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce4d7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ce4d7-106">Attributes and elements</span></span>

<span data-ttu-id="ce4d7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ce4d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce4d7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ce4d7-108">Attributes</span></span>

<span data-ttu-id="ce4d7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ce4d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce4d7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ce4d7-110">Child elements</span></span>

|<span data-ttu-id="ce4d7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce4d7-111">**Element**</span></span>|<span data-ttu-id="ce4d7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce4d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce4d7-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ce4d7-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="ce4d7-114">Представляет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="ce4d7-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce4d7-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ce4d7-115">Parent elements</span></span>

|<span data-ttu-id="ce4d7-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce4d7-116">**Element**</span></span>|<span data-ttu-id="ce4d7-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce4d7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce4d7-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="ce4d7-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ce4d7-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="ce4d7-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce4d7-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="ce4d7-120">Remarks</span></span>

<span data-ttu-id="ce4d7-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ce4d7-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ce4d7-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce4d7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce4d7-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ce4d7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce4d7-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ce4d7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce4d7-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ce4d7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ce4d7-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="ce4d7-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ce4d7-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ce4d7-127">Validation File</span></span>  <br/> |<span data-ttu-id="ce4d7-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ce4d7-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce4d7-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ce4d7-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ce4d7-130">См. также</span><span class="sxs-lookup"><span data-stu-id="ce4d7-130">See also</span></span>



- [<span data-ttu-id="ce4d7-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce4d7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

