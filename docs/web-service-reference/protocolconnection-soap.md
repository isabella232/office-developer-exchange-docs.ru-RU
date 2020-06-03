---
title: Протоколконнектион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: Элемент Протоколконнектион представляет подключение протокола для веб-клиента сервера.
ms.openlocfilehash: b9df3febe36db53d7c5bf0610ba857f13aa96abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528862"
---
# <a name="protocolconnection-soap"></a><span data-ttu-id="bab07-103">Протоколконнектион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bab07-103">ProtocolConnection (SOAP)</span></span>

<span data-ttu-id="bab07-104">Элемент **протоколконнектион** представляет подключение протокола для веб-клиента сервера.</span><span class="sxs-lookup"><span data-stu-id="bab07-104">The **ProtocolConnection** element represents the protocol connection of the server Web client.</span></span> 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 <span data-ttu-id="bab07-105">**протоколконнектион**</span><span class="sxs-lookup"><span data-stu-id="bab07-105">**ProtocolConnection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bab07-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bab07-106">Attributes and elements</span></span>

<span data-ttu-id="bab07-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bab07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bab07-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bab07-108">Attributes</span></span>

<span data-ttu-id="bab07-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bab07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bab07-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bab07-110">Child elements</span></span>

|<span data-ttu-id="bab07-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bab07-111">**Element**</span></span>|<span data-ttu-id="bab07-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bab07-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bab07-113">Имя узла (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bab07-113">Hostname (SOAP)</span></span>](hostname-soap.md) <br/> |<span data-ttu-id="bab07-114">Представляет часть имени узла для полного имени компьютера.</span><span class="sxs-lookup"><span data-stu-id="bab07-114">Represents the host name portion of the full computer name of the computer.</span></span>  <br/> |
|[<span data-ttu-id="bab07-115">Порт (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bab07-115">Port (SOAP)</span></span>](port-soap.md) <br/> |<span data-ttu-id="bab07-116">Представляет номер порта, который будет использоваться для протокола.</span><span class="sxs-lookup"><span data-stu-id="bab07-116">Represents the port number to use for the protocol.</span></span>  <br/> |
|[<span data-ttu-id="bab07-117">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bab07-117">EncryptionMethod (SOAP)</span></span>](encryptionmethod-soap.md) <br/> |<span data-ttu-id="bab07-118">Представляет криптографический метод, используемый для протоколов POP, IMAP и SMTP.</span><span class="sxs-lookup"><span data-stu-id="bab07-118">Represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bab07-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bab07-119">Parent elements</span></span>

|<span data-ttu-id="bab07-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bab07-120">**Element**</span></span>|<span data-ttu-id="bab07-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bab07-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bab07-122">Протоколконнектионс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bab07-122">ProtocolConnections (SOAP)</span></span>](protocolconnections-soap.md) <br/> |<span data-ttu-id="bab07-123">Содержит ноль или более подключений протоколов.</span><span class="sxs-lookup"><span data-stu-id="bab07-123">Contains zero or more protocol connections.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bab07-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bab07-124">Text value</span></span>

<span data-ttu-id="bab07-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bab07-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bab07-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bab07-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bab07-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bab07-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bab07-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bab07-128">Schema Name</span></span>  <br/> |<span data-ttu-id="bab07-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bab07-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bab07-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bab07-130">Validation File</span></span>  <br/> |<span data-ttu-id="bab07-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bab07-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bab07-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bab07-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="bab07-133">True</span><span class="sxs-lookup"><span data-stu-id="bab07-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bab07-134">См. также</span><span class="sxs-lookup"><span data-stu-id="bab07-134">See also</span></span>



[<span data-ttu-id="bab07-135">Протоколконнектионколлектионсеттинг (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bab07-135">ProtocolConnectionCollectionSetting (SOAP)</span></span>](protocolconnectioncollectionsetting-soap.md)

