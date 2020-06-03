---
title: граупсидс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: Элемент Граупсидс представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.
ms.openlocfilehash: 40f36176fcaa3e2160237f269fb2dc3b12bf8af2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530066"
---
# <a name="groupsids"></a><span data-ttu-id="962dd-103">граупсидс</span><span class="sxs-lookup"><span data-stu-id="962dd-103">GroupSids</span></span>

<span data-ttu-id="962dd-104">Элемент **граупсидс** представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="962dd-104">The **GroupSids** element represents a collection of Active Directory directory service group object security identifiers.</span></span> 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 <span data-ttu-id="962dd-105">**нонемптяррайофграупидентифиерстипе**</span><span class="sxs-lookup"><span data-stu-id="962dd-105">**NonEmptyArrayOfGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="962dd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="962dd-106">Attributes and elements</span></span>

<span data-ttu-id="962dd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="962dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="962dd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="962dd-108">Attributes</span></span>

<span data-ttu-id="962dd-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="962dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="962dd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="962dd-110">Child elements</span></span>

|<span data-ttu-id="962dd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="962dd-111">**Element**</span></span>|<span data-ttu-id="962dd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="962dd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="962dd-113">граупидентифиер</span><span class="sxs-lookup"><span data-stu-id="962dd-113">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="962dd-114">Представляет один идентификатор безопасности и атрибут для группы объектов Active Directory, членом которой является учетная запись.</span><span class="sxs-lookup"><span data-stu-id="962dd-114">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="962dd-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="962dd-115">Parent elements</span></span>

|<span data-ttu-id="962dd-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="962dd-116">**Element**</span></span>|<span data-ttu-id="962dd-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="962dd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="962dd-118">сериализедсекуритиконтекст</span><span class="sxs-lookup"><span data-stu-id="962dd-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="962dd-119">Используется в заголовке протокола SOAP для сериализации маркеров при проверке подлинности "сервер-сервер".</span><span class="sxs-lookup"><span data-stu-id="962dd-119">Used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="962dd-120">Сериализация маркеров не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="962dd-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="962dd-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="962dd-121">Remarks</span></span>

<span data-ttu-id="962dd-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="962dd-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="962dd-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="962dd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="962dd-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="962dd-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="962dd-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="962dd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="962dd-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="962dd-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="962dd-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="962dd-127">Validation File</span></span>  <br/> |<span data-ttu-id="962dd-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="962dd-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="962dd-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="962dd-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="962dd-130">False</span><span class="sxs-lookup"><span data-stu-id="962dd-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="962dd-131">См. также</span><span class="sxs-lookup"><span data-stu-id="962dd-131">See also</span></span>



- [<span data-ttu-id="962dd-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="962dd-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

