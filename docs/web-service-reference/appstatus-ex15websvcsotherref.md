---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: Значение элемента AppStatus указывает состояние почтового приложения.
ms.openlocfilehash: 69f481b197db513761b97d4fbba38452bbb4a9a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525318"
---
# <a name="appstatus"></a>AppStatus

Значение **элемента AppStatus** указывает состояние почтового приложения. 
  
```XML
<AppStatus/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Метаданные](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **AppStatus** указывает состояние почтового приложения. Если пользователь может устранить проблему, связанную со состоянием почтового приложения, элемент [ActionUrl](actionurl.md) предоставляет URL-адрес для выполнения исправления. 
  
**Таблица 1. Значения AppStatus**

|**Значение**|**Описание**|
|:-----|:-----|
|Null или 0  <br/> |Почтовое приложение имеет здоровый статус.  <br/> |
|1.0  <br/> |Приложение почты не может быть автоматически обновлено. Почтовое приложение необходимо повторно установить из Office Store.  <br/> |
|1.1  <br/> |Приложение почты не может быть автоматически обновлено. Почтовое приложение требует дополнительных разрешений, а для этого требуется проверка и подтверждение для установки.  <br/> |
|1.2  <br/> |Приложение для почты не удалось обновить автоматически. Срок действия текущей лицензии истек или является недействительным. Обновление почтового приложения из Office Store.  <br/> |
|2.0  <br/> |Лицензия почтового приложения не может быть автоматически обновлена. Лицензия для почтового приложения должна быть восстановлена из Office Store.  <br/> |
|2.1  <br/> |Лицензия почтового приложения не может быть автоматически обновлена. Срок действия текущей лицензии истек. Новая лицензия для этого приложения должна быть установлена из Office Store.  <br/> |
|3.0  <br/> |Статус Office магазина для почтового приложения изменился. Это может указывать на то, что существует проблема с почтовым приложением. Дополнительные сведения перейдите на страницу приложения почты в Office Store.  <br/> |
|3.1  <br/> |Почтовое приложение удалено из Office Store.  <br/> |
|3.2  <br/> |В почтовом приложении обнаружена проблема, которая временно была снята из Office Store.  <br/> |
|3.3  <br/> |Почтовое приложение будет удалено из магазина Office в течение 30 дней.  <br/> |
|4.0  <br/> |Почтовое приложение автоматически отключено клиентом почты.  <br/> |
|4.1  <br/> |Почтовое приложение было отключено Outlook по соображениям производительности.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Неприменимо  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Метаданные](metadata-ex15websvcsotherref.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

