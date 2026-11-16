# Inlämning 3: Smarta hemmet, del 1

Startkod för inlämning 3 i Programmeringsparadigmer 1. Hela uppgiftsbeskrivningen finns i Canvas. Kundens krav finns i `REQUIREMENTS.md`.

Projektet är ett Maven-projekt. Öppna mappen i IntelliJ IDEA, så känns det igen automatiskt.

| Var | Innehåll |
|---|---|
| `REQUIREMENTS.md` | Kravtexten från kunden |
| `design/` | Din design från del A: substantiv- och verblistan med genomspelningen, och senare eventuella avvikelser |
| `uml/` | Dina klass- och sekvensdiagram från Astah (`.asta`) eller Mermaid (`.mmd`), och exporterade bilder |
| `src/main/java/ax/ha/pp1/smarthome/` | Din kod. Det finns inget givet kontrakt, men paketen är givna: `capability` för förmågegränssnitten, `device` för enheterna, `home` för hemmet och `scene` för scenarier och åtgärder. `Main` skriver du i själva paketet `ax.ha.pp1.smarthome`. Filerna `package-info.java` beskriver vad varje paket är till för – ta inte bort dem. `llm/LlmClient.java` används bara i den valfria fördjupningen. |
| `src/test/java/ax/ha/pp1/smarthome/` | Dina JUnit-tester, i samma paket som koden de testar |
| `answers/` | Del C: prompten, AI:ns design och din jämförelse |

Arbetsordning:

1. Del A: designen checkas in **innan** du skriver någon egen kod.
2. Del B: kod och tester. Persiennen läggs till i en egen commit som **bara lägger till filer**.
3. Del C: jämförelsen med en AI-design.

Kör testerna genom att högerklicka på `src/test/java` och välja **Run 'All Tests'**, eller med `mvn test` i en terminal.

Vid varje push kör GitHub `mvn test` automatiskt (`.github/workflows/tests.yml`). Resultatet syns som en grön bock eller ett rött kryss vid commiten, och under fliken **Actions** ser du vilket test som gick fel. Innan du har skrivit några tester är bocken grön.
