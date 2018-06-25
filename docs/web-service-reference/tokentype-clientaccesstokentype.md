---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: Элемент TokenType определяет тип маркера доступа клиента, возвращаемого в ответе GetClientAccessToken.
ms.openlocfilehash: c9adb60acf76fefebd58e2fd3bc899332a63dbee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840213"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="c45e0-103">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="c45e0-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="c45e0-104">Элемент **TokenType** определяет тип маркера доступа клиента, возвращаемого в ответе **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="c45e0-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="c45e0-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="c45e0-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c45e0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c45e0-106">Attributes and elements</span></span>

<span data-ttu-id="c45e0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c45e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c45e0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c45e0-108">Attributes</span></span>

<span data-ttu-id="c45e0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c45e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c45e0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c45e0-110">Child elements</span></span>

<span data-ttu-id="c45e0-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c45e0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c45e0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c45e0-112">Parent elements</span></span>

<span data-ttu-id="c45e0-113">[TokenRequest](tokenrequest.md) | [маркера (ClientAccessTokenType)](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="c45e0-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c45e0-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c45e0-114">Text value</span></span>

<span data-ttu-id="c45e0-115">Текстовое значение **CallerIdentity** означает, что возвращаются маркера доступа клиента удостоверения вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="c45e0-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="c45e0-116">Текстовое значение **ExtensionCallback** указывает, что возвращается маркер расширение обратного вызова клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c45e0-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="c45e0-117">Текстовое значение **ScopedToken** указывает, что маркер доступа клиента маркер заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c45e0-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c45e0-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="c45e0-118">Remarks</span></span>

<span data-ttu-id="c45e0-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c45e0-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c45e0-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c45e0-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c45e0-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c45e0-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c45e0-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c45e0-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c45e0-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c45e0-123">Schema name</span></span>  <br/> |<span data-ttu-id="c45e0-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c45e0-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="c45e0-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c45e0-125">Validation file</span></span>  <br/> |<span data-ttu-id="c45e0-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c45e0-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c45e0-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c45e0-127">Can be empty</span></span>  <br/> |<span data-ttu-id="c45e0-128">Нет</span><span class="sxs-lookup"><span data-stu-id="c45e0-128">false</span></span>  <br/> |
   

