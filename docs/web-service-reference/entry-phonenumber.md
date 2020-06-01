---
title: Запись (PhoneNumber)
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
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: Элемент entry представляет телефонный номер контакта.
ms.openlocfilehash: 62f7091bb750dc7ca74b1e5637a437e2cdad4f1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459639"
---
# <a name="entry-phonenumber"></a><span data-ttu-id="8737f-103">Запись (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="8737f-103">Entry (PhoneNumber)</span></span>

<span data-ttu-id="8737f-104">Элемент **entry** представляет телефонный номер контакта.</span><span class="sxs-lookup"><span data-stu-id="8737f-104">The **Entry** element represents a telephone number for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="8737f-105">**фоненумбердиктионарентритипе**</span><span class="sxs-lookup"><span data-stu-id="8737f-105">**PhoneNumberDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8737f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8737f-106">Attributes and elements</span></span>

<span data-ttu-id="8737f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8737f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8737f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8737f-108">Attributes</span></span>

|<span data-ttu-id="8737f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8737f-109">**Attribute**</span></span>|<span data-ttu-id="8737f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8737f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8737f-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="8737f-111">**Key**</span></span> <br/> | <span data-ttu-id="8737f-112">Указывает номер телефона.</span><span class="sxs-lookup"><span data-stu-id="8737f-112">Identifies the telephone number.</span></span> <span data-ttu-id="8737f-113">Ключевой атрибут относится к типу **фоненумберкэйтипе**.</span><span class="sxs-lookup"><span data-stu-id="8737f-113">The Key attribute is of type **PhoneNumberKeyType**.</span></span><br/><br/> <span data-ttu-id="8737f-114">Ниже приведены возможные значения для этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="8737f-114">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="8737f-115">— Ассистантфоне</span><span class="sxs-lookup"><span data-stu-id="8737f-115">-  AssistantPhone</span></span>  <br/><span data-ttu-id="8737f-116">— Бусинессфакс</span><span class="sxs-lookup"><span data-stu-id="8737f-116">-  BusinessFax</span></span>  <br/><span data-ttu-id="8737f-117">— Бусинессфоне</span><span class="sxs-lookup"><span data-stu-id="8737f-117">-  BusinessPhone</span></span>  <br/><span data-ttu-id="8737f-118">- BusinessPhone2</span><span class="sxs-lookup"><span data-stu-id="8737f-118">-  BusinessPhone2</span></span>  <br/><span data-ttu-id="8737f-119">Ответный вызов</span><span class="sxs-lookup"><span data-stu-id="8737f-119">-  Callback</span></span>  <br/><span data-ttu-id="8737f-120">— Карфоне</span><span class="sxs-lookup"><span data-stu-id="8737f-120">-  CarPhone</span></span>  <br/><span data-ttu-id="8737f-121">— Компанимаинфоне</span><span class="sxs-lookup"><span data-stu-id="8737f-121">-  CompanyMainPhone</span></span>  <br/><span data-ttu-id="8737f-122">— Хомефакс</span><span class="sxs-lookup"><span data-stu-id="8737f-122">-  HomeFax</span></span>  <br/><span data-ttu-id="8737f-123">— HomePhone</span><span class="sxs-lookup"><span data-stu-id="8737f-123">-  HomePhone</span></span>  <br/><span data-ttu-id="8737f-124">- HomePhone2</span><span class="sxs-lookup"><span data-stu-id="8737f-124">-  HomePhone2</span></span>  <br/><span data-ttu-id="8737f-125">– ISDN</span><span class="sxs-lookup"><span data-stu-id="8737f-125">-  Isdn</span></span>  <br/><span data-ttu-id="8737f-126">— MobilePhone</span><span class="sxs-lookup"><span data-stu-id="8737f-126">-  MobilePhone</span></span>  <br/><span data-ttu-id="8737f-127">— OtherFax</span><span class="sxs-lookup"><span data-stu-id="8737f-127">-  OtherFax</span></span>  <br/><span data-ttu-id="8737f-128">— OtherTelephone</span><span class="sxs-lookup"><span data-stu-id="8737f-128">-  OtherTelephone</span></span>  <br/><span data-ttu-id="8737f-129">— Пейджер</span><span class="sxs-lookup"><span data-stu-id="8737f-129">-  Pager</span></span>  <br/><span data-ttu-id="8737f-130">— Примарифоне</span><span class="sxs-lookup"><span data-stu-id="8737f-130">-  PrimaryPhone</span></span>  <br/><span data-ttu-id="8737f-131">— Радиофоне</span><span class="sxs-lookup"><span data-stu-id="8737f-131">-  RadioPhone</span></span>  <br/><span data-ttu-id="8737f-132">— Телекса</span><span class="sxs-lookup"><span data-stu-id="8737f-132">-  Telex</span></span>  <br/><span data-ttu-id="8737f-133">— Ттитддфоне</span><span class="sxs-lookup"><span data-stu-id="8737f-133">-  TtyTddPhone</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8737f-134">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8737f-134">Child elements</span></span>

<span data-ttu-id="8737f-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8737f-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8737f-136">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8737f-136">Parent elements</span></span>

|<span data-ttu-id="8737f-137">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8737f-137">**Element**</span></span>|<span data-ttu-id="8737f-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8737f-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8737f-139">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="8737f-139">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="8737f-140">Представляет коллекцию телефонных номеров контакта.</span><span class="sxs-lookup"><span data-stu-id="8737f-140">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8737f-141">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8737f-141">Text value</span></span>

<span data-ttu-id="8737f-142">При использовании этого элемента необходимо указать текстовое значение, представляющее номер телефона.</span><span class="sxs-lookup"><span data-stu-id="8737f-142">A text value that represents a telephone number is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8737f-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="8737f-143">Remarks</span></span>

<span data-ttu-id="8737f-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8737f-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8737f-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8737f-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8737f-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8737f-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8737f-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8737f-147">Schema name</span></span>  <br/> |<span data-ttu-id="8737f-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8737f-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="8737f-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8737f-149">Validation file</span></span>  <br/> |<span data-ttu-id="8737f-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8737f-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8737f-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8737f-151">Can be empty</span></span>  <br/> |<span data-ttu-id="8737f-152">False</span><span class="sxs-lookup"><span data-stu-id="8737f-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8737f-153">См. также</span><span class="sxs-lookup"><span data-stu-id="8737f-153">See also</span></span>

- [<span data-ttu-id="8737f-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8737f-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="8737f-155">Создание контактов (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="8737f-155">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="8737f-156">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="8737f-156">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="8737f-157">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="8737f-157">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

