# VAPP — trvalé pokyny

- Produktové karty **náhradních dílů** NEobsahují výpis klíčových vlastností/parametrů. Klíčové vlastnosti se vypisují pouze na kartách **přívěsů**.
- Font webu: Exo 2 (Google Fonts). Základní text 16 px, minimální velikost 13 px, maximální font-weight 700.
- Rádiusy: jemné — 6 px (inputy, badge), 8 px (karty, tlačítka), 999 pill. Karty bez borderů; jemný stín jen při hoveru. Jen světlý režim.
- Oficiální logo: vapp-logo.svg (křivky, červená #E41D32).
- Všechny ikony ve standardu 24×24 px (SVG s viewBox 0 0 24 24, vykreslené 24×24). Výjimka: ikony skladovosti 18×18. Hlavní menu na desktopu 18 px.
- Hlavní menu: záložky s underline (aktivní položka podtržená), ne tlačítka.
- Produktový grid: 4 sloupce na desktopu, 2 na mobilu.
- Karta náhradního dílu obsahuje: fotku 4:3, název, 5hvězdičkové hodnocení (+počet), skladovost zeleným textem s ikonou („Skladem > 15 ks"), ceny vpravo pod sebou (primární bez DPH bez popisku, menší „X Kč s DPH"), kvantifikátor + tlačítko Koupit, dole checkbox Porovnat + Obj. č. (6místné, terciální). Celá karta klikací na detail. Badge (sleva / Doprava zdarma) vlevo nahoře na fotce.
- Jediný zdroj vzhledu karty: `ProduktovaKarta.dc.html` (ASCII název bez diakritiky/mezer kvůli exportu na GitHub) — upravovat POUZE tam; prototyp i katalog ji importují přes dc-import.
- Struktura projektu: `Design systém VAPP.dc.html` = jen barvy + typografie. `Komponenty VAPP.dc.html` = katalog všech UI prvků (karta, tlačítka, kvantifikátor, formuláře, badge, skladovost, výpis kategorií, menu, breadcrumb, patička) — jediné místo, kde se komponenty ladí; návrhové stránky je odtud přebírají. Reusable komponenty = samostatné .dc.html soubory importované přes dc-import.
