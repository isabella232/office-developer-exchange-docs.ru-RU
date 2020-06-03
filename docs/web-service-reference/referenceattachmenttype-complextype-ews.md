---
title: Референцеаттачменттипе complexType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: 24f5a62eadd490b5b0000dfe048850c44540f266
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528736"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="1ec96-102">Референцеаттачменттипе complexType (EWS)</span><span class="sxs-lookup"><span data-stu-id="1ec96-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="1ec96-103">Сведения о типе</span><span class="sxs-lookup"><span data-stu-id="1ec96-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ec96-104">**Пространство имен**</span><span class="sxs-lookup"><span data-stu-id="1ec96-104">**Namespace**</span></span> <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ec96-105">**Файл схемы**</span><span class="sxs-lookup"><span data-stu-id="1ec96-105">**Schema file**</span></span> <br/> |<span data-ttu-id="1ec96-106">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1ec96-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ec96-107">**Базовый элемент расширения**</span><span class="sxs-lookup"><span data-stu-id="1ec96-107">**Extension base**</span></span> <br/> |<span data-ttu-id="1ec96-108">т:аттачменттипе</span><span class="sxs-lookup"><span data-stu-id="1ec96-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="1ec96-109">Определение</span><span class="sxs-lookup"><span data-stu-id="1ec96-109">Definition</span></span>

```XML
<xs:complexType name="ReferenceAttachmentType">
    <xs:complexContent>
        <xs:extension base="t:AttachmentType">
            <xs:sequence>
                <xs:element name="AttachLongPathName" type="xs:string" maxOccurs="1" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:extension>
    </xs:complexContent>
</xs:complexType>

```

## <a name="elements-and-attributes"></a><span data-ttu-id="1ec96-110">Элементы и атрибуты</span><span class="sxs-lookup"><span data-stu-id="1ec96-110">Elements and attributes</span></span>

<span data-ttu-id="1ec96-111">Если в схеме определяются конкретные требования, например **sequence**, **minOccurs**, **maxOccurs** и **choice**, см. раздел определений.</span><span class="sxs-lookup"><span data-stu-id="1ec96-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="1ec96-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1ec96-112">Child elements</span></span>

|<span data-ttu-id="1ec96-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1ec96-113">**Element**</span></span>|<span data-ttu-id="1ec96-114">**Тип**</span><span class="sxs-lookup"><span data-stu-id="1ec96-114">**Type**</span></span>|<span data-ttu-id="1ec96-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1ec96-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="1ec96-116">аттачлонгпаснаме</span><span class="sxs-lookup"><span data-stu-id="1ec96-116">AttachLongPathName</span></span>](attachlongpathname.md) <br/> |<span data-ttu-id="1ec96-117">xs: String</span><span class="sxs-lookup"><span data-stu-id="1ec96-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="1ec96-118">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1ec96-118">Attributes</span></span>

<span data-ttu-id="1ec96-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ec96-119">None.</span></span>
  

