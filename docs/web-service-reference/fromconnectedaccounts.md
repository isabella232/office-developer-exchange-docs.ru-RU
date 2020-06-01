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
ms.openlocfilehash: 159ae064827c2f9c2b470580ad5457264e8dae93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464051"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="149a3-103">фромконнектедаккаунтс</span><span class="sxs-lookup"><span data-stu-id="149a3-103">FromConnectedAccounts</span></span>

<span data-ttu-id="149a3-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **FromConnectedAccounts** представляет имена учетных записей электронной почты, из которых нужно были сводный в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="149a3-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="149a3-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="149a3-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="149a3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="149a3-106">Attributes and elements</span></span>

<span data-ttu-id="149a3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="149a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="149a3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="149a3-108">Attributes</span></span>

<span data-ttu-id="149a3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="149a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="149a3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="149a3-110">Child elements</span></span>

|<span data-ttu-id="149a3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="149a3-111">**Element**</span></span>|<span data-ttu-id="149a3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="149a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="149a3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="149a3-113">String</span></span>](string.md) <br/> |<span data-ttu-id="149a3-114">Представляет собой имя учетной записи электронной почты, из которой нужно были сводный в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="149a3-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="149a3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="149a3-115">Parent elements</span></span>

|<span data-ttu-id="149a3-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="149a3-116">**Element**</span></span>|<span data-ttu-id="149a3-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="149a3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="149a3-118">Условия</span><span class="sxs-lookup"><span data-stu-id="149a3-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="149a3-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="149a3-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="149a3-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="149a3-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="149a3-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="149a3-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="149a3-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="149a3-122">Text value</span></span>

<span data-ttu-id="149a3-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="149a3-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="149a3-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="149a3-124">Remarks</span></span>

<span data-ttu-id="149a3-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="149a3-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="149a3-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="149a3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="149a3-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="149a3-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="149a3-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="149a3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="149a3-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="149a3-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="149a3-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="149a3-130">Validation File</span></span>  <br/> |<span data-ttu-id="149a3-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="149a3-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="149a3-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="149a3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="149a3-133">True</span><span class="sxs-lookup"><span data-stu-id="149a3-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="149a3-134">См. также</span><span class="sxs-lookup"><span data-stu-id="149a3-134">See also</span></span>



- [<span data-ttu-id="149a3-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="149a3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

