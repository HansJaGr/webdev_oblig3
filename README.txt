I oppgavebeskrivelsen står det at mobil-versjonene bare skal ha en kolonne. 
Jeg har demonstrert at jeg vet hvordan man gjør dette i signup.html, men har valgt å beholde to kollonner på visse steder, på det to andre sidene.
Dette er fordi det var sånn jeg designet wireframsene, og jeg ville holde meg nærmest mulig de. For å endre innholdet på index.html og products.html til å samsvare med oppgaven,
er det bare å endre på to css-linjer:
.main-content-products{ 
    display: grid;
    grid-template-areas: "left right";
    grid-template-columns: repeat(2, 1fr);
}
til 
.main-content-products{ 
    display: block;
    grid-template-areas: "left right";
    grid-template-columns: repeat(2, 1fr);
}

og

.horizontal-scroll{
    display: flex;
    flex-direction: row;
    align-self: flex-end;
    margin-left: auto;
}
til 
.horizontal-scroll{
    display: block;
    flex-direction: row;
    align-self: flex-end;
    margin-left: auto;
}

Altså, å endre display: grid; og display: flex; til displa: block;


