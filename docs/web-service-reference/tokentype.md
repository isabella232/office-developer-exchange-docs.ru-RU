---
title: токентипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: Элемент Токентипе указывает тип маркера.
ms.openlocfilehash: a42849dce9ed0253c3c5d4d4e899367b8e105594
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459884"
---
# <a name="tokentype"></a><span data-ttu-id="58c89-103">токентипе</span><span class="sxs-lookup"><span data-stu-id="58c89-103">TokenType</span></span>

<span data-ttu-id="58c89-104">Элемент **токентипе** указывает тип маркера.</span><span class="sxs-lookup"><span data-stu-id="58c89-104">The **TokenType** element specifies the type of token.</span></span> 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 <span data-ttu-id="58c89-105">**клиентакцесстокентипетипе**</span><span class="sxs-lookup"><span data-stu-id="58c89-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58c89-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="58c89-106">Attributes and elements</span></span>

<span data-ttu-id="58c89-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="58c89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58c89-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="58c89-108">Attributes</span></span>

<span data-ttu-id="58c89-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="58c89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58c89-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="58c89-110">Child elements</span></span>

<span data-ttu-id="58c89-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="58c89-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58c89-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="58c89-112">Parent elements</span></span>

<span data-ttu-id="58c89-113">[Токенрекуест](tokenrequest.md)  |  [Token (маркер](token.md) )</span><span class="sxs-lookup"><span data-stu-id="58c89-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="58c89-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="58c89-114">Text value</span></span>

<span data-ttu-id="58c89-115">Текстовое значение элемента **токентипе** — тип маркера.</span><span class="sxs-lookup"><span data-stu-id="58c89-115">The text value of the **TokenType** element is the token type.</span></span> <span data-ttu-id="58c89-116">Текстовое значение **каллеридентити** указывает на то, что маркер является маркером удостоверения звонящего.</span><span class="sxs-lookup"><span data-stu-id="58c89-116">The text value of **CallerIdentity** indicates that the token is a caller identity token.</span></span> <span data-ttu-id="58c89-117">Текстовое значение **екстенсионкаллбакк** указывает, что маркер предназначен для обратного вызова расширения.</span><span class="sxs-lookup"><span data-stu-id="58c89-117">The text value of **ExtensionCallback** indicates that the token is for an extension callback.</span></span> <span data-ttu-id="58c89-118">Текстовое значение **скопедтокен** указывает на то, что маркер клиентского доступа является маркером с областью действия.</span><span class="sxs-lookup"><span data-stu-id="58c89-118">The text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="58c89-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="58c89-119">Remarks</span></span>

<span data-ttu-id="58c89-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="58c89-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="58c89-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="58c89-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58c89-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="58c89-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58c89-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="58c89-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58c89-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="58c89-124">Schema name</span></span>  <br/> |<span data-ttu-id="58c89-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="58c89-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="58c89-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="58c89-126">Validation file</span></span>  <br/> |<span data-ttu-id="58c89-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="58c89-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58c89-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="58c89-128">Can be empty</span></span>  <br/> |<span data-ttu-id="58c89-129">false</span><span class="sxs-lookup"><span data-stu-id="58c89-129">false</span></span>  <br/> |
   

