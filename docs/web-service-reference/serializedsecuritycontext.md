---
title: сериализедсекуритиконтекст
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
description: Элемент Сериализедсекуритиконтекст используется в заголовке протокола SOAP для сериализации маркеров при проверке подлинности "сервер-сервер". Сериализация маркеров не поддерживается.
ms.openlocfilehash: 58fea1c7f613315d59e81935561f92f318afc769
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462054"
---
# <a name="serializedsecuritycontext"></a><span data-ttu-id="c6cf4-104">сериализедсекуритиконтекст</span><span class="sxs-lookup"><span data-stu-id="c6cf4-104">SerializedSecurityContext</span></span>

<span data-ttu-id="c6cf4-105">Элемент **сериализедсекуритиконтекст** используется в заголовке протокола SOAP для сериализации маркеров при проверке подлинности "сервер-сервер".</span><span class="sxs-lookup"><span data-stu-id="c6cf4-105">The **SerializedSecurityContext** element is used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="c6cf4-106">Сериализация маркеров не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-106">Token serialization is not supported.</span></span> 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 <span data-ttu-id="c6cf4-107">**сериализедсекуритиконтексттипе**</span><span class="sxs-lookup"><span data-stu-id="c6cf4-107">**SerializedSecurityContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6cf4-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c6cf4-108">Attributes and elements</span></span>

<span data-ttu-id="c6cf4-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6cf4-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c6cf4-110">Attributes</span></span>

<span data-ttu-id="c6cf4-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6cf4-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c6cf4-112">Child elements</span></span>

|<span data-ttu-id="c6cf4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c6cf4-113">**Element**</span></span>|<span data-ttu-id="c6cf4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c6cf4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6cf4-115">О.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-115">UserSid</span></span>](usersid.md) <br/> |<span data-ttu-id="c6cf4-116">Представляет форму языка определения дескрипторов безопасности (SDDL) для идентификатора безопасности пользователя в сериализованном SOAP-заголовке контекста безопасности.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-116">Represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span>  <br/> |
|[<span data-ttu-id="c6cf4-117">граупсидс</span><span class="sxs-lookup"><span data-stu-id="c6cf4-117">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="c6cf4-118">Представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-118">Represents a collection of Active Directory directory service group object security identifiers.</span></span>  <br/> |
|[<span data-ttu-id="c6cf4-119">рестриктедграупсидс</span><span class="sxs-lookup"><span data-stu-id="c6cf4-119">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="c6cf4-120">Представляет идентификатор и атрибуты безопасности группы для группы с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-120">Represents the group security identifier and attributes for a restricted group.</span></span>  <br/> |
|[<span data-ttu-id="c6cf4-121">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="c6cf4-121">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="c6cf4-122">Представляет основной SMTP-адрес учетной записи, которая будет использоваться для авторизации "сервер-сервер".</span><span class="sxs-lookup"><span data-stu-id="c6cf4-122">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6cf4-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c6cf4-123">Parent elements</span></span>

<span data-ttu-id="c6cf4-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="c6cf4-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c6cf4-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="c6cf4-125">Remarks</span></span>

<span data-ttu-id="c6cf4-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа (CAS).</span><span class="sxs-lookup"><span data-stu-id="c6cf4-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server (CAS) role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6cf4-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c6cf4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6cf4-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c6cf4-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6cf4-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c6cf4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="c6cf4-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c6cf4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="c6cf4-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c6cf4-131">Validation File</span></span>  <br/> |<span data-ttu-id="c6cf4-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c6cf4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6cf4-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c6cf4-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6cf4-134">False</span><span class="sxs-lookup"><span data-stu-id="c6cf4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6cf4-135">См. также</span><span class="sxs-lookup"><span data-stu-id="c6cf4-135">See also</span></span>



- [<span data-ttu-id="c6cf4-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c6cf4-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c6cf4-137">Авторизация между серверами в EWS</span><span class="sxs-lookup"><span data-stu-id="c6cf4-137">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

