---
title: Проверить сертификат сервера для управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Узнайте, как создавать и ссылаться метод обратного вызова проверки сертификата таким образом, можно выполнять запросы управляемый API веб-служб Exchange на сервере Exchange.
ms.openlocfilehash: 13d7c51e55308b9e9997697a075c8a9e6b4f10d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761125"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="0ff42-103">Проверить сертификат сервера для управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="0ff42-103">Validate a server certificate for the EWS Managed API</span></span>

<span data-ttu-id="0ff42-104">Узнайте, как создавать и ссылаться метод обратного вызова проверки сертификата таким образом, можно выполнять запросы управляемый API веб-служб Exchange на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ff42-104">Learn how to create and reference a certificate validation callback method so that you can make EWS Managed API requests to an Exchange server.</span></span>
  
<span data-ttu-id="0ff42-105">По умолчанию, версии Exchange, начиная с Exchange 2007 с пакетом обновления 1 используйте самозаверяющий X509 сертификаты для проверки подлинности вызовов из веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ff42-105">By default, versions of Exchange starting with Exchange 2007 SP1 use self-signed X509 certificates to authenticate calls from EWS.</span></span> <span data-ttu-id="0ff42-106">При использовании управляемого интерфейса API веб-служб Exchange, необходимо создать метод обратного вызова проверки сертификата; в противном случае не удастся управляемый API EWS запросов.</span><span class="sxs-lookup"><span data-stu-id="0ff42-106">When you are using the EWS Managed API, you need to create a certificate validation callback method; otherwise, EWS Managed API requests will fail.</span></span> <span data-ttu-id="0ff42-107">При использовании службы автообнаружения вызов метода автообнаружения управляемого API EWS завершится с ошибкой **AutodiscoverLocalException** .</span><span class="sxs-lookup"><span data-stu-id="0ff42-107">If you are using the Autodiscover service, the call to the EWS Managed API Autodiscover method will fail with an **AutodiscoverLocalException** error.</span></span> <span data-ttu-id="0ff42-108">Если вы используете созданный web веб-прокси службы, также может потребоваться создать метод обратного вызова, в зависимости от способа создания прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="0ff42-108">If you are using a web-generated web service proxy, you might also have to create a validation callback method, depending on how the proxy is created.</span></span> 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a><span data-ttu-id="0ff42-109">Необходимые условия для создания метода обратного вызова проверки</span><span class="sxs-lookup"><span data-stu-id="0ff42-109">Prerequisites for creating a validation callback method</span></span>
<span data-ttu-id="0ff42-110"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="0ff42-110"></span></span>

<span data-ttu-id="0ff42-111">Чтобы настроить для проверки сертификата сервера, убедитесь, что выполняются следующие условия:</span><span class="sxs-lookup"><span data-stu-id="0ff42-111">To set up to validate a server certificate, ensure that the following are true:</span></span> 
  
- <span data-ttu-id="0ff42-112">Exchange server с помощью самозаверяющий сертификат для веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ff42-112">Your Exchange server is using a self-signed certificate for EWS.</span></span> <span data-ttu-id="0ff42-113">Если администратор установил действующего сертификата, который выполняет трассировку в корневой сертификат, не нужно создать метод обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="0ff42-113">If the administrator has installed a valid certificate that traces to a root certificate, you do not need to create a validation callback method.</span></span> 
    
- <span data-ttu-id="0ff42-114">Вы создаете управляемые приложения, которое содержит ссылку на следующие обязательные .NET Framework пространства имен:</span><span class="sxs-lookup"><span data-stu-id="0ff42-114">You are creating a managed application that includes a reference to the following required .NET Framework namespaces:</span></span> 
    
  - <span data-ttu-id="0ff42-115">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="0ff42-115">**System.Net**</span></span>
  - <span data-ttu-id="0ff42-116">**System.Net.Security**</span><span class="sxs-lookup"><span data-stu-id="0ff42-116">**System.Net.Security**</span></span>  
  - <span data-ttu-id="0ff42-117">**System.Security.Cryptography.X509Certificates**</span><span class="sxs-lookup"><span data-stu-id="0ff42-117">**System.Security.Cryptography.X509Certificates**</span></span>
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="0ff42-118">Пример: Метод обратного вызова проверки сертификата сервера для управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="0ff42-118">Example: Callback method to validate a server certificate for the EWS Managed API</span></span>
<span data-ttu-id="0ff42-119"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="0ff42-119"></span></span>

<span data-ttu-id="0ff42-120">В следующем примере кода показано, как создать X509 метод обратного вызова проверки по сертификатам для управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ff42-120">The following code example shows how to create an X509 certificate validation callback method for the EWS Managed API.</span></span> <span data-ttu-id="0ff42-121">Этот метод будет проверять X509 сертификатов и возвращать только значение true, если выполнено хотя бы одно из следующих критериев:</span><span class="sxs-lookup"><span data-stu-id="0ff42-121">This method will validate an X509 certificate and only return true when either of the following criteria are met:</span></span> 
  
- <span data-ttu-id="0ff42-122">Сертификат является допустимым и трассировки обратно в допустимый корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="0ff42-122">The certificate is valid and traces back to a valid root certificate.</span></span>    
- <span data-ttu-id="0ff42-123">Сертификат является допустимым и самозаверяющий на сервере, который возвращается его.</span><span class="sxs-lookup"><span data-stu-id="0ff42-123">The certificate is valid and is self-signed by the server that returned it.</span></span> 
    
> [!IMPORTANT]
> <span data-ttu-id="0ff42-124">В данном примере метод обратного вызова проверки сертификата предоставляет необходимый уровень безопасности для разработки и тестирования приложений управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ff42-124">The certificate validation callback method in this example provides sufficient security for development and testing of EWS Managed API applications.</span></span> <span data-ttu-id="0ff42-125">Тем не менее он может обеспечивать необходимый уровень безопасности для развернутого приложения.</span><span class="sxs-lookup"><span data-stu-id="0ff42-125">However, it might not provide sufficient security for your deployed application.</span></span> <span data-ttu-id="0ff42-126">Всегда следует убедиться в том, что метод обратного вызова проверки сертификата, используемого соответствует требованиям безопасности организации.</span><span class="sxs-lookup"><span data-stu-id="0ff42-126">You should always make sure that the certificate validation callback method that you use meets the security requirements of your organization.</span></span> 
  
```cs
      private static bool CertificateValidationCallBack(
         object sender,
         System.Security.Cryptography.X509Certificates.X509Certificate certificate,
         System.Security.Cryptography.X509Certificates.X509Chain chain,
         System.Net.Security.SslPolicyErrors sslPolicyErrors)
    {
      // If the certificate is a valid, signed certificate, return true.
      if (sslPolicyErrors == System.Net.Security.SslPolicyErrors.None)
      {
        return true;
      }
      // If there are errors in the certificate chain, look at each error to determine the cause.
      if ((sslPolicyErrors &amp; System.Net.Security.SslPolicyErrors.RemoteCertificateChainErrors) != 0)
      {
        if (chain != null &amp;&amp; chain.ChainStatus != null)
        {
          foreach (System.Security.Cryptography.X509Certificates.X509ChainStatus status in chain.ChainStatus)
          {
            if ((certificate.Subject == certificate.Issuer) &amp;&amp;
               (status.Status == System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.UntrustedRoot))
            {
              // Self-signed certificates with an untrusted root are valid. 
              continue;
            }
            else
            {
              if (status.Status != System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.NoError)
              {
                // If there are any other errors in the certificate chain, the certificate is invalid,
             // so the method returns false.
                return false;
              }
            }
          }
        }
        // When processing reaches this line, the only errors in the certificate chain are 
    // untrusted root errors for self-signed certificates. These certificates are valid
    // for default Exchange server installations, so return true.
        return true;
      }
      else
      {
     // In all other cases, return false.
        return false;
      }
    }

```

<span data-ttu-id="0ff42-127">Используйте класс **ServicePointManager** в пространстве имен.NET **System.Net** подключить метод обратного вызова проверки путем установки свойства **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="0ff42-127">You use the **ServicePointManager** class in the .NET **System.Net** namespace to hook up a validation callback method by setting the **ServerCertificateValidationCallback** property.</span></span> <span data-ttu-id="0ff42-128">Можно использовать код, представленный в следующем примере кода задается свойство **ServerCertificateValidationCallback** .</span><span class="sxs-lookup"><span data-stu-id="0ff42-128">You can use code similar to the following code example to set the **ServerCertificateValidationCallback** property.</span></span> 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a><span data-ttu-id="0ff42-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="0ff42-129">Next steps</span></span>
<span data-ttu-id="0ff42-130"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="0ff42-130"></span></span>

<span data-ttu-id="0ff42-131">После создания метода обратного вызова проверки для управляемого API EWS для получения точек подключения и пользователей и Настройка домена с сервера Exchange, можно использовать службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0ff42-131">After you have created the validation callback method for the EWS Managed API, you can use the Autodiscover service to get connection points and user and domain settings from an Exchange server.</span></span> <span data-ttu-id="0ff42-132">Дополнительные сведения см в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="0ff42-132">For more information, see the following articles:</span></span>
  
- [<span data-ttu-id="0ff42-133">Использование службы автообнаружения для поиска точек подключения</span><span class="sxs-lookup"><span data-stu-id="0ff42-133">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="0ff42-134">Получить параметры пользователя из Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="0ff42-134">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="0ff42-135">Получение параметров домена с сервера Exchange</span><span class="sxs-lookup"><span data-stu-id="0ff42-135">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a><span data-ttu-id="0ff42-136">См. также</span><span class="sxs-lookup"><span data-stu-id="0ff42-136">See also</span></span>

- [<span data-ttu-id="0ff42-137">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="0ff42-137">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)  
- [<span data-ttu-id="0ff42-138">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="0ff42-138">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    

