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
ms.openlocfilehash: fcfee809261c7ed0a4e0d092c091841fec641e46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835201"
---
# <a name="restrictedgroupsids"></a><span data-ttu-id="575c1-103">рестриктедграупсидс</span><span class="sxs-lookup"><span data-stu-id="575c1-103">RestrictedGroupSids</span></span>

<span data-ttu-id="575c1-104">Элемент **рестриктедграупсидс** представляет коллекцию ограниченных групп из маркера пользователя.</span><span class="sxs-lookup"><span data-stu-id="575c1-104">The **RestrictedGroupSids** element represents a collection of restricted groups from a user's token.</span></span> 
  
```xml
<RestrictedGroupSids>
   <RestrictedGroupIdentifier/>
</RestrictedGroupSids>
```

 <span data-ttu-id="575c1-105">**нонемптяррайофрестриктедграупидентифиерстипе**</span><span class="sxs-lookup"><span data-stu-id="575c1-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="575c1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="575c1-106">Attributes and elements</span></span>

<span data-ttu-id="575c1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="575c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="575c1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="575c1-108">Attributes</span></span>

<span data-ttu-id="575c1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="575c1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="575c1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="575c1-110">Child elements</span></span>

|<span data-ttu-id="575c1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="575c1-111">**Element**</span></span>|<span data-ttu-id="575c1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="575c1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="575c1-113">рестриктедграупидентифиер</span><span class="sxs-lookup"><span data-stu-id="575c1-113">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="575c1-114">Представляет идентификатор безопасности группы (SID) и атрибуты для группы с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="575c1-114">Represents the group security identifier (SID) and attributes for a restricted group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="575c1-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="575c1-115">Parent elements</span></span>

|<span data-ttu-id="575c1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="575c1-116">**Element**</span></span>|<span data-ttu-id="575c1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="575c1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="575c1-118">сериализедсекуритиконтекст</span><span class="sxs-lookup"><span data-stu-id="575c1-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="575c1-119">Используется в заголовке SOAP для сериализации маркеров при проверке подлинности "сервер — сервер".</span><span class="sxs-lookup"><span data-stu-id="575c1-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span> <span data-ttu-id="575c1-120">Сериализация маркеров не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="575c1-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="575c1-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="575c1-121">Remarks</span></span>

<span data-ttu-id="575c1-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="575c1-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="575c1-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="575c1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="575c1-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="575c1-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="575c1-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="575c1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="575c1-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="575c1-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="575c1-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="575c1-127">Validation File</span></span>  <br/> |<span data-ttu-id="575c1-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="575c1-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="575c1-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="575c1-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="575c1-130">False</span><span class="sxs-lookup"><span data-stu-id="575c1-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="575c1-131">См. также</span><span class="sxs-lookup"><span data-stu-id="575c1-131">See also</span></span>



- [<span data-ttu-id="575c1-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="575c1-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

