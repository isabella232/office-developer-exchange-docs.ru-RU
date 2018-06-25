---
title: PostalAddress (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: Элемент PostalAddress указывает почтовый адрес для пользователя.
ms.openlocfilehash: fb418154867aebb4d284e75be579003c0ddc88f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834855"
---
# <a name="postaladdress-personapostaladdresstype"></a><span data-ttu-id="93577-103">PostalAddress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="93577-103">PostalAddress (PersonaPostalAddressType)</span></span>

<span data-ttu-id="93577-104">Элемент **PostalAddress** указывает почтовый адрес для пользователя.</span><span class="sxs-lookup"><span data-stu-id="93577-104">The **PostalAddress** element specifies the postal address for a persona.</span></span> 
  
```XML
<PostalAddress>
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
   <PostOfficeBox/>
   <Type/>
   <Latitude/>
   <Longitude/>
   <Accuracy/>
   <Altitude/>
   <AltitudeAccuracy/>
   <FormattedAddress/>
   <LocationUri/>
   <LocationSource/>
</PostalAddress>
```

 <span data-ttu-id="93577-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="93577-105">**PersonaPostalAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93577-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93577-106">Attributes and elements</span></span>

<span data-ttu-id="93577-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="93577-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93577-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93577-108">Attributes</span></span>

<span data-ttu-id="93577-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="93577-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93577-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93577-110">Child elements</span></span>

<span data-ttu-id="93577-111">[Улица](street.md) | [Город](city.md) | [состояние](state-ex15websvcsotherref.md) | [страны](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [типа (string)](type-string.md) | [широта](latitude.md)  |  [ Долгота](longitude.md) | [точность](accuracy.md) | [Высота](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="93577-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93577-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93577-112">Parent elements</span></span>

[<span data-ttu-id="93577-113">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="93577-113">EnhancedLocation</span></span>](enhancedlocation.md)
  
## <a name="remarks"></a><span data-ttu-id="93577-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="93577-114">Remarks</span></span>

<span data-ttu-id="93577-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="93577-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93577-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="93577-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93577-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93577-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93577-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93577-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93577-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93577-119">Schema name</span></span>  <br/> |<span data-ttu-id="93577-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="93577-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="93577-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93577-121">Validation file</span></span>  <br/> |<span data-ttu-id="93577-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="93577-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93577-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93577-123">Can be empty</span></span>  <br/> ||
   

