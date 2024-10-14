# VIS Projekt KAL0326 - Rezervace Klubů

## Proč
- Zákazník potřebuje nový informační systém, protože dosavadní rezervace klubů probíhaly komplikovaně a neefektivně.

## Co
- Systém bude obsahovat databázi klubů, které s námi budou ochotni spolupracovat. Databáze bude spojena s webovou stránkou, na které si registrovaný uživatel bude moct vyhledat a vybrat klub podle zadaných kategorií. 
- Systém umožní uživateli rezervaci klubu na zadané datum a čas. 
- Dále bude mít každý uživatel k dispozici jeho historii rezervací a plateb. 

## Kdo
### Registrovaný uživatel 
- Osoba, která chce pronajmout klub a používat služby systému pro rezervaci klubu na určité datum a čas. 
### Neregistrovaný uživatel 
- Osoba, která si nebude moct pronajmout klub, ale bude se moct podívat na nabídku klubů. 
### Majitel klubu
- Bude spolupracovat s tímto systémem a bude zveřejňovat informace o klubu v databázi.  
- Bude také přijímat rezervace a platby od zákazníků. 
### Správce systému 
- Osoba nebo tým, který bude spravovat systém a databázi klubů. 
- Bude také řešit technické a provozní záležitosti, jako je zabezpečení systému a udržování dostupnosti pro uživatele.

## Kde
- Celý systém bude běžet na nově vytvořené webové stránce. 
- Webová stránka bude komunikovat s databází, která slouží jako centrální uložiště všech klubů a všech podrobností o nich.
- Dále bude webová stránka komunikovat s platební bránou, která bude umožňovat rychlou a bezpečnou online platbu rezervací. 

## Kdy
- Systém bude využíván při rezervaci klubů a správě uživatelských účtů.

## Jak
- Systém bude vyvíjen agilním způsobem (viz. obrázek níže).

![Alt text](VIS_agile.png)

# Usecases
## Obrázek

![Alt text](Usecases.png)

## Use Case 3
### Název: Vytvořit rezervaci
- Aktéři: Uživatel, Systém
- Vstupní podmínky: Uživatel musí být registrovaný a přihlášený v systému a klub, který si vybral, musí existovat v databázi
- Spouštěč: Uživatel si chce rezervovat klub na dané datum a čas
- Úspěšný scénář:
  1. Uživatel se přihlásí do systému a chce podle zadaných podmínek vyhledat vhodný klub.
  2. Systém zpracuje požadavky uživatele a vrátí podle nich vyhovující kluby.
  3. Uživatel vybere ze seznamu klub
  4. Systém ověří dostupnost klubu na zvolené datum a čas a zobrazí uživateli rezervační formulář
  5. Uživatel vyplní rezervační formulář a bude chtít vytvořit rezervaci
  6. Systém zobrazí potvrzení rezervace a požádá uživatele o potvrzení.
  7. Uživatel potvrdí rezervaci.
  8. Systém odešle potvrzení rezervace uživateli a klubu.
  9. Systém vytvoří záznam o rezervaci v databázi a převede uživatele na platební bránu.
  10. Uživatel provede platbu.

### Aktivitní diagram pro Use Case 3
![Alt text](activityDiagramReservation.png)

## Use Case 7 
### Název: Stornování rezervace
- Aktéři: Uživatel, Systém
- Vstupní podmínky: Uživatel musí být registrovaný a přihlášený v systému a rezervace, kterou chce stornovat, musí v databázi existovat
- Spouštěč: Uživatel chce stornovat již vytvořenou rezervaci
- Úspěšný scénář:
  1. Uživatel se přihlásí do systému.
  2. Uživatel klikne na položku „Historie Rezervací“.
  3. Systém zpracuje požadavek uživatele a vrátí mu všechny rezervace, které uživatel vytvořil.
  4. Uživatel vybere rezervaci, kterou chce stornovat.
  5. Systém vytvoří záznam o stornování rezervace.
  6. Systém odešle potvrzení o stornování rezervace uživateli a klubu.
  7. Uživatel vidí stornovanou rezervaci v jeho historii rezervací.

## Use Case 1
### Název: Vyhledat kluby
- Aktéři: Uživatel, Systém
- Vstupní podmínky: : Uživatel zadá všechny potřebné požadavky pro vyhledávání
- Spouštěč: Uživatel chce vyhledat vhodný klub
- Úspěšný scénář:
  1. Uživatel chce vyhledat vhodné kluby podle jeho požadavků.
  2. Uživatel zadá všechny požadavky a klikne na tlačítko „Vyhledat Kluby“.
  3. Systém požadavky zpracuje a podle nich zobrazí uživateli vyhovující kluby.
  4. Uživateli se zobrazí kluby, které vyhovují jeho požadavkům.

  
