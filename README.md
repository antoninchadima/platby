# platby

## Obsah

[TOC]



## Právní rámec

### Zákon o hazardních hrách č. 186/2016 Sb.

#### § 76 Podmínky účasti

1. Podmínkou účasti na internetové hře je registrace, nejde-li o případ podle § 77 odst. 4.
   `Hrát za peníze je možné jen s trvalým hráčským účtem, vyjímkou je dočasný hráčský účet.`
2. ...
3. ...
4. ...
5. ...

#### § 77 Registrace

1. Pro účely registrace je osoba žádající o registraci povinna

   a) ...

   b) ...

   c) poskytnout provozovateli potřebné údaje o platebním účtu nebo platební kartě podle § 78.
   `Bez platebního účtu nebo platební karty není možné hráčský účet povýšit z dočasného na trvalý.`

2. K registraci dojde aktivací trvalého uživatelského konta po ověření a potvrzení údajů uvedených v odstavci 1.
   `Platební účet nebo platební karta musí být ověřena, že patří majiteli hráčského účtu.`

3. ...

4. Do okamžiku registrace zřídí provozovatel účastníkovi hazardní hry dočasné uživatelské konto.

5. Registraci nelze provést po uplynutí 30 dnů ode dne, kdy osoba požádala o registraci.
   `Po uplynutí 30dnů je potřeba dočasný účet zablokovat, převést peníze zpět smazat a `

6. ...

#### § 78 Registrovaný platební účet a platební karta

1. Pro účely registrace je osoba žádající o registraci povinna uvést

   a) číslo nebo jiný jedinečný identifikátor platebního účtu, jehož je majitelem, a ze kterého bude, výhradně, s výjimkou uvedenou v § 79 a 80, na uživatelské konto převádět peněžní prostředky a na který bude výhradně z uživatelského konta přijímat peněžní prostředky (dále jen „registrovaný platební účet“), nebo

   b) číslo nebo jiný jedinečný identifikátor platební karty nebo jiného platebního prostředku, jejichž je držitelem, a ze kterých bude, výhradně, s výjimkou uvedenou v § 79 a 80, na uživatelské konto převádět peněžní prostředky a na které bude výhradně z uživatelského konta přijímat peněžní prostředky (dále jen „registrovaná platební karta“), tak, aby ji na základě tohoto čísla nebo tohoto identifikátoru bylo možno identifikovat jako majitele registrovaného platebního účtu nebo držitele registrované platební karty.

2. Registrovaným platebním účtem může být pouze platební účet vedený u osoby, která je oprávněna poskytovat platební služby v členském státě Evropské unie nebo ve státě, který je smluvní stranou Dohody o Evropském hospodářském prostoru.
3. Registrovanou platební kartou může být pouze platební karta vydaná osobou, která je oprávněna poskytovat platební služby v členském státě Evropské unie nebo ve státě, který je smluvní stranou Dohody o Evropském hospodářském prostoru.

#### § 79 Vícezdrojové financování internetové hry

...
`pravidla pro vkládání hotovosti např. fyzicky na herně`

#### § 80 Dočasné uživatelské konto

1. Dočasné uživatelské konto může být aktivní nejdéle 30 dní.
2. Během doby, kdy je dočasné uživatelské konto aktivní, nesmí celkový vklad přesáhnout částku 3000 Kč, a to ani v součtu jednotlivých vkladů.
3. Z dočasného uživatelského konta nelze vybírat vložené vklady nebo výhry.
4. Dojde-li k registraci účastníka hazardní hry, je provozovatel povinen převést evidované peněžní nebo hrací prostředky z jeho dočasného uživatelského konta na jeho uživatelské konto.
5. Nedojde-li k registraci účastníka hazardní hry, je provozovatel povinen mu vrátit nevyčerpaný vklad nejpozději do 7 dnů ode dne zrušení jeho dočasného uživatelského konta.

### PCI DSS

If you have enabled payments via credit cards, you are obliged to be PCI DSS compliant. You should annually complete a Self-Assessment Questionnaire (SAQ) and conduct on a quarterly basis network scan by an Approved Scan Vendor (ASV). Additionally if you process over 6 million card transactions annually you should complete Report on Compliance (ROC) by Qualified Security Assessor (QSA). You can find more information at [Security Standards Council](https://www.pcisecuritystandards.org/merchants/).

> Potřebujeme splňovat standard PCI DSS (Payment Card Industry Data Security Standard), případně další normy a osvědčení podle požadavků karetních asociací a objemu zpracovávaných peněžních prostředků. Dodržování standardu PCI DSS je povinné pro všechny organizace, které zpracovávají, přenášejí nebo uchovávají data z platebních karet, a je vyžadováno bankami po celém světě. Tato mezinárodní norma totiž určuje, jak s informacemi správně nakládat, aby zůstaly v bezpečí. Pravděpodobně ale nebudeme potřebovat i certifikovat na normu PCI DSS.

## Use case

### Dočasný účet

#### První platba

##### Platební karta

Hráč **na stránkách online casina** zadá **částku**, **číslo karty**, **platnost karty do** a **kontrolní kód CVV2/CVC2**. Zároveň souhlasí s uložením karty pro opakované použití. Dále je potřeba již v tomto formuláři dle obchodních podmínek zobrazit logo PayU a loga osvědčení/karetních asociací dle požadavku bank zpracovavajích požadavky PayU a karetních asociací.

If you have enabled payments via credit cards, you are obliged to be PCI DSS compliant. You should annually complete a Self-Assessment Questionnaire (SAQ) and conduct on a quarterly basis network scan by an Approved Scan Vendor (ASV). Additionally if you process over 6 million card transactions annually you should complete Report on Compliance (ROC) by Qualified Security Assessor (QSA). You can find more information at [Security Standards Council](https://www.pcisecuritystandards.org/merchants/).

> Potřebujeme splňovat standard PCI DSS (Payment Card Industry Data Security Standard), případně další normy a osvědčení podle požadavků karetních asociací a objemu zpracovávaných peněžních prostředků. Dodržování standardu PCI DSS je povinné pro všechny organizace, které zpracovávají, přenášejí nebo uchovávají data z platebních karet, a je vyžadováno bankami po celém světě. Tato mezinárodní norma totiž určuje, jak s informacemi správně nakládat, aby zůstaly v bezpečí. *A je potřeba ověřit* zda budeme potřebovat i certifikovat na normu PCI DSS.

## Implementace

### Dočasný účet

#### První platba

##### Platební karta

**Slepá cesta:**

Pro účely hazardu je potřeba ověřit zda je registrovaný hráč držitelem zadané platební karty. Proto se na první pohled jeví, že nejsou standardní způsoby platby kartou, PayU hosted payment form, PayU hosted inline widget, PayU hosted pop-up widget a  Custom payment form použitelné. A nabízí se, že je použitelný jenom tzv. Card data in plain text a transparentní white label integrace, kdy by se posílala i volitelná položka vlastníka karty do platební brány, následně by se sledovalo  zda platba s daným vlastníkem projde a data ke kartě by se ukládala na straně provozovatele. Tento způsob ale je problematický v tom, že by na provozovateli ponechal odpovědnost za veškerá data o platebních kartách.

**Správný způsob:**

Při analýze platební brány společnosti Sazka a.s. je ale vidět, že využívají nejpoužívanější metodu PayU hosted pop-up widget a kreditní karty pro opakované použití ukládají na straně PayU spárované s hráčovým emailem. Widget zasílá data platební karty na PayU a dostane zpět token pro jednorázové použití. Pomocí POST metody se odešle tento jednorázový token zpět do online casina (PHP SDK). Odtamtud se pak odešle požadavek platby a získá informace o stavu platby. Příklad odesílaných dat do online casina a tokenu:

```json
value:"TOK_1IOPVS7EMKVT4GYvs44XPxAOb8yc",
maskedCard:"424242******4242",
tokenType:"STANDARD",
type:"CARD_TOKEN"
```

Diagram komunikace:



Dokumentace k tomuto způsobu platby je k nalezení [na strankách PayU](http://developers.payu.com/en/payu_express.html#payu_express_front_widget). Dokumentace parametrů a způsobu vypočítání SIG je pak [zde](http://developers.payu.com/en/payu_express.html#payu_express_widget) (SHA256 funkce nad zřetězenými parametry spolu s privátním klíčem). Příklad parametrů:

```html
<script
    src="https://secure.payu.com/front/widget/js/payu-bootstrap.js"
    pay-button="#pay-button"
    merchant-pos-id="145227"
    shop-name="Casino Kartáč"
    total-amount="9.99"
    currency-code="CZK"
    customer-language="cs"
    store-card="true"
    recurring-payment="true"
    widget-mode="pay"
    customer-email="antonin.chadima@leris.cz"
    sig="6c9bb18db84165f53b5918380833723bc5fbb95ec5a9b73a4cb02dd60c11c64e">
</script>
```

Platbu je potřeba provést jako auto-receive disabled. Tento způsob chování platební brány je potřeba nastavit v ovládacím panelu obchodního účtu PayU. Každá příchozí platba z PayU musí být potvrzena nebo zrušena. Pokud nedojde k potvrzení přijetí platby ze strany online kasina je platba pro platební karty automaticky zamítnuta po uplynutí [5ti dnů](http://developers.payu.com/en/overview.html#paymethods). Toto chování jez hlediska právních vztahů správné, a zajišťuje abychom nepřijmuli platbu z platební karty, u které by nebyl majitelem registrovaný hráč.

Diagram stavu platby:

a tady začíná malé velké peklo - jak se proboha dozvědí od PayU kdo je majitelem platební karty - vím že to normálně nejde (drivejsi praxe a bojovani se shopcentrikem coz je ostatne vlastneny stejnou firmou jako payU...) 

Transaction data retrieve totiz nabizi pro karty jen - a vraceni jmena majitele uctu se bere za unik osobnich dat...

```json
{
  "transactions": [
    {
      "payMethod": {
        "value": "c"
      },
      "paymentFlow": "FIRST_ONE_CLICK_CARD",
      // also CARD, MASTERPASS, VISA_CHECKOUT, ONE_CLICK_CARD, ONE_CLICK_CARD_RECURRING etc.
      "card": {
        "cardData": {
          "cardNumberMasked": "543402******4014",
          "cardScheme": "MC", //MC (MasterCard/Maestro), VS (Visa)
          "cardProfile": "CONSUMER", // CONSUMER lub BUSINESS
          "cardClassification": "DEBIT", //DEBIT lub CREDIT
          "cardResponseCode":"000", //details are described below
          "cardResponseCodeDesc":"000 - OK",//details are described below
          "cardEciCode":"5",//details are described below
          "card3DsStatus":"AY", //details are described below
          "cardBinCountry":"PL",
          "firstTransactionId": "MCC0111LL1121"
        }
      }
    }
  ]
}
```

