---
title: Почтовый ящик (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4ad59e5b-4047-4c34-a318-ca06c31d3de8
description: Элемент почтовых ящиков содержит адрес электронной почты пользователя, чтобы обнаружить.
ms.openlocfilehash: b98397dadf8c467031eb8febe9732d4e426372e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834253"
---
# <a name="mailbox-soap"></a><span data-ttu-id="5420a-103">Почтовый ящик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5420a-103">Mailbox (SOAP)</span></span>

<span data-ttu-id="5420a-104">Элемент **почтовых ящиков** содержит адрес электронной почты пользователя, чтобы обнаружить.</span><span class="sxs-lookup"><span data-stu-id="5420a-104">The **Mailbox** element contains the e-mail address of the user to be discovered.</span></span> 
  
```XML
<Mailbox/>
```

<span data-ttu-id="5420a-105">**string**</span><span class="sxs-lookup"><span data-stu-id="5420a-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5420a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5420a-106">Attributes and elements</span></span>

<span data-ttu-id="5420a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5420a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5420a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5420a-108">Attributes</span></span>

<span data-ttu-id="5420a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5420a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5420a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5420a-110">Child elements</span></span>

<span data-ttu-id="5420a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5420a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5420a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5420a-112">Parent elements</span></span>

|<span data-ttu-id="5420a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5420a-113">**Element**</span></span>|<span data-ttu-id="5420a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5420a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5420a-115">Пользователь (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5420a-115">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="5420a-116">Представляет идентификатор одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5420a-116">Represents the identity of a single user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5420a-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5420a-117">Text value</span></span>

<span data-ttu-id="5420a-118">Текстовое значение элемента **почтового ящика** представляет собой адрес электронной почты пользователя для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="5420a-118">The text value of the **Mailbox** element is the e-mail address of the user to be discovered.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5420a-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5420a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5420a-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5420a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5420a-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5420a-121">Schema Name</span></span>  <br/> |<span data-ttu-id="5420a-122">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="5420a-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5420a-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5420a-123">Validation File</span></span>  <br/> |<span data-ttu-id="5420a-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5420a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5420a-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5420a-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="5420a-126">True</span><span class="sxs-lookup"><span data-stu-id="5420a-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5420a-127">См. также</span><span class="sxs-lookup"><span data-stu-id="5420a-127">See also</span></span>

- [<span data-ttu-id="5420a-128">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5420a-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

