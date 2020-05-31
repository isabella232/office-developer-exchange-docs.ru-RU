---
title: О.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserSid
api_type:
- schema
ms.assetid: f8a0dcd9-8564-4e35-b307-c5d2761b48d8
description: Элемент "код возврата" представляет форму SDDL идентификатора безопасности пользователя в заголовке SOAP сериализованного контекста безопасности. Сериализация маркеров не поддерживается.
ms.openlocfilehash: 3c72f68638f99a4ee5081517027f0834ebf65b49
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840444"
---
# <a name="usersid"></a><span data-ttu-id="c9e00-104">О.</span><span class="sxs-lookup"><span data-stu-id="c9e00-104">UserSid</span></span>

<span data-ttu-id="c9e00-105">Элемент **"код возврата" представляет** форму SDDL идентификатора безопасности пользователя в заголовке SOAP сериализованного контекста безопасности.</span><span class="sxs-lookup"><span data-stu-id="c9e00-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="c9e00-106">Сериализация маркеров не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9e00-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="c9e00-107">**String**</span><span class="sxs-lookup"><span data-stu-id="c9e00-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9e00-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c9e00-108">Attributes and elements</span></span>

<span data-ttu-id="c9e00-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c9e00-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9e00-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c9e00-110">Attributes</span></span>

<span data-ttu-id="c9e00-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9e00-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9e00-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c9e00-112">Child elements</span></span>

<span data-ttu-id="c9e00-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9e00-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9e00-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c9e00-114">Parent elements</span></span>

|<span data-ttu-id="c9e00-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9e00-115">**Element**</span></span>|<span data-ttu-id="c9e00-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9e00-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9e00-117">сериализедсекуритиконтекст</span><span class="sxs-lookup"><span data-stu-id="c9e00-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="c9e00-118">Используется в заголовке SOAP для сериализации маркеров при проверке подлинности "сервер — сервер".</span><span class="sxs-lookup"><span data-stu-id="c9e00-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9e00-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c9e00-119">Text value</span></span>

<span data-ttu-id="c9e00-120">Текстовое значение представляет идентификатор безопасности пользователя.</span><span class="sxs-lookup"><span data-stu-id="c9e00-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c9e00-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="c9e00-121">Remarks</span></span>

<span data-ttu-id="c9e00-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c9e00-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9e00-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c9e00-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9e00-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c9e00-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9e00-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c9e00-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c9e00-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c9e00-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9e00-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c9e00-127">Validation File</span></span>  <br/> |<span data-ttu-id="c9e00-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c9e00-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9e00-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c9e00-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9e00-130">False</span><span class="sxs-lookup"><span data-stu-id="c9e00-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9e00-131">См. также</span><span class="sxs-lookup"><span data-stu-id="c9e00-131">See also</span></span>



- [<span data-ttu-id="c9e00-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c9e00-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

