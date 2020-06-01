---
title: Токентипе (Клиентакцесстокентипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: Элемент Токентипе определяет тип маркера клиентского доступа, который будет возвращен в ответе GetClientAccessToken.
ms.openlocfilehash: 49ba2973967b12396e0c7f56129c89c40ccbcf97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466054"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="b7339-103">Токентипе (Клиентакцесстокентипе)</span><span class="sxs-lookup"><span data-stu-id="b7339-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="b7339-104">Элемент **токентипе** определяет тип маркера клиентского доступа, который будет возвращен в ответе **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="b7339-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="b7339-105">**клиентакцесстокентипетипе**</span><span class="sxs-lookup"><span data-stu-id="b7339-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7339-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b7339-106">Attributes and elements</span></span>

<span data-ttu-id="b7339-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b7339-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7339-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b7339-108">Attributes</span></span>

<span data-ttu-id="b7339-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b7339-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7339-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b7339-110">Child elements</span></span>

<span data-ttu-id="b7339-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b7339-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7339-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b7339-112">Parent elements</span></span>

<span data-ttu-id="b7339-113">[Токенрекуест](tokenrequest.md)  |  [Маркер (клиентакцесстокентипе)](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="b7339-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b7339-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b7339-114">Text value</span></span>

<span data-ttu-id="b7339-115">Текстовое значение **каллеридентити** означает, что возвращается маркер доступа клиента идентификации звонящего.</span><span class="sxs-lookup"><span data-stu-id="b7339-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="b7339-116">Текстовое значение **екстенсионкаллбакк** указывает на то, что маркер доступа клиента обратного вызова для расширения возвращается.</span><span class="sxs-lookup"><span data-stu-id="b7339-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="b7339-117">Текстовое значение **скопедтокен** указывает на то, что маркер клиентского доступа является маркером с областью действия.</span><span class="sxs-lookup"><span data-stu-id="b7339-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b7339-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="b7339-118">Remarks</span></span>

<span data-ttu-id="b7339-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b7339-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b7339-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7339-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7339-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b7339-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7339-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b7339-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b7339-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b7339-123">Schema name</span></span>  <br/> |<span data-ttu-id="b7339-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b7339-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="b7339-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b7339-125">Validation file</span></span>  <br/> |<span data-ttu-id="b7339-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b7339-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b7339-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b7339-127">Can be empty</span></span>  <br/> |<span data-ttu-id="b7339-128">false</span><span class="sxs-lookup"><span data-stu-id="b7339-128">false</span></span>  <br/> |
   

