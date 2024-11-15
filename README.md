# What is this repo about?
Idee war es ein Skript zu schreiben, welches automatisiert die Preise in unserem CRM anpasst. 

# Wie genau? 
1. Eine csv mit neuen Verkaufs wie auch Einkaufspreisen + jeweilige Artikel _ID 
2. Diese Csv wird in Python geladen und in ein DataFrame gepackt
3. get all relevant article Data via api (prices are nested in articles entity)
4. get all relevant article purchase price via api (nested in supply source entity)
5. update relevant data
6. upload all new data using requests.put()

# Warum wurde es gestoppt? 
Unser CRM bietet eine möglichkeit csv's mit paar klicks zu uploaden. Für diesen Case ist diese Möglichkeit effizienter. 