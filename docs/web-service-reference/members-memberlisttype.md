---
title: Members (Мемберлисттипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Members
api_type:
- schema
ms.assetid: cbd38049-2ef7-40bf-9bec-0469af0f58ec
description: Элемент Members предоставляет список членов для списка рассылки.
ms.openlocfilehash: 8cf9ed7a64a908614ce7be30a9bef631739fcebf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834439"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="99a59-103">Members (Мемберлисттипе)</span><span class="sxs-lookup"><span data-stu-id="99a59-103">Members (MemberListType)</span></span>

<span data-ttu-id="99a59-104">Элемент **Members** предоставляет список членов для списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="99a59-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="99a59-105">**мемберлисттипе**</span><span class="sxs-lookup"><span data-stu-id="99a59-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="99a59-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="99a59-106">Attributes and elements</span></span>

<span data-ttu-id="99a59-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="99a59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99a59-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="99a59-108">Attributes</span></span>

<span data-ttu-id="99a59-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="99a59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99a59-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="99a59-110">Child elements</span></span>

|<span data-ttu-id="99a59-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99a59-111">**Element**</span></span>|<span data-ttu-id="99a59-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99a59-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99a59-113">Элемент</span><span class="sxs-lookup"><span data-stu-id="99a59-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="99a59-114">Предоставляет идентификатор для полностью разрешенного адреса электронной почты, а также состояние этого адреса на сервере.</span><span class="sxs-lookup"><span data-stu-id="99a59-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="99a59-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="99a59-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="99a59-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="99a59-116">Parent elements</span></span>

|<span data-ttu-id="99a59-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99a59-117">**Element**</span></span>|<span data-ttu-id="99a59-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99a59-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99a59-119">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="99a59-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="99a59-120">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="99a59-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="99a59-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="99a59-121">Remarks</span></span>

<span data-ttu-id="99a59-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="99a59-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99a59-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="99a59-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99a59-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="99a59-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99a59-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="99a59-125">Schema Name</span></span>  <br/> |<span data-ttu-id="99a59-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="99a59-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="99a59-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="99a59-127">Validation File</span></span>  <br/> |<span data-ttu-id="99a59-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="99a59-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99a59-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="99a59-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="99a59-130">False</span><span class="sxs-lookup"><span data-stu-id="99a59-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99a59-131">См. также</span><span class="sxs-lookup"><span data-stu-id="99a59-131">See also</span></span>

- [<span data-ttu-id="99a59-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="99a59-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

