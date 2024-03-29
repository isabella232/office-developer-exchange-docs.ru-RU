---
title: Ошибки, связанные со свойствами EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 1c4c5969-7bdd-4021-be0e-cae99e86cf2c
description: Узнайте, как обрабатывать ошибки, связанные с свойством, в приложении EWS.
ms.openlocfilehash: 019a13116ae9a08c19381b78e1fd38c26f50c0d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512270"
---
# <a name="ews-property-related-errors"></a>Ошибки, связанные со свойствами EWS

Узнайте, как обрабатывать ошибки, связанные с свойством, в приложении EWS.
  
Большинство клиентских приложений EWS будут использовать свойства, а это значит, что вам придется обрабатывать ошибки, связанные с свойством. Вы можете обрабатывать эти ошибки во время работы или во время разработки приложения EWS.
  
**Таблица 1. Ошибки, связанные с собственностью, и их обработка**

|**Ошибка**|**Вызвано попыткой...**|**Обработать его...**|
|:-----|:-----|:-----|
|ErrorDataSizeLimitExceeded  <br/> |Установите свойство со значением, которое превышает максимальный размер для свойства или свойство не поддерживает потоковую передачу, например свойства папок.  <br/> |Ограничение размера данных, установленных в свойстве.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Получите свойство, которое не удалось получить.  <br/> |Указывает, что свойство не может быть извлечено.  <br/> |
|ErrorInvalidExtendedProperty  <br/> |Установите недействительное сочетание значений расширенного свойства или приводит к недействительным расширенному идентификатору ресурсов единого свойства (URI).  <br/> |Проверка расширенного значения свойства.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Установите расширенное значение свойства, которое не соответствует указанному типу  <br/> |Обновление кода для проверки на соответствие типам.  <br/> |
|ErrorInvalidFolderId  <br/> |Установите структуру идентификатора папки в недействительную форму.  <br/> |Только с помощью идентификаторов, возвращенных EWS.  <br/> |
|ErrorInvalidId  <br/> |Установите структуру идентификатора и/или измените ключ на недействительный вид.  <br/> |Только с помощью идентификаторов, возвращенных EWS.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Установите пустой идентификатор.  <br/> |Настройка идентификатора с допустимым элементом или идентификатором папок.  <br/> |
|ErrorInvalidMalformed  <br/> |Установите структуру идентификатора и/или измените ключ на недействительный вид.  <br/> |Только с помощью идентификаторов, возвращенных EWS.  <br/> |
|ErrorInvalidPropertyAppend  <br/> |Приложение свойства, которое не поддерживает приложение.  <br/> |Обновление кода таким образом, чтобы он пытался только при добавлении значений к свойствам коллекции получателей (To, Cc, Bcc), свойствам коллекции Attendee (Required, Optional, Resources), свойству Body и свойству ReplyTo.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Удаление свойства, которое не поддерживает удаление.  <br/> |Обновление кода, чтобы не пытаться удалить свойство. Например, нельзя удалить папку и идентификаторы элементов.  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Установите ограничение поиска на основе экзистенциального на основе флага.  <br/> |Обновление кода, чтобы не использовать свойства на основе флага в ограничении поиска на основе экзистенциальных данных. Свойства на основе флага: IsDraft, IsSubmitted, IsUnmodified, IsResend и IsFromMe.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Действие свойства элемента или папки, не поддерживаемого операцией.  <br/> |Обновление кода, чтобы не получить доступ к свойству с помощью операции, вызвавшего ошибку.  <br/> |
|ErrorInvalidPropertyRequest  <br/> |Укажите свойство в запросе, который не поддерживается для типа элемента.  <br/> |Обновление кода, чтобы не пытаться получить доступ к свойству с помощью операции.  <br/> |
|ErrorInvalidPropertySet  <br/> |Установите свойство только для чтения.  <br/> |Обновление кода, чтобы не пытаться установить свойство.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Сравните значение свойства в ограничении поиска, где значение сравнения не соответствует типу свойства.  <br/> |Обновление кода для проверки несоответствия типа свойства.  <br/> |
|ErrorItemSavePropertyError  <br/> |Сохраните элемент или папку с недействительными значениями свойств.  <br/> |Проверка значений и типов свойств перед отправкой их в запросе.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Установите класс папки в новой папке, которая не является базовым типом папки.  <br/> |Использование типовой папки для набора класса папок.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Ссылка на пользовательское расширенное свойство по тегу свойства.  <br/> |Обновление кода для ссылки на пользовательское расширенное свойство по идентификатору набора свойств и либо имени свойства или идентификатора отправки свойств.  <br/> |
|ErrorObjectTypeChanged  <br/> |Установите или обновим класс элемента на элементе, который не соответствует типу схемы.  <br/> |Обновление кода таким образом, чтобы класс элемента совпадал с типом схемы элемента.  <br/> |
|ErrorPropertyUpdate  <br/> |Обновление свойства с недействительным значением свойства.  <br/> |Проверка значения свойства перед отправкой его в [запрос UpdateItem.](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Отправьте запрос CreateAttachment, в результате чего отсутствует необходимое свойство.  <br/> |Обновление кода, чтобы установить недостающее свойство, указанное путем свойства, возвращаемого в ответе.  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Используйте расширенные типы свойств объекта типа, массива объектов, ошибок или null.  <br/> |Обновление кода, чтобы не использовать ограниченные расширенные типы свойств.  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Используйте неподтверченный путь свойств в ограничении поиска.  <br/> |Изменение ограничения поиска, чтобы исключить неподтверченный путь свойства.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Используйте неподтверченный путь свойства в отсортировали или сгруппировали запрос на поиск.  <br/> |Изменение ограничения поиска, чтобы исключить неподтверченный путь свойства.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Запрос типа свойства, который не может быть преобразован в XML для EWS, чтобы вернуться в ответ.  <br/> |Обновление кода, чтобы не запрашивать неподтверченное свойство.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Обнови элемент или папку, описание изменений для которого не соответствует свойству, указанному для обновления.  <br/> |Изменение кода таким образом, чтобы описание изменений совпадает с типом обновляемого элемента или папки.  <br/> |
   
## <a name="see-also"></a>См. также


- [Свойства и расширенные свойства в веб-службах Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

