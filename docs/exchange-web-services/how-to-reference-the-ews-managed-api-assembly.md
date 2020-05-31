---
title: Ссылка на сборку управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Сведения о том, как ссылаться на сборку управляемого API EWS.
ms.openlocfilehash: a08ce43d139440186f611049fa1e457ea44f0362
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353688"
---
# <a name="reference-the-ews-managed-api-assembly"></a>Ссылка на сборку управляемого API EWS

Сведения о том, как ссылаться на сборку управляемого API EWS.
  
Управляемый API EWS предоставляет простой и полнофункциональный интерфейс для разработки и расширения приложений, использующих веб-службы Exchange (EWS). Если вы используете Visual Studio или другой редактор кода для разработки приложения управляемого API EWS, вам потребуется создать ссылку на сборку управляемого API EWS. Если вы еще не установили управляемый API EWS, обязательно [Скачайте API](http://aka.ms/ews-managed-api-readme).
  
> [!NOTE]
> Управляемое API EWS теперь доступно в качестве проекта с открытым кодом на [GitHub](https://github.com/officedev/ews-managed-api). Вы можете использовать библиотеку открытого кода, чтобы: 
> - добавлять исправления ошибок и улучшения в API; 
> - получать исправления ошибок и улучшения до того, как они станут доступны в официальном выпуске; 
> - получать доступ к самой полной и актуальной реализации API, которую можно использовать для справки или для создания новых библиотек на новых платформах.
> 
>  Мы будем рады вашему [вкладу](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) в GitHub. 
  
## <a name="referencing-the-assembly"></a>Ссылка на сборку

Наиболее распространенный способ добавления ссылки — использование Visual Studio. Мы знаем, что некоторые разработчики хотели бы использовать другие редакторы, поэтому мы предоставляем инструкции по использованию компилятора командной строки, а также инструкции по использованию Visual Studio. Вы можете заметить, что в приведенных ниже примерах кода **используются** одни и те же операторы using. Разница между этими двумя методами состоит в том, что компилятору командной строки требуется расположение файла сборки. Справка по Visual Studio обрабатывает это в фоновом режиме. 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a>Добавление ссылки с помощью Visual Studio

1. Поместите файл Microsoft. Exchange. WebServices. dll и Microsoft. Exchange. WebServices. XML в выбранную папку. По умолчанию файлы установлены в `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, но их можно хранить в любом месте на компьютере.
    
2. В области Обозреватель решений в Visual Studio выберите **ссылки**, а затем нажмите кнопку **Добавить ссылку**. Откроется окно Добавить ссылку.
    
3. В окне Добавить ссылку перейдите на вкладку **Обзор** , перейдите к расположению файла Microsoft. Exchange. WebServices. dll, выберите этот файл и нажмите кнопку **ОК**. 
    
4. Чтобы использовать управляемый API EWS в приложении, добавьте инструкцию **using** для пространства имен **Microsoft. Exchange. WebServices. Data** . 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a>Добавление ссылки и построение приложения с помощью компилятора командной строки

1. Поместите файл Microsoft. Exchange. WebServices. dll в выбранную папку. Эта папка будет выходной папкой для компилятора.
    
2. В редакторе исходного кода добавьте оператор **using** в исходный код для пространства имен **Microsoft. Exchange. WebServices. Data** . 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. Запустите компилятор командной строки, чтобы создать приложение. Следующая команда использует компилятор C# .NET Framework для создания приложения Windows, определенного в файле исходного кода "program.cs". Предполагается, что компилятор находится в каталоге установки по умолчанию, а файл Microsoft. Exchange. WebServices. DLL находится в подкаталоге текущего каталога с именем "Build".
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a>См. также

- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md)    
- [Настройка среды разработки приложений Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Взаимодействие с EWS с помощью управляемого API EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

