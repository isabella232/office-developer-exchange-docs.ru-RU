---
title: ексчанжеимперсонатион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: Элемент Ексчанжеимперсонатион используется в заголовке SOAP запроса. Когда этот элемент присутствует, вызывающий абонент пытается олицетворить учетную запись, содержащуюся в элементе Ексчанжеимперсонатион.
ms.openlocfilehash: 188219d95453dc45378c6ca65ab93c2de7db4eac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463351"
---
# <a name="exchangeimpersonation"></a><span data-ttu-id="bc138-104">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="bc138-104">ExchangeImpersonation</span></span>

<span data-ttu-id="bc138-105">Элемент **ексчанжеимперсонатион** используется в заголовке SOAP запроса.</span><span class="sxs-lookup"><span data-stu-id="bc138-105">The **ExchangeImpersonation** element is used in the SOAP header of a request.</span></span> <span data-ttu-id="bc138-106">Когда этот элемент присутствует, вызывающий абонент пытается олицетворить учетную запись, содержащуюся в элементе **ексчанжеимперсонатион** .</span><span class="sxs-lookup"><span data-stu-id="bc138-106">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span> 
  
[<span data-ttu-id="bc138-107">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="bc138-107">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 <span data-ttu-id="bc138-108">**ексчанжеимперсонатионтипе**</span><span class="sxs-lookup"><span data-stu-id="bc138-108">**ExchangeImpersonationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc138-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc138-109">Attributes and elements</span></span>

<span data-ttu-id="bc138-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc138-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc138-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc138-111">Attributes</span></span>

<span data-ttu-id="bc138-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc138-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc138-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc138-113">Child elements</span></span>

|<span data-ttu-id="bc138-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc138-114">**Element**</span></span>|<span data-ttu-id="bc138-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc138-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc138-116">коннектингсид</span><span class="sxs-lookup"><span data-stu-id="bc138-116">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="bc138-117">Представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.</span><span class="sxs-lookup"><span data-stu-id="bc138-117">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc138-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc138-118">Parent elements</span></span>

<span data-ttu-id="bc138-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc138-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc138-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="bc138-120">Remarks</span></span>

<span data-ttu-id="bc138-121">Вызывающая учетная запись должна иметь **MS-дов-олицетворение** прямо на сервере клиентского доступа и в службе **MS-дов-майимперсонате** в базе данных почтовых ящиков, которая содержит почтовый ящик для олицетворения или объекта пользователя или контакта Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bc138-121">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory User/Contact object.</span></span> 
  
<span data-ttu-id="bc138-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bc138-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc138-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc138-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc138-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc138-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc138-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc138-125">Schema name</span></span>  <br/> |<span data-ttu-id="bc138-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bc138-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc138-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc138-127">Validation file</span></span>  <br/> |<span data-ttu-id="bc138-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bc138-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc138-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc138-129">Can be empty</span></span>  <br/> |<span data-ttu-id="bc138-130">False</span><span class="sxs-lookup"><span data-stu-id="bc138-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc138-131">См. также</span><span class="sxs-lookup"><span data-stu-id="bc138-131">See also</span></span>



[<span data-ttu-id="bc138-132">Авторизация между серверами в EWS</span><span class="sxs-lookup"><span data-stu-id="bc138-132">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

