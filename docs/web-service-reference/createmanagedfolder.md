---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: Элемент CreateManagedFolder определяет запрос на добавление настраиваемых управляемых папок почтового ящика.
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761908"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

Элемент **CreateManagedFolder** определяет запрос на добавление настраиваемых управляемых папок почтового ящика. 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 **CreateManagedFolderRequestType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |Содержит массив именованных управляемые папки для добавления к почтовому ящику.  <br/> |
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Учетная запись пользователя, отправившего запрос необходимы разрешения FullAccess для почтового ящика, где создаются управляемых папок. Параметр _ _ - AccessRights можно использовать с помощью командной консоли Exchange **Add-MailboxPermission** используется для назначения разрешений FullAccess. 
  
Несмотря на то, что веб-служб Exchange можно использовать для добавления управляемых папок для почтового ящика, нельзя использовать веб-служб Exchange для доступа к списку управляемых папок, которые доступны. Для получения списка доступных управляемых папок, используйте командлет **get-managedfolder** Командная консоль Exchange. Список, который возвращается с помощью **командлета get-managedfolder** будет содержать управляемые настраиваемые папки и управляемые папки по умолчанию. Только могут добавлять папки из типа **managedcustomfolder** к почтовому ящику с помощью операции CreateManagedFolder. 
  
> [!NOTE]
> Список управляемых папок можно также получить с помощью API DirectoryServices платформы Microsoft .NET Framework. 
  
[Операция FindFolder](findfolder-operation.md) можно использовать для поиска управляемых папок в почтовом ящике. Управляемые папки можно отличить путем установки для параметра элемент [BaseShape](baseshape.md) AllProperties в запросе. Ответ будет содержать элемент [ManagedFolderInformation](managedfolderinformation.md) , чтобы отличать управляемых папок из папки хранилища Exchange. Управляемые папки можно удалить точно так же, удалить другие типы папки. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateManagedFolder](createmanagedfolder-operation.md)
  
[FindFolder Operation](findfolder-operation.md)


[Поиск папок](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

