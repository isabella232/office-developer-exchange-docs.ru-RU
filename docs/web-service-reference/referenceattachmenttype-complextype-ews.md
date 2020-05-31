---
title: Референцеаттачменттипе complexType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: c53686ccd032cabcc3f64a3a6684f29afe63a9b1
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354178"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="2b696-102">Референцеаттачменттипе complexType (EWS)</span><span class="sxs-lookup"><span data-stu-id="2b696-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="2b696-103">Сведения о типе</span><span class="sxs-lookup"><span data-stu-id="2b696-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b696-104">**Пространство имен**</span><span class="sxs-lookup"><span data-stu-id="2b696-104">**Namespace**</span></span> <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b696-105">**Файл схемы**</span><span class="sxs-lookup"><span data-stu-id="2b696-105">**Schema file**</span></span> <br/> |<span data-ttu-id="2b696-106">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2b696-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b696-107">**Базовый элемент расширения**</span><span class="sxs-lookup"><span data-stu-id="2b696-107">**Extension base**</span></span> <br/> |<span data-ttu-id="2b696-108">т:аттачменттипе</span><span class="sxs-lookup"><span data-stu-id="2b696-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="2b696-109">Определение</span><span class="sxs-lookup"><span data-stu-id="2b696-109">Definition</span></span>

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

## <a name="elements-and-attributes"></a><span data-ttu-id="2b696-110">Элементы и атрибуты</span><span class="sxs-lookup"><span data-stu-id="2b696-110">Elements and attributes</span></span>

<span data-ttu-id="2b696-111">Если в схеме определяются конкретные требования, например **sequence**, **minOccurs**, **maxOccurs** и **choice**, см. раздел определений.</span><span class="sxs-lookup"><span data-stu-id="2b696-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="2b696-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2b696-112">Child elements</span></span>

|<span data-ttu-id="2b696-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2b696-113">**Element**</span></span>|<span data-ttu-id="2b696-114">**Тип**</span><span class="sxs-lookup"><span data-stu-id="2b696-114">**Type**</span></span>|<span data-ttu-id="2b696-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2b696-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="2b696-116">аттачлонгпаснаме</span><span class="sxs-lookup"><span data-stu-id="2b696-116">AttachLongPathName</span></span>](attachlongpathname.md) <br/> |<span data-ttu-id="2b696-117">xs: String</span><span class="sxs-lookup"><span data-stu-id="2b696-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="2b696-118">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2b696-118">Attributes</span></span>

<span data-ttu-id="2b696-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b696-119">None.</span></span>
  

