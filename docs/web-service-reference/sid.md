---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: Элемент SID представляет форму языка определения дескрипторов безопасности (SID) для учетной записи, используемой для олицетворения или доступа представителей.
ms.openlocfilehash: 0e3f740e9a056f7c0042049d97757b5f2d3c441d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468049"
---
# <a name="sid"></a><span data-ttu-id="03285-103">SID</span><span class="sxs-lookup"><span data-stu-id="03285-103">SID</span></span>

<span data-ttu-id="03285-104">Элемент **SID** представляет форму языка определения дескрипторов безопасности (SID) для учетной записи, используемой для олицетворения или доступа представителей.</span><span class="sxs-lookup"><span data-stu-id="03285-104">The **SID** element represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation or delegate access.</span></span> 
  
```xml
<SID/>
```

 <span data-ttu-id="03285-105">**сидтипе**</span><span class="sxs-lookup"><span data-stu-id="03285-105">**SIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03285-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="03285-106">Attributes and elements</span></span>

<span data-ttu-id="03285-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="03285-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03285-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="03285-108">Attributes</span></span>

<span data-ttu-id="03285-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="03285-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03285-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="03285-110">Child elements</span></span>

<span data-ttu-id="03285-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="03285-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03285-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="03285-112">Parent elements</span></span>

|<span data-ttu-id="03285-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03285-113">**Element**</span></span>|<span data-ttu-id="03285-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03285-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03285-115">коннектингсид</span><span class="sxs-lookup"><span data-stu-id="03285-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="03285-116">Представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.</span><span class="sxs-lookup"><span data-stu-id="03285-116">Represents an account to impersonate when using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="03285-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="03285-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="03285-118">UserId</span><span class="sxs-lookup"><span data-stu-id="03285-118">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="03285-119">Определяет делегата или пользователя с разрешениями на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="03285-119">Identifies a delegate user or a user with folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03285-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="03285-120">Text value</span></span>

<span data-ttu-id="03285-121">Текстовое значение — это строковое представление идентификатора безопасности.</span><span class="sxs-lookup"><span data-stu-id="03285-121">The text value is a string representation of a SID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03285-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="03285-122">Remarks</span></span>

<span data-ttu-id="03285-123">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="03285-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03285-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="03285-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03285-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="03285-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03285-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="03285-126">Schema Name</span></span>  <br/> |<span data-ttu-id="03285-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="03285-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="03285-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="03285-128">Validation File</span></span>  <br/> |<span data-ttu-id="03285-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="03285-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03285-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="03285-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="03285-131">False</span><span class="sxs-lookup"><span data-stu-id="03285-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03285-132">См. также</span><span class="sxs-lookup"><span data-stu-id="03285-132">See also</span></span>



- [<span data-ttu-id="03285-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="03285-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

