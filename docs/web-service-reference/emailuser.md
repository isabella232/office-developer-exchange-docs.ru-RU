---
title: Свойства emailuser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc8133ff-c34e-4921-bb56-06e79aee0a8a
description: Элемент свойства emailuser указывает получателя электронной почты.
ms.openlocfilehash: e724b3996d37a42527ec1183cef9bb6b312b8c93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762324"
---
# <a name="emailuser"></a><span data-ttu-id="fb37a-103">Свойства emailuser</span><span class="sxs-lookup"><span data-stu-id="fb37a-103">EmailUser</span></span>

<span data-ttu-id="fb37a-104">Элемент **Свойства emailuser** указывает получателя электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fb37a-104">The **EmailUser** element specifies an email recipient.</span></span> 
  
```XML
<EmailUser>
    <Name/>
    <UserId/>
</EmailUser>
```

 <span data-ttu-id="fb37a-105">**емаилусертипе**</span><span class="sxs-lookup"><span data-stu-id="fb37a-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb37a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fb37a-106">Attributes and elements</span></span>

<span data-ttu-id="fb37a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fb37a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb37a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fb37a-108">Attributes</span></span>

<span data-ttu-id="fb37a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fb37a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb37a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fb37a-110">Child elements</span></span>

|<span data-ttu-id="fb37a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fb37a-111">**Element**</span></span>|<span data-ttu-id="fb37a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb37a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb37a-113">Имя (строка)</span><span class="sxs-lookup"><span data-stu-id="fb37a-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="fb37a-114">Задает имя или ключ уточнения поиска или имя пользователя электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fb37a-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="fb37a-115">UserId (строка)</span><span class="sxs-lookup"><span data-stu-id="fb37a-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="fb37a-116">Указывает идентификатор пользователя электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fb37a-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb37a-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fb37a-117">Parent elements</span></span>

|<span data-ttu-id="fb37a-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fb37a-118">**Element**</span></span>|<span data-ttu-id="fb37a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb37a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb37a-120">'</span><span class="sxs-lookup"><span data-stu-id="fb37a-120">Attendees</span></span>](attendees.md) <br/> |<span data-ttu-id="fb37a-121">Указывает получателей приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="fb37a-121">Specifies the recipients of an invitation to a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fb37a-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="fb37a-122">Remarks</span></span>

<span data-ttu-id="fb37a-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fb37a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fb37a-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb37a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb37a-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fb37a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb37a-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fb37a-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb37a-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fb37a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="fb37a-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="fb37a-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="fb37a-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fb37a-129">Validation File</span></span>  <br/> |<span data-ttu-id="fb37a-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fb37a-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb37a-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fb37a-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fb37a-132">См. также</span><span class="sxs-lookup"><span data-stu-id="fb37a-132">See also</span></span>



- [<span data-ttu-id="fb37a-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fb37a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

