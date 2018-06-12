---
title: Ошибки, связанные с свойство веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1c4c5969-7bdd-4021-be0e-cae99e86cf2c
description: Узнайте, как обрабатывать ошибки, связанные с свойство в приложении веб-служб Exchange.
ms.openlocfilehash: f214ab40c3717178c6957a9da93bdf89999fc1d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760950"
---
# <a name="ews-property-related-errors"></a><span data-ttu-id="56c40-103">Ошибки, связанные с свойство веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="56c40-103">EWS property-related errors</span></span>

<span data-ttu-id="56c40-104">Узнайте, как обрабатывать ошибки, связанные с свойство в приложении веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="56c40-104">Find out how to handle property-related errors in your EWS application.</span></span>
  
<span data-ttu-id="56c40-105">Большинство клиентских приложений веб-служб Exchange будет использовать свойства, что означает, что необходимо обрабатывать ошибки, связанные с свойство.</span><span class="sxs-lookup"><span data-stu-id="56c40-105">Most EWS client applications will use properties, which means that you will have to handle property-related errors.</span></span> <span data-ttu-id="56c40-106">Может обрабатывать эти ошибки во время выполнения или при разработке приложения веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="56c40-106">You can handle these errors at runtime, or while you are developing your EWS application.</span></span>
  
<span data-ttu-id="56c40-107">**В таблице 1: Ошибки, связанные с свойство и порядок их обработки**</span><span class="sxs-lookup"><span data-stu-id="56c40-107">**Table 1: Property-related errors and how to handle them**</span></span>

|<span data-ttu-id="56c40-108">**Error**</span><span class="sxs-lookup"><span data-stu-id="56c40-108">**Error**</span></span>|<span data-ttu-id="56c40-109">**Возникающие при попытке...**</span><span class="sxs-lookup"><span data-stu-id="56c40-109">**Caused by an attempt to…**</span></span>|<span data-ttu-id="56c40-110">**Обработать его с...**</span><span class="sxs-lookup"><span data-stu-id="56c40-110">**Handle it by…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="56c40-111">ErrorDataSizeLimitExceeded</span><span class="sxs-lookup"><span data-stu-id="56c40-111">ErrorDataSizeLimitExceeded</span></span>  <br/> |<span data-ttu-id="56c40-112">Задайте для свойства значение, превышающее максимальный размер для свойства или свойства не поддерживает потоковая передача по технологии, такие как свойства папки.</span><span class="sxs-lookup"><span data-stu-id="56c40-112">Set a property with a value that exceeds the maximum size for the property or the property does not support streaming, such as folder properties.</span></span>  <br/> |<span data-ttu-id="56c40-113">Ограничение размера данных, задайте для свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-113">Limiting the size of data you set on the property.</span></span>  <br/> |
|<span data-ttu-id="56c40-114">ErrorFolderPropertRequestFailed</span><span class="sxs-lookup"><span data-stu-id="56c40-114">ErrorFolderPropertRequestFailed</span></span>  <br/> |<span data-ttu-id="56c40-115">Получите свойство, которое не удалось получить.</span><span class="sxs-lookup"><span data-stu-id="56c40-115">Get a property that could not be retrieved.</span></span>  <br/> |<span data-ttu-id="56c40-116">Указывает, что свойство не удается получить.</span><span class="sxs-lookup"><span data-stu-id="56c40-116">Indicating that the property cannot be retrieved.</span></span>  <br/> |
|<span data-ttu-id="56c40-117">ErrorInvalidExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="56c40-117">ErrorInvalidExtendedProperty</span></span>  <br/> |<span data-ttu-id="56c40-118">Задайте Недопустимое сочетание значений расширенных свойств или результаты в недопустимом расширенные свойства универсальный код ресурса (URI).</span><span class="sxs-lookup"><span data-stu-id="56c40-118">Set an invalid combination of extended property values or results in an invalid extended property Uniform Resource Identifier (URI).</span></span>  <br/> |<span data-ttu-id="56c40-119">Проверка значения расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-119">Checking the extended property value.</span></span>  <br/> |
|<span data-ttu-id="56c40-120">ErrorInvalidExtendedPropertyValue</span><span class="sxs-lookup"><span data-stu-id="56c40-120">ErrorInvalidExtendedPropertyValue</span></span>  <br/> |<span data-ttu-id="56c40-121">Задайте значение расширенного свойства, которое не соответствует указанному типу</span><span class="sxs-lookup"><span data-stu-id="56c40-121">Set an extended property value that does not match the specified type</span></span>  <br/> |<span data-ttu-id="56c40-122">Обновление кода для проверки соответствия типов.</span><span class="sxs-lookup"><span data-stu-id="56c40-122">Updating your code to check for matching types.</span></span>  <br/> |
|<span data-ttu-id="56c40-123">ErrorInvalidFolderId</span><span class="sxs-lookup"><span data-stu-id="56c40-123">ErrorInvalidFolderId</span></span>  <br/> |<span data-ttu-id="56c40-124">Значение структуры идентификатор папки недопустимый формы.</span><span class="sxs-lookup"><span data-stu-id="56c40-124">Set the structure of a folder identifier to an invalid form.</span></span>  <br/> |<span data-ttu-id="56c40-125">Только с использованием идентификаторов возвращаемых веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="56c40-125">Only using identifiers returned by EWS.</span></span>  <br/> |
|<span data-ttu-id="56c40-126">ErrorInvalidId</span><span class="sxs-lookup"><span data-stu-id="56c40-126">ErrorInvalidId</span></span>  <br/> |<span data-ttu-id="56c40-127">Задайте структура идентификатора и/или изменить ключ на недопустимое формы.</span><span class="sxs-lookup"><span data-stu-id="56c40-127">Set the structure of an identifier and/or change key to an invalid form.</span></span>  <br/> |<span data-ttu-id="56c40-128">Только с использованием идентификаторов возвращаемых веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="56c40-128">Only using identifiers returned by EWS.</span></span>  <br/> |
|<span data-ttu-id="56c40-129">ErrorInvalidIdEmpty</span><span class="sxs-lookup"><span data-stu-id="56c40-129">ErrorInvalidIdEmpty</span></span>  <br/> |<span data-ttu-id="56c40-130">Задайте пустой идентификатор.</span><span class="sxs-lookup"><span data-stu-id="56c40-130">Set an empty an identifier.</span></span>  <br/> |<span data-ttu-id="56c40-131">Настройка идентификатора с допустимым идентификатором элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="56c40-131">Setting the identifier with a valid item or folder identifier.</span></span>  <br/> |
|<span data-ttu-id="56c40-132">ErrorInvalidIdMalformed</span><span class="sxs-lookup"><span data-stu-id="56c40-132">ErrorInvalidIdMalformed</span></span>  <br/> |<span data-ttu-id="56c40-133">Задайте структура идентификатора и/или изменить ключ на недопустимое формы.</span><span class="sxs-lookup"><span data-stu-id="56c40-133">Set the structure of an identifier and/or change key to an invalid form.</span></span>  <br/> |<span data-ttu-id="56c40-134">Только с использованием идентификаторов возвращаемых веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="56c40-134">Only using identifiers returned by EWS.</span></span>  <br/> |
|<span data-ttu-id="56c40-135">ErrorInvalidPropertyAppend</span><span class="sxs-lookup"><span data-stu-id="56c40-135">ErrorInvalidPropertyAppend</span></span>  <br/> |<span data-ttu-id="56c40-136">Добавьте свойство, которое не поддерживает добавление.</span><span class="sxs-lookup"><span data-stu-id="56c40-136">Append a property that does not support appending.</span></span>  <br/> |<span data-ttu-id="56c40-137">Обновление кода, чтобы она пытается добавить значения свойства набор получателей (Кому, копия, Bcc), свойства коллекции Attendee (требуется, необязательно, ресурсы), свойство Body и свойство ReplyTo.</span><span class="sxs-lookup"><span data-stu-id="56c40-137">Updating your code so that it only attempts to append values to the recipient collection properties (To, Cc, Bcc), Attendee collection properties (Required, Optional, Resources), Body property, and the ReplyTo property.</span></span>  <br/> |
|<span data-ttu-id="56c40-138">ErrorInvalidPropertyDelete</span><span class="sxs-lookup"><span data-stu-id="56c40-138">ErrorInvalidPropertyDelete</span></span>  <br/> |<span data-ttu-id="56c40-139">Удаление свойства, которое не поддерживает удаление.</span><span class="sxs-lookup"><span data-stu-id="56c40-139">Delete a property that does not support deleting.</span></span>  <br/> |<span data-ttu-id="56c40-140">Обновление кода, не пытайтесь удалить свойство.</span><span class="sxs-lookup"><span data-stu-id="56c40-140">Updating your code to not try to delete the property.</span></span> <span data-ttu-id="56c40-141">Например невозможно удалить папку и идентификаторы элементов.</span><span class="sxs-lookup"><span data-stu-id="56c40-141">For example, the folder and item identifiers cannot be deleted.</span></span>  <br/> |
|<span data-ttu-id="56c40-142">ErrorInvalidPropertyForExists</span><span class="sxs-lookup"><span data-stu-id="56c40-142">ErrorInvalidPropertyForExists</span></span>  <br/> |<span data-ttu-id="56c40-143">Задайте ограничения существования на основе поиска на основе флаг свойство.</span><span class="sxs-lookup"><span data-stu-id="56c40-143">Set an existential based search restriction on a flag-based property.</span></span>  <br/> |<span data-ttu-id="56c40-144">Обновление кода, не используйте свойства на основе флаг в ограничения существования на основе поиска.</span><span class="sxs-lookup"><span data-stu-id="56c40-144">Updating your code to not use flag-based properties in an existential based search restriction.</span></span> <span data-ttu-id="56c40-145">На основе флаг свойства — это IsDraft, IsSubmitted, IsUnmodified, IsResend и IsFromMe.</span><span class="sxs-lookup"><span data-stu-id="56c40-145">Flag-based properties are IsDraft, IsSubmitted, IsUnmodified, IsResend, and IsFromMe.</span></span>  <br/> |
|<span data-ttu-id="56c40-146">ErrorInvalidPropertyForOperation</span><span class="sxs-lookup"><span data-stu-id="56c40-146">ErrorInvalidPropertyForOperation</span></span>  <br/> |<span data-ttu-id="56c40-147">Работать с свойства элемента или папки, не поддерживаемые операции.</span><span class="sxs-lookup"><span data-stu-id="56c40-147">Act on a property of an item or folder that is not supported by the operation.</span></span>  <br/> |<span data-ttu-id="56c40-148">Обновление кода, не доступа к свойству с помощью операции, вызвавшей ошибку.</span><span class="sxs-lookup"><span data-stu-id="56c40-148">Updating your code to not access the property with the operation that caused the error.</span></span>  <br/> |
|<span data-ttu-id="56c40-149">ErrorInvalidPropertyRequest</span><span class="sxs-lookup"><span data-stu-id="56c40-149">ErrorInvalidPropertyRequest</span></span>  <br/> |<span data-ttu-id="56c40-150">Задает свойство в запросе, который не поддерживается для типа элемента.</span><span class="sxs-lookup"><span data-stu-id="56c40-150">Specify a property in the request that is not supported for the item type.</span></span>  <br/> |<span data-ttu-id="56c40-151">Обновление кода, не пытается получить доступ к свойству с помощью операции.</span><span class="sxs-lookup"><span data-stu-id="56c40-151">Updating your code to not try to access the property with the operation.</span></span>  <br/> |
|<span data-ttu-id="56c40-152">ErrorInvalidPropertySet</span><span class="sxs-lookup"><span data-stu-id="56c40-152">ErrorInvalidPropertySet</span></span>  <br/> |<span data-ttu-id="56c40-153">Необходимо задайте свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="56c40-153">Set a read-only property.</span></span>  <br/> |<span data-ttu-id="56c40-154">Обновление кода, не пытайтесь задать свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-154">Updating your code to not try to set the property.</span></span>  <br/> |
|<span data-ttu-id="56c40-155">ErrorInvalidValueForProperty</span><span class="sxs-lookup"><span data-stu-id="56c40-155">ErrorInvalidValueForProperty</span></span>  <br/> |<span data-ttu-id="56c40-156">Сравните значение свойства в качестве ограничения поиска, где значение сравнения не соответствует тип свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-156">Compare a property value in a search restriction where the comparison value does not match the property type.</span></span>  <br/> |<span data-ttu-id="56c40-157">Обновление кода на наличие Несоответствие типа свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-157">Updating your code to check for property type mismatch.</span></span>  <br/> |
|<span data-ttu-id="56c40-158">ErrorItemSavePropertyError</span><span class="sxs-lookup"><span data-stu-id="56c40-158">ErrorItemSavePropertyError</span></span>  <br/> |<span data-ttu-id="56c40-159">Сохраните значения недопустимые свойства элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="56c40-159">Save an item or folder with invalid property values.</span></span>  <br/> |<span data-ttu-id="56c40-160">Проверка значений свойств и типы перед отправкой их в запросе.</span><span class="sxs-lookup"><span data-stu-id="56c40-160">Checking the property values and types before submitting them in a request.</span></span>  <br/> |
|<span data-ttu-id="56c40-161">ErrorNoFolderClassOverride</span><span class="sxs-lookup"><span data-stu-id="56c40-161">ErrorNoFolderClassOverride</span></span>  <br/> |<span data-ttu-id="56c40-162">Задайте класса папки на новую папку, которая не является типом основной папки.</span><span class="sxs-lookup"><span data-stu-id="56c40-162">Set the folder class on a new folder that is not the base folder type.</span></span>  <br/> |<span data-ttu-id="56c40-163">Задайте класса папки с помощью типа общей папки.</span><span class="sxs-lookup"><span data-stu-id="56c40-163">Using a generic folder type to set the folder class.</span></span>  <br/> |
|<span data-ttu-id="56c40-164">ErrorNoPropertyTagForCustomProperties</span><span class="sxs-lookup"><span data-stu-id="56c40-164">ErrorNoPropertyTagForCustomProperties</span></span>  <br/> |<span data-ttu-id="56c40-165">Ссылаться на дополнительное пользовательское свойство с его свойство тег.</span><span class="sxs-lookup"><span data-stu-id="56c40-165">Reference a custom extended property by its property tag.</span></span>  <br/> |<span data-ttu-id="56c40-166">Обновление кода ссылок на настраиваемые дополнительный идентификатор набора свойств, свойств и имя свойства или идентификатор свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-166">Updating your code to reference the custom extended property by property set identifier and either the property name or property dispatch identifier.</span></span>  <br/> |
|<span data-ttu-id="56c40-167">ErrorObjectTypeChanged</span><span class="sxs-lookup"><span data-stu-id="56c40-167">ErrorObjectTypeChanged</span></span>  <br/> |<span data-ttu-id="56c40-168">Установить или обновить класс элемента на элемент, который не совпадает с типом схемы.</span><span class="sxs-lookup"><span data-stu-id="56c40-168">Set or update the item class on an item that doesn't match with its schema type.</span></span>  <br/> |<span data-ttu-id="56c40-169">Обновление кода, чтобы класс элемента совпадает с типом элемента схемы.</span><span class="sxs-lookup"><span data-stu-id="56c40-169">Updating your code so that item class matches the item schema type.</span></span>  <br/> |
|<span data-ttu-id="56c40-170">ErrorPropertyUpdate</span><span class="sxs-lookup"><span data-stu-id="56c40-170">ErrorPropertyUpdate</span></span>  <br/> |<span data-ttu-id="56c40-171">Обновите свойство с недопустимое значение свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-171">Update a property with an invalid property value.</span></span>  <br/> |<span data-ttu-id="56c40-172">Проверка значения свойства перед отправкой в запросе [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="56c40-172">Checking the property value before submitting it in an [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) request.</span></span>  <br/> |
|<span data-ttu-id="56c40-173">ErrorRequiredPropertyMissing</span><span class="sxs-lookup"><span data-stu-id="56c40-173">ErrorRequiredPropertyMissing</span></span>  <br/> |<span data-ttu-id="56c40-174">Отправьте запрос CreateAttachment, где отсутствуют необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-174">Send a CreateAttachment request that is missing a required property.</span></span>  <br/> |<span data-ttu-id="56c40-175">Обновление кода, присвойте свойству отсутствующие в соответствии с путь свойства, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="56c40-175">Updating your code to set the missing property as specified by the property path returned in the response.</span></span>  <br/> |
|<span data-ttu-id="56c40-176">ErrorUnsupportedMapiPropertyType</span><span class="sxs-lookup"><span data-stu-id="56c40-176">ErrorUnsupportedMapiPropertyType</span></span>  <br/> |<span data-ttu-id="56c40-177">Используйте типы расширенных свойств тип объекта, массив объектов, ошибки или null.</span><span class="sxs-lookup"><span data-stu-id="56c40-177">Use extended property types of type object, object array, error or null.</span></span>  <br/> |<span data-ttu-id="56c40-178">Обновление кода, не используйте типы ограниченных расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="56c40-178">Updating your code to not use the restricted extended property types.</span></span>  <br/> |
|<span data-ttu-id="56c40-179">ErrorUnsupportedPathForQuery</span><span class="sxs-lookup"><span data-stu-id="56c40-179">ErrorUnsupportedPathForQuery</span></span>  <br/> |<span data-ttu-id="56c40-180">Используйте путь неподдерживаемые свойства в качестве ограничения поиска.</span><span class="sxs-lookup"><span data-stu-id="56c40-180">Use an unsupported property path in a search restriction.</span></span>  <br/> |<span data-ttu-id="56c40-181">Изменение ограничения поиска, чтобы исключить путь неподдерживаемые свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-181">Changing the search restriction to exclude the unsupported property path.</span></span>  <br/> |
|<span data-ttu-id="56c40-182">ErrorUnsupportedPathForSortGroup</span><span class="sxs-lookup"><span data-stu-id="56c40-182">ErrorUnsupportedPathForSortGroup</span></span>  <br/> |<span data-ttu-id="56c40-183">Используйте путь неподдерживаемые свойства в отсортированный или сгруппированные поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="56c40-183">Use an unsupported property path in a sorted or grouped search request.</span></span>  <br/> |<span data-ttu-id="56c40-184">Изменение ограничения поиска, чтобы исключить путь неподдерживаемые свойства.</span><span class="sxs-lookup"><span data-stu-id="56c40-184">Changing the search restriction to exclude the unsupported property path.</span></span>  <br/> |
|<span data-ttu-id="56c40-185">ErrorUnsupportedTypeForConversion</span><span class="sxs-lookup"><span data-stu-id="56c40-185">ErrorUnsupportedTypeForConversion</span></span>  <br/> |<span data-ttu-id="56c40-186">Тип свойства, которое не может быть преобразована XML для веб-служб Exchange для возврата в ответ на запрос.</span><span class="sxs-lookup"><span data-stu-id="56c40-186">Request a property type that cannot be converted to XML for EWS to return in a response.</span></span>  <br/> |<span data-ttu-id="56c40-187">Обновление кода, не запрашивать свойство не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56c40-187">Updating your code to not request the unsupported property.</span></span>  <br/> |
|<span data-ttu-id="56c40-188">ErrorUpdatePropertyMismatch</span><span class="sxs-lookup"><span data-stu-id="56c40-188">ErrorUpdatePropertyMismatch</span></span>  <br/> |<span data-ttu-id="56c40-189">Обновление элемента или папки Описание изменений, для которого не совпадает с свойство, заданный для обновления.</span><span class="sxs-lookup"><span data-stu-id="56c40-189">Update an item or folder the change description for which doesn't match the property that is specified to be updated.</span></span>  <br/> |<span data-ttu-id="56c40-190">Изменение кода, чтобы изменить описание совпадает с типом элемента или папки, которая обновляется.</span><span class="sxs-lookup"><span data-stu-id="56c40-190">Changing your code so that the change description matches the item or folder type that is being updated.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56c40-191">См. также</span><span class="sxs-lookup"><span data-stu-id="56c40-191">See also</span></span>


- [<span data-ttu-id="56c40-192">Свойства и расширенные свойства в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="56c40-192">Properties and extended properties in EWS in Exchange</span></span>](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [<span data-ttu-id="56c40-193">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="56c40-193">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="56c40-194">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="56c40-194">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
