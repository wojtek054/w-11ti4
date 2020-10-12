# w-11ti4
4TI

# Własne repozytorium kodu
 
```php
<?php
$servername = "localhost";
$username = "username";
$password = "password";
$dbname = "myDB";

// Create connection
$conn = new mysqli($servername, $username, $password, $dbname);
// Check connection
if ($conn->connect_error) {
  die("Connection failed: " . $conn->connect_error);
}

$sql = "SELECT id, firstname, lastname FROM MyGuests";
$result = $conn->query($sql);

if ($result->num_rows > 0) {
  // output data of each row
  while($row = $result->fetch_assoc()) {
    echo "id: " . $row["id"]. " - Name: " . $row["firstname"]. " " . $row["lastname"]. "<br>";
  }
} else {
  echo "0 results";
}
$conn->close();
?>
```

## Dokumentacja

Moja dokumantacja dotycząca pracy w domu na zajęciach tworzenie stron i aplikacji internetowych.
 
## Instalacja

Insatalacja została wykonana na zajęciach.
 
Możesz zanstalować to z kompozytorium:
 
```
https://github.com/wojtek054/w-11ti4
```
 
 
## Cel i funkcje
 
* Zbiór elementów pracy w domu
* Możliwość pomocy kolegów z zespołu projektowego
* Nadzór kierownika projektu
 
## Wkład projektowy
 
* Główny nadzór: https://github.com/wojtek054
* Kod projektu: https://github.com/wojtek054

 
## Licencja
 
Ten projekt jest udostępniony na licencji MIT. Szczegółowe informacje można znaleźć w dołączonym pliku LICENCJA.
 
## Autor
 
Wojtek Świniarski
