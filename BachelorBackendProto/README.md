# BachelorBackendProto

Backend-Service zur Bereitstellung der Test-APIs für die Bachelorarbeit  
**„Optimierung von Datenströmen zwischen Frontend und Backend: gRPC im Vergleich zu REST und GraphQL“**.

## Implementierte APIs
- **REST API** (ASP.NET Core Controller)
- **GraphQL API** (HotChocolate Framework)
- **gRPC Services**
- **gRPC-Web Services**

## Services
- **Text-Service** (klein, mittel, groß)  
- **Media-Service** (Foto, Audio, Video)  
- **Blog-Service** (verschachtelte Datenstruktur)

# Testdaten
Im Projektordner `Common/Payload` sind Strukturen für die Beispielinhalte vorbereitet:

- **Text**
  - `small.txt`
  - `medium.txt`
  - `large.txt`

- **Media**
  - `foto.jpg`
  - `music.wav`
  - `video.mp4`

- **Blog**
  - `BlogData.cs`
  - `BlogPost.cs`

Diese Dateien sind im Repository **nicht mit Inhalten befüllt**, um die Datenmenge klein zu halten.  
Falls der Prototyp getestet werden soll, müssen diese Inhalte (Texte, Bilder, Audio, Video) mit den oben angeführten Namen in die jeweiligen Ordner kopiert werden.

## Nutzung mit den Clients

### Web-Client
- Kommuniziert über **REST**, **GraphQL** und **gRPC-Web**  
- Dient zur Messung von End-zo-End-Latenz im Browser 

### Konsolen-Client
- Kommuniziert über **gRPC** (direkt, ohne Web-Layer)  
- Vergleich zwischen **gRPC** und **gRPC-Web** in einer Microservice-Architektur  

## Technologien
- **.NET 9**
- **ASP.NET Core**
- **HotChocolate GraphQL**
- **gRPC / gRPC-Web**
- **Protobuf**

## Starten
1. Repository klonen  
2. In das Backend-Verzeichnis des jeweiligen Projekts wechseln und Solution öffnen 
3. Build & Run:  
   dotnet restore
   dotnet build
   dotnet run
