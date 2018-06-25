---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: Элемент SerializedSecurityContext используется в заголовке Simple Object Access Protocol (SOAP) для сериализации маркера проверки подлинности сервер сервер. Сериализация маркера не поддерживается.
ms.openlocfilehash: c5590551dc0780d918b05902e4f48fb9d1390b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835363"
---
# <a name="serializedsecuritycontext"></a><span data-ttu-id="1ba67-104">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="1ba67-104">SerializedSecurityContext</span></span>

<span data-ttu-id="1ba67-105">Элемент **SerializedSecurityContext** используется в заголовке Simple Object Access Protocol (SOAP) для сериализации маркера проверки подлинности сервер сервер.</span><span class="sxs-lookup"><span data-stu-id="1ba67-105">The **SerializedSecurityContext** element is used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="1ba67-106">Сериализация маркера не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ba67-106">Token serialization is not supported.</span></span> 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 <span data-ttu-id="1ba67-107">**SerializedSecurityContextType**</span><span class="sxs-lookup"><span data-stu-id="1ba67-107">**SerializedSecurityContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ba67-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1ba67-108">Attributes and elements</span></span>

<span data-ttu-id="1ba67-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1ba67-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ba67-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1ba67-110">Attributes</span></span>

<span data-ttu-id="1ba67-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ba67-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ba67-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1ba67-112">Child elements</span></span>

|<span data-ttu-id="1ba67-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1ba67-113">**Element**</span></span>|<span data-ttu-id="1ba67-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1ba67-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ba67-115">UserSid</span><span class="sxs-lookup"><span data-stu-id="1ba67-115">UserSid</span></span>](usersid.md) <br/> |<span data-ttu-id="1ba67-116">Представляет форме безопасности определения дескриптора языке SDDL идентификатор безопасности пользователя в заголовке SOAP контекста сериализованных безопасности.</span><span class="sxs-lookup"><span data-stu-id="1ba67-116">Represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span>  <br/> |
|[<span data-ttu-id="1ba67-117">GroupSids</span><span class="sxs-lookup"><span data-stu-id="1ba67-117">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="1ba67-118">Представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1ba67-118">Represents a collection of Active Directory directory service group object security identifiers.</span></span>  <br/> |
|[<span data-ttu-id="1ba67-119">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="1ba67-119">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="1ba67-120">Представляет идентификатор группы безопасности и атрибуты, используемые для группа с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="1ba67-120">Represents the group security identifier and attributes for a restricted group.</span></span>  <br/> |
|[<span data-ttu-id="1ba67-121">Параметр PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1ba67-121">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="1ba67-122">Представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетной записи, которое будет использоваться для проверки подлинности сервер сервер.</span><span class="sxs-lookup"><span data-stu-id="1ba67-122">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ba67-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1ba67-123">Parent elements</span></span>

<span data-ttu-id="1ba67-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ba67-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1ba67-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="1ba67-125">Remarks</span></span>

<span data-ttu-id="1ba67-126">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера (CAS) клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1ba67-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server (CAS) role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ba67-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1ba67-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ba67-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1ba67-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ba67-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1ba67-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1ba67-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1ba67-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="1ba67-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1ba67-131">Validation File</span></span>  <br/> |<span data-ttu-id="1ba67-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1ba67-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ba67-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1ba67-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ba67-134">False</span><span class="sxs-lookup"><span data-stu-id="1ba67-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ba67-135">См. также</span><span class="sxs-lookup"><span data-stu-id="1ba67-135">See also</span></span>



- [<span data-ttu-id="1ba67-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1ba67-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1ba67-137">Сервер сервер авторизации в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ba67-137">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

