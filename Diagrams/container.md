# Container

```mermaid
C4Context
    title Container Diagram - Dinheiros S/A - Onboarding

    Enterprise_Boundary(banco,"Dinheiros S/A") {
        Person(backoffice, "backoffice", "Pessoa responsável por processos internos")
        Container(app-mobile, "Onboarding APP", "TypeScript, React Native", "App do banco")

    Container_Boundary(banco,"Dinheiros S/A") {        
            ContainerDb(mongodb, "Database", "MongoDB", "Armazena os dados das contas")
            ContainerDb(redis, "Cache", "Redis", "Armazena dados de cache")

            Container(api, "Onboarding API", "ASP NET 7", "Sistema para gerenciamento e Onboarding", "API")
            Container(app, "Onboarding Site", "JavaScript, Angular", "Sistema para gerenciamento e Onboarding via web browser")
        }
    }

    Container_Ext(documentos, "Documento OCR API", "", "Analisa e retorna dados das imagens dos documentos enviado")
    Container_Ext(notifications, "Sistema de notificações", "", "Notifica pessoas por e-mail e SMS")

    Person(cliente, "cliente", "Gerencia seu onboarding")

    Rel(api, mongodb, "Le e escreve dados no", "TCP")
    Rel(api, redis, "Le e escreve dados de cache no", "TCP")

    Rel(cliente, app, "Acessa", "HTTPS/JSON")
    Rel(cliente, app-mobile, "Acessa", "HTTPS/JSON")

    Rel(backoffice, app, "Acessa", "")
    Rel(backoffice, app-mobile, "Acessa", "")

    Rel(app, api, "Faz chamadas para API", "HTTPS/JSON")
    Rel(app-mobile, api, "Faz chamadas para API", "HTTPS/JSON")

    Rel(api, documentos, "Faz chamadas para API", "HTTPS/JSON")
    Rel(api, notifications,"Faz chamadas para API", "HTTPS/JSON")

    Rel(notifications, cliente, "Envia notificações para", "SMTP")
```