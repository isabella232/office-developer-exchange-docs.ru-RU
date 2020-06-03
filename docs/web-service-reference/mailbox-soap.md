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
description: Элемент Mailbox содержит адрес электронной почты пользователя, которого требуется обнаружить.
ms.openlocfilehash: e050cd9d3ca4a2d2450f315f1eedd3862328d096
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467286"
---
# <a name="mailbox-soap"></a><span data-ttu-id="746d9-103">Почтовый ящик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="746d9-103">Mailbox (SOAP)</span></span>

<span data-ttu-id="746d9-104">Элемент **Mailbox** содержит адрес электронной почты пользователя, которого требуется обнаружить.</span><span class="sxs-lookup"><span data-stu-id="746d9-104">The **Mailbox** element contains the e-mail address of the user to be discovered.</span></span> 
  
```XML
<Mailbox/>
```

<span data-ttu-id="746d9-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="746d9-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="746d9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="746d9-106">Attributes and elements</span></span>

<span data-ttu-id="746d9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="746d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="746d9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="746d9-108">Attributes</span></span>

<span data-ttu-id="746d9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="746d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="746d9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="746d9-110">Child elements</span></span>

<span data-ttu-id="746d9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="746d9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="746d9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="746d9-112">Parent elements</span></span>

|<span data-ttu-id="746d9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="746d9-113">**Element**</span></span>|<span data-ttu-id="746d9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="746d9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="746d9-115">Пользователь (SOAP)</span><span class="sxs-lookup"><span data-stu-id="746d9-115">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="746d9-116">Представляет идентификатор одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="746d9-116">Represents the identity of a single user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="746d9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="746d9-117">Text value</span></span>

<span data-ttu-id="746d9-118">Текстовое значение элемента **Mailbox** — это адрес электронной почты пользователя, который будет обнаружен.</span><span class="sxs-lookup"><span data-stu-id="746d9-118">The text value of the **Mailbox** element is the e-mail address of the user to be discovered.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="746d9-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="746d9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="746d9-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="746d9-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="746d9-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="746d9-121">Schema Name</span></span>  <br/> |<span data-ttu-id="746d9-122">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="746d9-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="746d9-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="746d9-123">Validation File</span></span>  <br/> |<span data-ttu-id="746d9-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="746d9-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="746d9-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="746d9-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="746d9-126">True</span><span class="sxs-lookup"><span data-stu-id="746d9-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="746d9-127">См. также</span><span class="sxs-lookup"><span data-stu-id="746d9-127">See also</span></span>

- [<span data-ttu-id="746d9-128">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="746d9-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

