---
title: UserSid
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
description: Элемент UserSid представляет форме безопасности определения дескриптора языке SDDL идентификатор безопасности пользователя в заголовке SOAP контекста сериализованных безопасности. Сериализация маркера не поддерживается.
ms.openlocfilehash: 3c72f68638f99a4ee5081517027f0834ebf65b49
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840444"
---
# <a name="usersid"></a><span data-ttu-id="72582-104">UserSid</span><span class="sxs-lookup"><span data-stu-id="72582-104">UserSid</span></span>

<span data-ttu-id="72582-105">Элемент **UserSid** представляет форме безопасности определения дескриптора языке SDDL идентификатор безопасности пользователя в заголовке SOAP контекста сериализованных безопасности.</span><span class="sxs-lookup"><span data-stu-id="72582-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="72582-106">Сериализация маркера не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72582-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="72582-107">**Строка**</span><span class="sxs-lookup"><span data-stu-id="72582-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72582-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="72582-108">Attributes and elements</span></span>

<span data-ttu-id="72582-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="72582-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72582-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="72582-110">Attributes</span></span>

<span data-ttu-id="72582-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="72582-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72582-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="72582-112">Child elements</span></span>

<span data-ttu-id="72582-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="72582-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72582-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="72582-114">Parent elements</span></span>

|<span data-ttu-id="72582-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="72582-115">**Element**</span></span>|<span data-ttu-id="72582-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="72582-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72582-117">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="72582-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="72582-118">Используется в заголовке SOAP для сериализации маркера проверки подлинности сервер сервер.</span><span class="sxs-lookup"><span data-stu-id="72582-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72582-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="72582-119">Text value</span></span>

<span data-ttu-id="72582-120">Текстовое значение представляет идентификатор безопасности пользователя.</span><span class="sxs-lookup"><span data-stu-id="72582-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="72582-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="72582-121">Remarks</span></span>

<span data-ttu-id="72582-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="72582-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72582-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="72582-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72582-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="72582-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72582-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="72582-125">Schema Name</span></span>  <br/> |<span data-ttu-id="72582-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="72582-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="72582-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="72582-127">Validation File</span></span>  <br/> |<span data-ttu-id="72582-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="72582-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72582-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="72582-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="72582-130">False</span><span class="sxs-lookup"><span data-stu-id="72582-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72582-131">См. также</span><span class="sxs-lookup"><span data-stu-id="72582-131">See also</span></span>



- [<span data-ttu-id="72582-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="72582-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

