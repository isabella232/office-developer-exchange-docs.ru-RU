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
ms.openlocfilehash: 2cdfb81dfbc223db365d49ed44d4893339eb4653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462432"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="6047e-103">Members (Мемберлисттипе)</span><span class="sxs-lookup"><span data-stu-id="6047e-103">Members (MemberListType)</span></span>

<span data-ttu-id="6047e-104">Элемент **Members** предоставляет список членов для списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="6047e-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="6047e-105">**мемберлисттипе**</span><span class="sxs-lookup"><span data-stu-id="6047e-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6047e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6047e-106">Attributes and elements</span></span>

<span data-ttu-id="6047e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6047e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6047e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6047e-108">Attributes</span></span>

<span data-ttu-id="6047e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6047e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6047e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6047e-110">Child elements</span></span>

|<span data-ttu-id="6047e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6047e-111">**Element**</span></span>|<span data-ttu-id="6047e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6047e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6047e-113">Элемент</span><span class="sxs-lookup"><span data-stu-id="6047e-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6047e-114">Предоставляет идентификатор для полностью разрешенного адреса электронной почты, а также состояние этого адреса на сервере.</span><span class="sxs-lookup"><span data-stu-id="6047e-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="6047e-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6047e-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6047e-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6047e-116">Parent elements</span></span>

|<span data-ttu-id="6047e-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6047e-117">**Element**</span></span>|<span data-ttu-id="6047e-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6047e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6047e-119">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="6047e-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="6047e-120">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="6047e-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6047e-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="6047e-121">Remarks</span></span>

<span data-ttu-id="6047e-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6047e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6047e-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6047e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6047e-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6047e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6047e-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6047e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6047e-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6047e-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="6047e-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6047e-127">Validation File</span></span>  <br/> |<span data-ttu-id="6047e-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6047e-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6047e-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6047e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="6047e-130">False</span><span class="sxs-lookup"><span data-stu-id="6047e-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6047e-131">См. также</span><span class="sxs-lookup"><span data-stu-id="6047e-131">See also</span></span>

- [<span data-ttu-id="6047e-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6047e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

