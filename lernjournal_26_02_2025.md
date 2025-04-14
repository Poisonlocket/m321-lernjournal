# Lernjournal LU05a – LU06b: Authentisierung, Autorisierung und Token in Webanwendungen

## Kurzbeschrieb

In diesen Unterrichtsblöcken ging es um die Grundlagen der Authentisierung und Autorisierung in Webanwendungen sowie um moderne Verfahren zur sicheren Identifikation von Benutzern. Dabei wurde insbesondere auf JSON Web Tokens (JWT) eingegangen, die eine zentrale Rolle bei der Realisierung von Sicherheitsmechanismen in verteilten Systemen spielen. Ergänzend wurde erklärt, wie man solche Tokens in Clients speichern und bei Requests verwenden kann.

## Lernerfolge

Ich habe ein fundiertes Verständnis der Unterschiede zwischen **Authentisierung** (Identitätsbehauptung) und **Authentifizierung** (Identitätsprüfung) gewonnen. Besonders spannend war die Unterscheidung der Authentifizierungsarten: Wissen (z.B. Passwort), Besitz (z.B. SMS-Code) und Sein (z.B. Fingerabdruck).

Die Einführung von **Mehr-Faktor-Authentifizierung** sowie Technologien wie **FIDO2** zeigen, wie wichtig es ist, die Benutzeridentität auf mehrere Arten zu überprüfen – vor allem im Kontext von Webdiensten mit sensiblen Daten.

Ein besonderes Aha-Erlebnis hatte ich beim Thema **JWT**: Endlich habe ich wirklich verstanden, wie ein stateless Authentifizierungsmechanismus funktioniert. Dass ein Token nach erfolgreichem Login erstellt, signiert und verschlüsselt wird, und dann bei jedem weiteren Request mitgeschickt wird, ist ein extrem eleganter Ansatz.

## Reflexion

Ich finde es sehr sinnvoll, dass wir in unserer IDPA-Vorabschlussarbeit *Sproutly* genau diese Techniken einsetzen: Wir nutzen JWT und speichern das Token im `sessionStorage`. Das war am Anfang etwas verwirrend, aber durch das Unterrichtsmaterial habe ich das Konzept nun wirklich durchschaut.

Etwas irritierend finde ich allerdings, dass trotz Single Sign-On mit Azure AD am BZZ manchmal mehrere Logins notwendig sind. Ich benutze privat den Brave-Browser, was möglicherweise auch eine Rolle spielt. Aber ich verstehe jetzt: SSO gilt jeweils nur innerhalb der gleichen Umgebung, also z.B. nur im selben Browser.

## Glossar (in eigenen Worten)

- **Authentisierung**: Ich sage dem System, wer ich bin – z.B. durch Eingabe meines Benutzernamens.
- **Authentifizierung**: Das System prüft, ob ich wirklich die Person bin – z.B. durch Überprüfung des Passworts.
- **Autorisierung**: Das System entscheidet, ob ich etwas tun darf – z.B. ob ich Bücher aus einer Liste abrufen darf.
- **JWT (JSON Web Token)**: Ein kompaktes, verschlüsseltes Token, das Informationen über mich enthält, z.B. meine Rolle oder ID.
- **Session Storage**: Ein Zwischenspeicher im Browser, der Daten nur solange aufbewahrt, wie die Seite offen ist.
- **Mehr-Faktor-Authentifizierung (MFA)**: Ich muss mehrere Dinge beweisen, z.B. Passwort + Code auf dem Handy.
- **FIDO2**: Ein Authentifizierungsverfahren ohne Passwort, das z.B. auf Hardware-Token basiert.
- **Single Sign-On (SSO)**: Einmal anmelden, mehrfach nutzen – aber nur innerhalb eines bestimmten Kontexts (z.B. derselbe Browser).
