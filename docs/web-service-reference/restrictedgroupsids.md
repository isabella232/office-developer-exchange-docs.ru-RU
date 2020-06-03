---
title: рестриктедграупсидс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RestrictedGroupSids
api_type:
- schema
ms.assetid: 569ab552-5616-444a-a7f5-de366a684a34
description: Элемент Рестриктедграупсидс представляет коллекцию ограниченных групп из маркера пользователя.
ms.openlocfilehash: 739a73d2ac4bdbbee03650d035271b5c8d9ea25a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465361"
---
# <a name="restrictedgroupsids"></a><span data-ttu-id="a25f5-103">рестриктедграупсидс</span><span class="sxs-lookup"><span data-stu-id="a25f5-103">RestrictedGroupSids</span></span>

<span data-ttu-id="a25f5-104">Элемент **рестриктедграупсидс** представляет коллекцию ограниченных групп из маркера пользователя.</span><span class="sxs-lookup"><span data-stu-id="a25f5-104">The **RestrictedGroupSids** element represents a collection of restricted groups from a user's token.</span></span> 
  
```xml
<RestrictedGroupSids>
   <RestrictedGroupIdentifier/>
</RestrictedGroupSids>
```

 <span data-ttu-id="a25f5-105">**нонемптяррайофрестриктедграупидентифиерстипе**</span><span class="sxs-lookup"><span data-stu-id="a25f5-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a25f5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a25f5-106">Attributes and elements</span></span>

<span data-ttu-id="a25f5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a25f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a25f5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a25f5-108">Attributes</span></span>

<span data-ttu-id="a25f5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a25f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a25f5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a25f5-110">Child elements</span></span>

|<span data-ttu-id="a25f5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a25f5-111">**Element**</span></span>|<span data-ttu-id="a25f5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a25f5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a25f5-113">рестриктедграупидентифиер</span><span class="sxs-lookup"><span data-stu-id="a25f5-113">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="a25f5-114">Представляет идентификатор безопасности группы (SID) и атрибуты для группы с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="a25f5-114">Represents the group security identifier (SID) and attributes for a restricted group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a25f5-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a25f5-115">Parent elements</span></span>

|<span data-ttu-id="a25f5-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a25f5-116">**Element**</span></span>|<span data-ttu-id="a25f5-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a25f5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a25f5-118">сериализедсекуритиконтекст</span><span class="sxs-lookup"><span data-stu-id="a25f5-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="a25f5-119">Используется в заголовке SOAP для сериализации маркеров при проверке подлинности "сервер — сервер".</span><span class="sxs-lookup"><span data-stu-id="a25f5-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span> <span data-ttu-id="a25f5-120">Сериализация маркеров не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a25f5-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a25f5-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="a25f5-121">Remarks</span></span>

<span data-ttu-id="a25f5-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a25f5-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a25f5-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a25f5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a25f5-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a25f5-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a25f5-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a25f5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a25f5-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a25f5-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="a25f5-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a25f5-127">Validation File</span></span>  <br/> |<span data-ttu-id="a25f5-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a25f5-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a25f5-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a25f5-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="a25f5-130">False</span><span class="sxs-lookup"><span data-stu-id="a25f5-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a25f5-131">См. также</span><span class="sxs-lookup"><span data-stu-id="a25f5-131">See also</span></span>



- [<span data-ttu-id="a25f5-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a25f5-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

