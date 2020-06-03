---
title: Emails3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f4dc589-4530-4a35-b2a6-0c83cac23637
description: Элемент Emails3 указывает массив значений Емаиладдрессаттрибутедвалуе и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 0505b0ea248a3ab2de7ec18a344fa57651f84cca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460724"
---
# <a name="emails3"></a><span data-ttu-id="6769c-103">Emails3</span><span class="sxs-lookup"><span data-stu-id="6769c-103">Emails3</span></span>

<span data-ttu-id="6769c-104">Элемент **Emails3** указывает массив значений **емаиладдрессаттрибутедвалуе** и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6769c-104">The **Emails3** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails3>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails3>
```

 <span data-ttu-id="6769c-105">**аррайофемаиладдрессаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="6769c-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6769c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6769c-106">Attributes and elements</span></span>

<span data-ttu-id="6769c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6769c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6769c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6769c-108">Attributes</span></span>

<span data-ttu-id="6769c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6769c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6769c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6769c-110">Child elements</span></span>

|<span data-ttu-id="6769c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6769c-111">**Element**</span></span>|<span data-ttu-id="6769c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6769c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6769c-113">емаиладдрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="6769c-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="6769c-114">Указывает экземпляр массива адресов электронной почты и связанные с ними атрибуты.</span><span class="sxs-lookup"><span data-stu-id="6769c-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6769c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6769c-115">Parent elements</span></span>

|<span data-ttu-id="6769c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6769c-116">**Element**</span></span>|<span data-ttu-id="6769c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6769c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6769c-118">Роль</span><span class="sxs-lookup"><span data-stu-id="6769c-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="6769c-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="6769c-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6769c-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="6769c-120">Remarks</span></span>

<span data-ttu-id="6769c-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6769c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6769c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6769c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6769c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6769c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6769c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6769c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6769c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6769c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6769c-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="6769c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6769c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6769c-127">Validation File</span></span>  <br/> |<span data-ttu-id="6769c-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6769c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6769c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6769c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6769c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="6769c-130">See also</span></span>



- [<span data-ttu-id="6769c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6769c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

