# diagramme-de-classe-avec-implementation-C-
class Adherent 
{
    public string nom { get; set; }
    public int prenom { get; set; }
    public List<Emprunte> Emprunte { get; set; }

    public void Emprunter(Document doc) { /* Code pour emprunter un document */ }
    public void Retourner(Document doc) { /* Code pour retourner un document */ }
    public void ProlongerEmprunt(Emprunte emp) { /* Code pour prolonger un emprunt */ }
}

class Bibliotheque 
{
    public List<Document> Documents { get; set; }
    public List<Adherent> Adherents { get; set; }
    public List<Emprunte> Emprunts { get; set; }

    public void AjouterDocument(Document doc) { /* Code pour ajouter un document */ }
    public void SupprimerAdherent() { }
    public void AjouterAdherent() {  }
}

class Emprunte 
{
    public Adherent Adherent { get; set; }
    public Document Document { get; set; }
    public DateTime Date_Emprunt { get; set; }
    public DateTime Date_Retour { get; set; }
    public bool ProlongerDateRetour { get; set; }
}

class Document 
{
    public string Titre { get; set; }
    
}

class Journal : Document { 
    public DateTime date_parution {get; set;}
 }
class Volume : Document { 
    public string auteur {get; set;}
 }
class Livre : Document {
    public bool disponible { get; set; }
    public string auteur { get; set; }
    public string titre { get; set; }
     }
class BD : Document { 
    public string Dessinateur { get; set; }
}
class Dictionnaire : Document { 
    
 }
