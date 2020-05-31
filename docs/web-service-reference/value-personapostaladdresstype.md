---
title: Значение (Персонапосталаддресстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: Элемент value указывает сведения, связанные с почтовым адресом.
ms.openlocfilehash: 048d3a49552f1a9e89744e4cd16ec1745417e923
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840462"
---
# <a name="value-personapostaladdresstype"></a><span data-ttu-id="1cc3c-103">Значение (Персонапосталаддресстипе)</span><span class="sxs-lookup"><span data-stu-id="1cc3c-103">Value (PersonaPostalAddressType)</span></span>

<span data-ttu-id="1cc3c-104">Элемент **value** указывает сведения, связанные с почтовым адресом.</span><span class="sxs-lookup"><span data-stu-id="1cc3c-104">The **Value** element specifies information associated with a postal address.</span></span> 
  
```XML
<Value>
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
</Value>
```

<span data-ttu-id="1cc3c-105">**персонапосталаддресстипе**</span><span class="sxs-lookup"><span data-stu-id="1cc3c-105">**PersonaPostalAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1cc3c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1cc3c-106">Attributes and elements</span></span>

<span data-ttu-id="1cc3c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1cc3c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cc3c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1cc3c-108">Attributes</span></span>

<span data-ttu-id="1cc3c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1cc3c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cc3c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1cc3c-110">Child elements</span></span>

<span data-ttu-id="1cc3c-111">[Street](street.md)[State](state-ex15websvcsotherref.md)[PostalCode](postalcode.md) | [Altitude](altitude.md) | [LocationSource](locationsource.md) [PostOfficeBox](postofficebox.md) | [Latitude](latitude.md) | [LocationUri](locationuri.md)[FormattedAddress](formattedaddress.md)[Country](country.md) | [City](city.md) |  |  | [AltitudeAccuracy](altitudeaccuracy.md)[Accuracy](accuracy.md)[Longitude](longitude.md)[Type (string)](type-string.md)Город проживания |  | страна с | адресом PostOfficeBox тип (String) Широта/Долгота точность точность высота алтитудеаккураци форматтедаддресс LocationUri локатионсаурце |  |  | </span><span class="sxs-lookup"><span data-stu-id="1cc3c-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1cc3c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1cc3c-112">Parent elements</span></span>

[<span data-ttu-id="1cc3c-113">посталаддрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="1cc3c-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="1cc3c-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="1cc3c-114">Remarks</span></span>

<span data-ttu-id="1cc3c-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1cc3c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1cc3c-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1cc3c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cc3c-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1cc3c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cc3c-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1cc3c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1cc3c-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1cc3c-119">Schema name</span></span>  <br/> |<span data-ttu-id="1cc3c-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1cc3c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="1cc3c-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1cc3c-121">Validation file</span></span>  <br/> |<span data-ttu-id="1cc3c-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1cc3c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1cc3c-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1cc3c-123">Can be empty</span></span>  <br/> ||
   

