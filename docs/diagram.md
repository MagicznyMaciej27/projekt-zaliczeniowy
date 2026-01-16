# diagram projektu (mermaid)

Poniżej diagram przepływu:

```mermaid
flowchart TD
    Start([Start])
    Menu[/Menu główne/]
    Add["Dodaj monetę"]
    Form["Formularz danych"]
    Save["Zapisz monetę"]
    List["Lista monet"]
    Filter["Filtruj / Szukaj"]
    End([Koniec])

    Start --> Menu
    Menu --> Add
    Menu --> List
    Add --> Form
    Form --> Save
    Save --> Menu
    List --> Filter
    Filter --> List
    List --> Menu
    Menu --> End