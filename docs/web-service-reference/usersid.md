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
ms.openlocfilehash: b8ee51b1998546fc4ab14bd3666192ae63c8dba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462019"
---
# <a name="usersid"></a><span data-ttu-id="19fcb-104">О.</span><span class="sxs-lookup"><span data-stu-id="19fcb-104">UserSid</span></span>

<span data-ttu-id="19fcb-105">Элемент **"код возврата" представляет** форму SDDL идентификатора безопасности пользователя в заголовке SOAP сериализованного контекста безопасности.</span><span class="sxs-lookup"><span data-stu-id="19fcb-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="19fcb-106">Сериализация маркеров не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fcb-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="19fcb-107">**String**</span><span class="sxs-lookup"><span data-stu-id="19fcb-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19fcb-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="19fcb-108">Attributes and elements</span></span>

<span data-ttu-id="19fcb-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="19fcb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19fcb-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="19fcb-110">Attributes</span></span>

<span data-ttu-id="19fcb-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="19fcb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19fcb-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="19fcb-112">Child elements</span></span>

<span data-ttu-id="19fcb-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="19fcb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19fcb-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="19fcb-114">Parent elements</span></span>

|<span data-ttu-id="19fcb-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="19fcb-115">**Element**</span></span>|<span data-ttu-id="19fcb-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="19fcb-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19fcb-117">сериализедсекуритиконтекст</span><span class="sxs-lookup"><span data-stu-id="19fcb-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="19fcb-118">Используется в заголовке SOAP для сериализации маркеров при проверке подлинности "сервер — сервер".</span><span class="sxs-lookup"><span data-stu-id="19fcb-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19fcb-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="19fcb-119">Text value</span></span>

<span data-ttu-id="19fcb-120">Текстовое значение представляет идентификатор безопасности пользователя.</span><span class="sxs-lookup"><span data-stu-id="19fcb-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19fcb-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="19fcb-121">Remarks</span></span>

<span data-ttu-id="19fcb-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="19fcb-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19fcb-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="19fcb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19fcb-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="19fcb-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19fcb-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="19fcb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="19fcb-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="19fcb-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="19fcb-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="19fcb-127">Validation File</span></span>  <br/> |<span data-ttu-id="19fcb-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="19fcb-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19fcb-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="19fcb-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="19fcb-130">False</span><span class="sxs-lookup"><span data-stu-id="19fcb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19fcb-131">См. также</span><span class="sxs-lookup"><span data-stu-id="19fcb-131">See also</span></span>



- [<span data-ttu-id="19fcb-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="19fcb-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

