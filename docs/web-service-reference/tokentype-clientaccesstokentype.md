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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840213"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="b4af1-103">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="b4af1-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="b4af1-104">Элемент **TokenType** определяет тип маркера доступа клиента, возвращаемого в ответе **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="b4af1-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="b4af1-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="b4af1-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4af1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b4af1-106">Attributes and elements</span></span>

<span data-ttu-id="b4af1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b4af1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4af1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4af1-108">Attributes</span></span>

<span data-ttu-id="b4af1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b4af1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4af1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b4af1-110">Child elements</span></span>

<span data-ttu-id="b4af1-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b4af1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b4af1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b4af1-112">Parent elements</span></span>

<span data-ttu-id="b4af1-113">[TokenRequest](tokenrequest.md) | [маркера (ClientAccessTokenType)](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="b4af1-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b4af1-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b4af1-114">Text value</span></span>

<span data-ttu-id="b4af1-115">Текстовое значение **CallerIdentity** означает, что возвращаются маркера доступа клиента удостоверения вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="b4af1-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="b4af1-116">Текстовое значение **ExtensionCallback** указывает, что возвращается маркер расширение обратного вызова клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b4af1-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="b4af1-117">Текстовое значение **ScopedToken** указывает, что маркер доступа клиента маркер заданной областью.</span><span class="sxs-lookup"><span data-stu-id="b4af1-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b4af1-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="b4af1-118">Remarks</span></span>

<span data-ttu-id="b4af1-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b4af1-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b4af1-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4af1-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4af1-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b4af1-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4af1-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b4af1-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4af1-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b4af1-123">Schema name</span></span>  <br/> |<span data-ttu-id="b4af1-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b4af1-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4af1-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b4af1-125">Validation file</span></span>  <br/> |<span data-ttu-id="b4af1-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b4af1-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4af1-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b4af1-127">Can be empty</span></span>  <br/> |<span data-ttu-id="b4af1-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b4af1-128">false</span></span>  <br/> |
   

