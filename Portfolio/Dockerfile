FROM ubuntu:latest

# Installieren Sie den Apache-Webserver und aktualisieren Sie das System
RUN apt-get update && apt-get install -y apache2 && apt-get clean

# Kopieren Sie die Webseite in das Image
COPY index.html /var/www/html/

# Öffnen Sie den Port 8080 für eingehende Verbindungen
EXPOSE 8080

# Starten Sie den Apache-Webserver
CMD ["apache2ctl", "-D", "FOREGROUND"]