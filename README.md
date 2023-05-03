
# Backendutveckling och API:er #5: Authentisering i REST API + Mer teori om REST & RESTful

👋 Se Linus Rudbecks föreläsning från 2 maj ✅ 



### Innehåll denna workshop:

* Authentisering i REST API med kryptering av lösenord samt tokenisering med JWT
* Mer toeri om REST & RESTful


# 👩🏽‍💻 Övning: Skapa authentisering i REST API

Du bygger vidare på förra veckans workshop. Om du inte har en resurs för användare ```users``` så skapa den. Använd lämpliga inloggningsuppgifter som exempelvis namn, email och lösenord. 

Använd dig av en s.k ```auth-controller.js``` som har hand om att registrera en ny användare samt att logga in för en redan existerande. Använda```bcrypt``` fär att hasha lösenordet, samt även ange ett värde för att salta lösenordet. 

Använd dig av JWT för en tokenbaserad inloggning. Använd dig av detta paket [https://www.npmjs.com/package/jsonwebtoken
](https://www.npmjs.com/package/jsonwebtoken)

Skapa en middleware som tar emot en token och kontrollerar om användaren är inloggad. Använd denna middleware på de routes du vill ska vara inloggningssäkra. 

Följ Linus föreläsning eller använd dig av lämplig dokumentation på nätet.

### 💬 Diskutera authentisering
* Vad menas med hashing?
* Vad är ett salt?
* Hur använder man paketet bcrypt för att hasha och dekryptera ett lösenord?
* Vad är JWT? Vad är header, payload och signature? [https://jwt.io/](https://jwt.io/)
* Vad finns det för andra metoder att authentisera än att använda tokens?
* Vad finns det för tredje-parts alternativ samt ramverk för authentisering?

### Redovisning:
* Du redovisar ett REST API där man authentiserar en användare som får tillgång till en eller flera routes (routes som man inte har tillgång till om man inte är authentiserad.

***Om du inte kan delta på workshopen, redovisar du ovanstående nästkommande workshop***


# 💬 Teori om REST & RESTful

Diskutera/Skapa anteckningar inför kommande teorihandbok.

* Beskriv egenskaperna för HTTP-protokollet
* Grunden för REST API:er är HTTP-protokollet, vad menas med det?
* Vad är Richardson Maturity Model? Vad kännetecknar de fyra olika nivåerna i modellen?
* Vad är skillnaden mellan REST och RESTful?
* Vad är CORS? När bör man använda sig av CORS?
* Vad är versionering för att skapa API:er?
* Varför är det viktigt att dokumentera ett API?
