# Mitarbeit am Story-Konzept.

Ziel ist es, unter Befolgung der Github Issues in Kombination mit [waffle.io](https://waffle.io) und �ber die Anwendung eines Git Flows das gesamte Konzept der Story in Mindmaps, Visualisierungen und (kurzen) Markdown-Files im Repository abzulegen.

Um eine einfachere Zusammenarbeit zu erreichen, werden die ersten Entw�rfe jeweils in Google Dokumenten oder anderen Collaboration-Tools erstellt.

Sobald diese Dokumente eine gen�gende Reife haben, um sie als erledigt zu betrachten, sollen Sie in Markdown-Files (oder in Bilder) konvertiert und ins Repository hochgeladen werden. Dabei ist ein Link auf die urspr�ngliche Datei miteinzubinden.

## Vorgehen f�r �nderungen/Erg�nzungen am Repository

1. Erstelle lokalen feature branch gem�� Github Issue. Beispiel: `git branch feature/#1-nameDesBranches`
2. F�ge lokal Dateien hinzu oder implementiere die �nderungen.
3. Pushe den feature branch zum Repo. Beispiel: `git push feature/#1-nameDesBranches feature/#1-nameDesBranches`
4. �ffne ein [Pull Request](https://help.github.com/articles/about-pull-requests/) auf Github.
5. Andere revidieren die �nderungen und stimmen dem Pull Request zu oder lehnen ihn ab.
6. Als Folge wird der feature branche in den develop branch gemerged.
7. Wenn ein Meilenstein erreicht wird, wird der develop branch in den master branch gemerged und dieser getagged.

## Was kann ich tun?

Checke die Github Issues oder schaue auf https://waffle.io nach, um zu checken welche Teilaufgaben noch von niemandem bearbeitet werden oder um herauszufinden, wer bei einer bestehenden Aufgabe unterst�tzt werden kann.

## Erstellen von Google Docs/Collaboration-Tool-Dateien

Die Entwurfsdatei soll immer von derjenigen Persion erstellt werden, die ein Issue als erster �bernommen hat. Allf�llige weitere Mitarbeiter werden sp�testens auf Anfrage vom Ersteller der Datei eingeladen.

## Zusammenhang waffle.io <-> GitHub Issues <-> Pull Requests
Wenn ein Issue auf Github erstellt wird, wird auf [waffle.io](https://waffle.io) automatisch eine entsprechende Karte im Kanban-Board erstellt.

Dies funktioniert auf umgekehrt: Wenn eine Karte auf Waffle erstellt wird, wird autoamtisch ein Issue erstellt. Dies ist die bevorzugte Variante.

Wenn ein Branch mit #[IssueNr.] im Namen erstellt wird, wechselt ein Issue automatisch auf "In progress". Dies wird auch von Waffle entsprechend angezeigt.

Erstellt man ein Pull Request, wechselt das Issue (auch in Waffle) auf "Review".

Um das Issue dann zu schlie�en, muss es entweder in Github manuell geschlossen werden (dann wechselt es in Waffle auf "Done") oder man schiebt es in Waffle auf "Done", dann wird es in Github automatisch geschlossen.

