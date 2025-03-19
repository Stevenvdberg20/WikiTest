
# Template voor README

Dit is gewoon de README test, hier kan van alles komen te staan als inleiding voor het project bijvoorbeeld, of informatie over de repository (hoe wordt deze onderhouden, welke licentie hangt eraan vast, ....)

## Inhoudsopgave (overgenomen van https://github.com/codefornl/community-translations-standard/blob/main/nl/index.md, maar doet het niet. Is alleen voor de looks even)

* [Auteurs](AUTHORS)
* [Voorwoord bij de vertaling](translation-foreword)
* [Voorwoord](foreword)
* [Leeswijzer](readers-guide)
* [Begrippenlijst](glossary)
* [Criteria](criteria/){% assign sorted = site.pages | sort:"order" %}{% for page in sorted %}{% if page.dir == "/nl/criteria/" %}{% if page.name != "index.md" %}{% if page.title %}
  * [{{page.title}}]({{site.baseurl}}{{page.url}}){% endif%}{% endif%}{% endif%}{% endfor %}
* [Bijdragen](CONTRIBUTING)
* [Gedragscode](CODE_OF_CONDUCT)
* [Governance](GOVERNANCE)
* [Versiegeschiedenis](CHANGELOG)
* [Licentie](LICENSE)
