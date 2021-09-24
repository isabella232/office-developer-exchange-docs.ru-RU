---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: Элемент CreateManagedFolder определяет запрос на добавление управляемых пользовательских папок в почтовый ящик.
ms.openlocfilehash: ca6850cfdc8a37bf0480db0c040b035591a59ce6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536375"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

Элемент **CreateManagedFolder** определяет запрос на добавление управляемых пользовательских папок в почтовый ящик. 
  
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
|[FolderNames](foldernames.md) <br/> |Содержит массив именных управляемых папок, которые необходимо добавить в почтовый ящик.  <br/> |
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Учетная запись пользователя, который делает запрос, должна иметь разрешения FullAccess в почтовом ящике, где создаются управляемые папки. Чтобы назначить разрешение FullAccess, можно использовать параметр _-AccessRights _ с помощью Exchange управления shell **add-MailboxPermission.** 
  
Несмотря на Exchange веб-служб для добавления управляемых папок в почтовый ящик, вы не можете использовать Exchange-службы для доступа к списку доступных управляемых папок. Чтобы получить список доступных управляемых папок, используйте комлет **get-managedfolder** Exchange Management Shell. Список, возвращаемый комлетом **get-managedfolder,** будет содержать как управляемые пользовательские папки, так и управляемые папки по умолчанию. В почтовый ящик можно добавить папки типа **managedcustomfolder,** используя операцию CreateManagedFolder. 
  
> [!NOTE]
> Вы также можете получить список управляемых папок с помощью API DirectoryServices microsoft платформа .NET Framework. 
  
Операцию [FindFolder](findfolder-operation.md) можно использовать для поиска управляемых папок в почтовом ящике. Управляемые папки можно отличить, задав элемент [BaseShape](baseshape.md) allProperties в запросе. Ответ будет содержать элемент [ManagedFolderInformation,](managedfolderinformation.md) чтобы отличать управляемые папки от Exchange папок магазина. Вы можете удалять управляемые папки таким же образом, как и другие типы папок. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateManagedFolder](createmanagedfolder-operation.md)
  
[Операция FindFolder](findfolder-operation.md)


[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Добавление управляемых папок](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

