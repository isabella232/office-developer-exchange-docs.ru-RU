---
title: Ауспаккаже (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: Элемент Ауспаккаже указывает схему проверки подлинности, используемую при проверке подлинности на сервере Exchange, на котором установлена роль сервера почтовых ящиков.
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761526"
---
# <a name="authpackage-pox"></a><span data-ttu-id="b5aca-103">Ауспаккаже (POX)</span><span class="sxs-lookup"><span data-stu-id="b5aca-103">AuthPackage (POX)</span></span>

<span data-ttu-id="b5aca-104">Элемент **ауспаккаже** указывает схему проверки подлинности, используемую при проверке подлинности на сервере Exchange, на котором установлена роль сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="b5aca-104">The **AuthPackage** element specifies the authentication scheme that is used when authenticating against the Exchange server that has the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="b5aca-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="b5aca-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="b5aca-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="b5aca-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="b5aca-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="b5aca-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="b5aca-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="b5aca-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="b5aca-109">Ауспаккаже (POX)</span><span class="sxs-lookup"><span data-stu-id="b5aca-109">AuthPackage (POX)</span></span>](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b5aca-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b5aca-110">Attributes and elements</span></span>

<span data-ttu-id="b5aca-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b5aca-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5aca-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b5aca-112">Attributes</span></span>

<span data-ttu-id="b5aca-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5aca-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5aca-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b5aca-114">Child elements</span></span>

<span data-ttu-id="b5aca-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5aca-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5aca-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b5aca-116">Parent elements</span></span>

|<span data-ttu-id="b5aca-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b5aca-117">**Element**</span></span>|<span data-ttu-id="b5aca-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b5aca-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5aca-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="b5aca-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b5aca-120">Содержит спецификации для подключения клиента к серверу клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b5aca-120">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5aca-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b5aca-121">Text value</span></span>

<span data-ttu-id="b5aca-122">Текстовое значение указывает схему проверки подлинности, используемую при проверке подлинности на сервере почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="b5aca-122">The text value specifies the authentication scheme that is used when authenticating against the Mailbox server.</span></span> <span data-ttu-id="b5aca-123">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="b5aca-123">The following are the possible values:</span></span>
  
- <span data-ttu-id="b5aca-124">Основное</span><span class="sxs-lookup"><span data-stu-id="b5aca-124">basic</span></span>
- <span data-ttu-id="b5aca-125">Kerbtray</span><span class="sxs-lookup"><span data-stu-id="b5aca-125">kerb</span></span>
- <span data-ttu-id="b5aca-126">кербнтлм</span><span class="sxs-lookup"><span data-stu-id="b5aca-126">kerbntlm</span></span>
- <span data-ttu-id="b5aca-127">NTLM</span><span class="sxs-lookup"><span data-stu-id="b5aca-127">ntlm</span></span>
- <span data-ttu-id="b5aca-128">certificate</span><span class="sxs-lookup"><span data-stu-id="b5aca-128">certificate</span></span>
- <span data-ttu-id="b5aca-129">подключение</span><span class="sxs-lookup"><span data-stu-id="b5aca-129">negotiate</span></span>
- <span data-ttu-id="b5aca-130">nego2</span><span class="sxs-lookup"><span data-stu-id="b5aca-130">nego2</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b5aca-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="b5aca-131">Remarks</span></span>

<span data-ttu-id="b5aca-132">Элемент **ауспаккаже** используется только в том случае, когда элемент [Type (POX)](type-pox.md) имеет текстовое значение в формате "курс" или "expr".</span><span class="sxs-lookup"><span data-stu-id="b5aca-132">The **AuthPackage** element is only used when the [Type (POX)](type-pox.md) element has a text value of EXCH or EXPR.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="b5aca-133">Различия версий</span><span class="sxs-lookup"><span data-stu-id="b5aca-133">Version differences</span></span>

<span data-ttu-id="b5aca-134">Office 365, Exchange Online и локальная версия Exchange, начиная с сборки 15.00.0995.014, возвращают значение "Negotiate" только в том случае, если сервер настроен на использование проверки подлинности согласования, а клиент включает заголовок [X-клиентканхандле](pox-autodiscover-request-for-exchange.md) , который содержит "Negotiate".</span><span class="sxs-lookup"><span data-stu-id="b5aca-134">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "negotiate" only if the server is configured to use Negotiate authentication and the client includes a [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "Negotiate".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b5aca-135">См. также</span><span class="sxs-lookup"><span data-stu-id="b5aca-135">See also</span></span>

- [<span data-ttu-id="b5aca-136">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="b5aca-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

