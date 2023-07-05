# Imagen base para el runtime de .NET Core
FROM mcr.microsoft.com/dotnet/core/aspnet:3.1

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar los archivos de publicación del proyecto al contenedor
COPY bin/Release/netcoreapp3.1/publish/ .

# Exponer el puerto en el que se ejecutará la aplicación
EXPOSE 5000

# Especificar el comando de inicio de la aplicación
ENTRYPOINT ["dotnet", "ProyectoBackend.dll"]
