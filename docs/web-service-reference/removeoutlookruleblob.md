---
title: ремовеаутлукрулеблоб
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: Элемент Ремовеаутлукрулеблоб указывает, следует ли удалить большой двоичный объект правила Microsoft Outlook.
ms.openlocfilehash: b4202ab52bf16d1ad1546ec963cd8b9dacd2bd63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467671"
---
# <a name="removeoutlookruleblob"></a><span data-ttu-id="d0e99-103">ремовеаутлукрулеблоб</span><span class="sxs-lookup"><span data-stu-id="d0e99-103">RemoveOutlookRuleBlob</span></span>

<span data-ttu-id="d0e99-104">Элемент **ремовеаутлукрулеблоб** указывает, следует ли удалить большой двоичный объект правила Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="d0e99-104">The **RemoveOutlookRuleBlob** element indicates whether to remove the Microsoft Outlook rule blob.</span></span> 
  
[<span data-ttu-id="d0e99-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d0e99-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="d0e99-106">ремовеаутлукрулеблоб</span><span class="sxs-lookup"><span data-stu-id="d0e99-106">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 <span data-ttu-id="d0e99-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d0e99-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0e99-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d0e99-108">Attributes and elements</span></span>

<span data-ttu-id="d0e99-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d0e99-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0e99-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d0e99-110">Attributes</span></span>

<span data-ttu-id="d0e99-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d0e99-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0e99-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d0e99-112">Child elements</span></span>

<span data-ttu-id="d0e99-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d0e99-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d0e99-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d0e99-114">Parent elements</span></span>

|<span data-ttu-id="d0e99-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d0e99-115">**Element**</span></span>|<span data-ttu-id="d0e99-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0e99-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0e99-117">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d0e99-117">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="d0e99-118">Определяет запрос на обновление правил папки "Входящие" в почтовом ящике в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="d0e99-118">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0e99-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d0e99-119">Text value</span></span>

<span data-ttu-id="d0e99-120">Текстовое значение **true** указывает, что большой двоичный объект правила Outlook должен быть удален.</span><span class="sxs-lookup"><span data-stu-id="d0e99-120">A text value of **true** indicates that the Outlook rule blob should be removed.</span></span> <span data-ttu-id="d0e99-121">Текстовое значение **false** указывает, что большой двоичный объект правила Outlook не должен удаляться.</span><span class="sxs-lookup"><span data-stu-id="d0e99-121">A text value of **false** indicates that the Outlook rule blob should not be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d0e99-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="d0e99-122">Remarks</span></span>

<span data-ttu-id="d0e99-123">Установите для этого элемента **значение true** , чтобы разрешить обновление правила для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="d0e99-123">Set this element to **true** to allow for an Inbox rule update.</span></span> 
  
<span data-ttu-id="d0e99-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0e99-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0e99-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d0e99-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0e99-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d0e99-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0e99-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d0e99-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d0e99-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d0e99-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="d0e99-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d0e99-129">Validation File</span></span>  <br/> |<span data-ttu-id="d0e99-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d0e99-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0e99-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d0e99-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0e99-132">True</span><span class="sxs-lookup"><span data-stu-id="d0e99-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0e99-133">См. также</span><span class="sxs-lookup"><span data-stu-id="d0e99-133">See also</span></span>



[<span data-ttu-id="d0e99-134">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d0e99-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="d0e99-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d0e99-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

