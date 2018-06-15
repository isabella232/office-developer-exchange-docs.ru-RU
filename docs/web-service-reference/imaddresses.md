---
title: ImAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ImAddresses
api_type:
- schema
ms.assetid: 29f614a7-7fe6-47fa-b5f2-8feff106aa99
description: Элемент ImAddresses представляет коллекцию мгновенного обмена сообщениями адресов для контакта.
ms.openlocfilehash: e8c7a22e8537a4526594042905f7bb8454238bf1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833861"
---
# <a name="imaddresses"></a><span data-ttu-id="887d1-103">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="887d1-103">ImAddresses</span></span>

<span data-ttu-id="887d1-104">Элемент **ImAddresses** представляет коллекцию мгновенного обмена сообщениями адресов для контакта.</span><span class="sxs-lookup"><span data-stu-id="887d1-104">The **ImAddresses** element represents a collection of instant messaging addresses for a contact.</span></span> 
  
```xml
<ImAddresses>
   <Entry/>
</ImAddresses>
```

 <span data-ttu-id="887d1-105">**ImAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="887d1-105">**ImAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="887d1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="887d1-106">Attributes and elements</span></span>

<span data-ttu-id="887d1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="887d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="887d1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="887d1-108">Attributes</span></span>

<span data-ttu-id="887d1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="887d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="887d1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="887d1-110">Child elements</span></span>

|<span data-ttu-id="887d1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="887d1-111">**Element**</span></span>|<span data-ttu-id="887d1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="887d1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="887d1-113">Запись (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="887d1-113">Entry (IMAddress)</span></span>](entry-imaddress.md) <br/> |<span data-ttu-id="887d1-114">Представляет обмена мгновенными сообщениями адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="887d1-114">Represents an instant messaging address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="887d1-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="887d1-115">Parent elements</span></span>

|<span data-ttu-id="887d1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="887d1-116">**Element**</span></span>|<span data-ttu-id="887d1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="887d1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="887d1-118">Контакт</span><span class="sxs-lookup"><span data-stu-id="887d1-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="887d1-119">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="887d1-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="887d1-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="887d1-120">Remarks</span></span>

<span data-ttu-id="887d1-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="887d1-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="887d1-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="887d1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="887d1-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="887d1-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="887d1-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="887d1-124">Schema name</span></span>  <br/> |<span data-ttu-id="887d1-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="887d1-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="887d1-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="887d1-126">Validation file</span></span>  <br/> |<span data-ttu-id="887d1-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="887d1-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="887d1-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="887d1-128">Can be empty</span></span>  <br/> |<span data-ttu-id="887d1-129">False</span><span class="sxs-lookup"><span data-stu-id="887d1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="887d1-130">См. также</span><span class="sxs-lookup"><span data-stu-id="887d1-130">See also</span></span>



- [<span data-ttu-id="887d1-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="887d1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
