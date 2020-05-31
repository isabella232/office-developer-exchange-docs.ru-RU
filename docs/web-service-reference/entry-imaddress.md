---
title: Запись (адрес)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: ee444170-7353-4e86-86c6-d7300a2f1777
description: Элемент entry представляет адрес обмена мгновенными сообщениями для контакта.
ms.openlocfilehash: 77de059cef470dde90ab0b929845cb260b4b867c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762383"
---
# <a name="entry-imaddress"></a><span data-ttu-id="cd894-103">Запись (адрес)</span><span class="sxs-lookup"><span data-stu-id="cd894-103">Entry (IMAddress)</span></span>

<span data-ttu-id="cd894-104">Элемент **entry** представляет адрес обмена мгновенными сообщениями для контакта.</span><span class="sxs-lookup"><span data-stu-id="cd894-104">The **Entry** element represents an instant messaging (IM) address for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="cd894-105">**имаддрессдиктионарентритипе**</span><span class="sxs-lookup"><span data-stu-id="cd894-105">**ImAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd894-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cd894-106">Attributes and elements</span></span>

<span data-ttu-id="cd894-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cd894-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd894-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cd894-108">Attributes</span></span>

|<span data-ttu-id="cd894-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="cd894-109">**Attribute**</span></span>|<span data-ttu-id="cd894-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd894-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cd894-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="cd894-111">**Key**</span></span> <br/> | <span data-ttu-id="cd894-112">Определяет адрес для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="cd894-112">Identifies the IM address.</span></span><br/><br/><span data-ttu-id="cd894-113">Ниже приведены возможные значения для этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="cd894-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="cd894-114">- ImAddress1</span><span class="sxs-lookup"><span data-stu-id="cd894-114">-  ImAddress1</span></span>  <br/><span data-ttu-id="cd894-115">- ImAddress2</span><span class="sxs-lookup"><span data-stu-id="cd894-115">-  ImAddress2</span></span>  <br/><span data-ttu-id="cd894-116">- ImAddress3</span><span class="sxs-lookup"><span data-stu-id="cd894-116">-  ImAddress3</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cd894-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cd894-117">Child elements</span></span>

<span data-ttu-id="cd894-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="cd894-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd894-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cd894-119">Parent elements</span></span>

|<span data-ttu-id="cd894-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd894-120">**Element**</span></span>|<span data-ttu-id="cd894-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd894-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd894-122">Адреса</span><span class="sxs-lookup"><span data-stu-id="cd894-122">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="cd894-123">Представляет коллекцию адресов обмена мгновенными сообщениями для контакта.</span><span class="sxs-lookup"><span data-stu-id="cd894-123">Represents a collection of IM addresses for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd894-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cd894-124">Text value</span></span>

<span data-ttu-id="cd894-125">При использовании этого элемента необходимо указать текстовое значение, представляющее адрес для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="cd894-125">A text value that represents the IM address is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cd894-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="cd894-126">Remarks</span></span>

<span data-ttu-id="cd894-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cd894-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd894-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cd894-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd894-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cd894-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd894-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cd894-130">Schema name</span></span>  <br/> |<span data-ttu-id="cd894-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cd894-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd894-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cd894-132">Validation file</span></span>  <br/> |<span data-ttu-id="cd894-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cd894-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd894-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cd894-134">Can be empty</span></span>  <br/> |<span data-ttu-id="cd894-135">False</span><span class="sxs-lookup"><span data-stu-id="cd894-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd894-136">См. также</span><span class="sxs-lookup"><span data-stu-id="cd894-136">See also</span></span>

- [<span data-ttu-id="cd894-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cd894-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="cd894-138">Создание контактов (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="cd894-138">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="cd894-139">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="cd894-139">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="cd894-140">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="cd894-140">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

