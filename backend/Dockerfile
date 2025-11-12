#Basisimage
FROM python:3.11-slim           
#hier wird das Arbeitsverzeichnis gesetzt                            
WORKDIR /app  
#Kopiere Datei mit Liste an Abhängigkeiten ins Image                                              
COPY requirements.txt .       
#Installation der Abhängigkeiten                              
RUN pip install --no-cache-dir -r requirements.txt   
#Kopieren des restlichen Source Code       
COPY . .                
#Der Conmmand app.py soll zur Laufzeit des Container ausgeführt werden                                    
CMD ["python", "app.py"]