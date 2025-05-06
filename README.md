 Gegevensinname met een pipeline in Microsoft Fabric

Beschrijving:
In deze oefening implementeer je een ETL-proces (Extract, Transform, Load) met behulp van Microsoft Fabric. Je maakt gebruik van een pipeline en een Spark-notebook om gegevens van een externe bron in een lakehouse te laden, te transformeren en op te slaan in een tabel.

Stappenplan:

Workspace maken

Ga naar https://app.fabric.microsoft.com

Maak een nieuwe workspace aan met Fabric-triallicentie.

Lakehouse aanmaken

Maak een nieuw lakehouse aan in de workspace.

Voeg een submap toe onder "Files" met de naam new_data.

Pipeline aanmaken: "Ingest Sales Data"

Voeg een Copy Data activiteit toe die gegevens van de volgende URL kopieert:
https://raw.githubusercontent.com/MicrosoftLearning/dp-data/main/sales.csv

Sla het bestand op in de map Files/new_data/sales.csv.

Notebook aanmaken: "Load Sales"

Lees de CSV in met Spark.

Voeg kolommen "Year", "Month", "FirstName", en "LastName" toe.

Filter en herordeneer de kolommen.

Sla het resultaat op in een Delta-tabel genaamd sales.

Pipeline uitbreiden

Voeg een Delete Data activiteit toe om oude CSV-bestanden te verwijderen.

Voeg een Notebook activiteit toe die het notebook uitvoert en de gegevens laadt in een nieuwe tabel new_sales.

Resultaat controleren

Na het uitvoeren van de pipeline is de tabel new_sales zichtbaar in je lakehouse met getransformeerde gegevens.

Benodigdheden:

Microsoft Fabric met actieve triallicentie

Internetverbinding voor het ophalen van externe data
# Ingest-data-with-a-pipeline-in-Microsoft-Fabric
