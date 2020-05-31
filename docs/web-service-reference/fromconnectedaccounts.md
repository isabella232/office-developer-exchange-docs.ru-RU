---
title: фромконнектедаккаунтс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromConnectedAccounts
api_type:
- schema
ms.assetid: d4d7ddd7-078d-4f1a-a26b-22dce0c49f3a
description: Элемент FromConnectedAccounts представляет имена учетных записей электронной почты, из которых нужно были сводный в порядке для условие или исключение для применения входящих сообщений.
ms.openlocfilehash: 426e81bbbe96fb5fb4b36506438dc4af4f560eef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762662"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="e18a6-103">фромконнектедаккаунтс</span><span class="sxs-lookup"><span data-stu-id="e18a6-103">FromConnectedAccounts</span></span>

<span data-ttu-id="e18a6-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **FromConnectedAccounts** представляет имена учетных записей электронной почты, из которых нужно были сводный в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="e18a6-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="e18a6-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="e18a6-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e18a6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e18a6-106">Attributes and elements</span></span>

<span data-ttu-id="e18a6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e18a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e18a6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e18a6-108">Attributes</span></span>

<span data-ttu-id="e18a6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e18a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e18a6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e18a6-110">Child elements</span></span>

|<span data-ttu-id="e18a6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e18a6-111">**Element**</span></span>|<span data-ttu-id="e18a6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e18a6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e18a6-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e18a6-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e18a6-114">Представляет собой имя учетной записи электронной почты, из которой нужно были сводный в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="e18a6-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e18a6-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e18a6-115">Parent elements</span></span>

|<span data-ttu-id="e18a6-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e18a6-116">**Element**</span></span>|<span data-ttu-id="e18a6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e18a6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e18a6-118">Условия</span><span class="sxs-lookup"><span data-stu-id="e18a6-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e18a6-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="e18a6-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e18a6-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="e18a6-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e18a6-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="e18a6-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e18a6-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e18a6-122">Text value</span></span>

<span data-ttu-id="e18a6-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="e18a6-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e18a6-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="e18a6-124">Remarks</span></span>

<span data-ttu-id="e18a6-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e18a6-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e18a6-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e18a6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e18a6-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e18a6-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e18a6-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e18a6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e18a6-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e18a6-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e18a6-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e18a6-130">Validation File</span></span>  <br/> |<span data-ttu-id="e18a6-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e18a6-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e18a6-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e18a6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e18a6-133">True</span><span class="sxs-lookup"><span data-stu-id="e18a6-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e18a6-134">См. также</span><span class="sxs-lookup"><span data-stu-id="e18a6-134">See also</span></span>



- [<span data-ttu-id="e18a6-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e18a6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

