---
title: EmailAddresses (Аррайофемаиладдрессестипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95084659-aa5a-4bac-8977-00db3b87883e
description: Элемент EmailAddresses указывает массив всех адресов электронной почты связанного пользователя.
ms.openlocfilehash: e6132e9ef4ed13ea2546783f65d184fafeed5530
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463421"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="f9585-103">EmailAddresses (Аррайофемаиладдрессестипе)</span><span class="sxs-lookup"><span data-stu-id="f9585-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="f9585-104">Элемент **EmailAddresses** указывает массив всех адресов электронной почты связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f9585-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="f9585-105">**аррайофемаиладдрессестипе**</span><span class="sxs-lookup"><span data-stu-id="f9585-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9585-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f9585-106">Attributes and elements</span></span>

<span data-ttu-id="f9585-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f9585-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9585-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f9585-108">Attributes</span></span>

<span data-ttu-id="f9585-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f9585-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9585-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f9585-110">Child elements</span></span>

|<span data-ttu-id="f9585-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f9585-111">**Element**</span></span>|<span data-ttu-id="f9585-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f9585-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9585-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f9585-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="f9585-114">Представляет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="f9585-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9585-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f9585-115">Parent elements</span></span>

|<span data-ttu-id="f9585-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f9585-116">**Element**</span></span>|<span data-ttu-id="f9585-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f9585-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9585-118">Роль</span><span class="sxs-lookup"><span data-stu-id="f9585-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f9585-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="f9585-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9585-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="f9585-120">Remarks</span></span>

<span data-ttu-id="f9585-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f9585-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f9585-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9585-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9585-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f9585-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9585-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f9585-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9585-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f9585-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f9585-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="f9585-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f9585-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f9585-127">Validation File</span></span>  <br/> |<span data-ttu-id="f9585-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f9585-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9585-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f9585-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f9585-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f9585-130">See also</span></span>



- [<span data-ttu-id="f9585-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f9585-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

