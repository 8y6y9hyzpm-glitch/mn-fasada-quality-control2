# MN Fasada Quality Control — početni prototip

Ovo je mobilno prilagođen frontend prototip za MN Fasada Consulting.

## Šta radi
- Bosanski / njemački prikaz
- Kontrolna tabla
- Evidencija objekata
- Evidencija kontrolnih pregleda
- Evidencija nedostataka i preporuka
- Evidencija nacrta izvještaja
- Navigacija prilagođena telefonu
- Demo unosi čuvaju se samo u lokalnom pregledniku (localStorage)

## Šta još NIJE povezano
- Supabase Auth prijava i stvarni korisnički nalozi
- Supabase baza i Storage
- Upload fotografija
- PDF generisanje
- QR kodovi
- Produkcijska pravila pristupa i testiranje

## Pregled
Otvorite `index.html` u modernom pregledniku. Ovo je demo, nije javno objavljena web-stranica.

## Objavljivanje
Za javno objavljivanje potreban je GitHub repozitorij i Vercel projekat kojim upravlja odrasla odgovorna osoba. Prije povezivanja sa stvarnom bazom potrebno je:
1. Dodati Supabase URL i publishable/anon ključ kroz sigurno podešavanje projekta.
2. Implementirati Supabase Auth.
3. Uskladiti frontend sa stvarnim RLS pravilima i testirati svaku ulogu.
4. Uvesti server-side/Edge Function tok za sigurno generisanje QR pristupa.
5. Testirati privatni Storage pristup, PDF izvještaje i autorizaciju.

Nikada ne stavljati `service_role` ključ ili druge tajne u frontend.
