# zoran-éthique-garde

**Moteur de règles éthiques** pour l’écosystème Zoran / QuantaGlottal©® — définition, application et explication de politiques éthiques (YAML), avec capacités de veto.

---

## ✨ Fonctionnalités
- **Chargement de politiques éthiques** au format YAML
- **Application en temps réel** des règles sur actions et décisions
- **Veto immédiat** si une règle est violée
- **Explications contextualisées** des refus
- **Extension modulaire** des politiques (plugins)
- **Interopérabilité** avec injecteurs, orchestrateurs et modules de gouvernance

---

## 📦 Installation (développement)
```bash
pip install -e .


---

⚡ Exemple rapide

from zoran_ethique_garde import EthicGuard

guard = EthicGuard(policy_file="policies.yaml")

action = {"type": "deploy", "impact": "environnemental", "risk": "high"}

if guard.check(action):
    print("Action autorisée")
else:
    print("Action bloquée :", guard.last_reason())


---

🧱 Structure suggérée

src/zoran_ethique_garde/
  __init__.py
  guard.py             # logique d'application des règles
  loader.py            # chargement YAML
  veto.py              # gestion des blocages
  explain.py           # génération d'explications
policies/
  default.yaml
tests/
  test_guard.py
pyproject.toml
.gitignore
LICENSE
README.md


---

🧪 Tests

pytest -q


---

🔐 Éthique

Le zoran-éthique-garde est fondé sur le principe :

vivant > humain comme règle suprême

transparence des décisions

capacité d’évolution des politiques



---

📜 Licence

MIT — voir LICENSE.


---

Auteur : Frédéric Tabary — Institut IA
Contact : 0645605023 — Canada, Montréal, France
INSTITUT🦋 IA INC., 7100-380, rue Saint-Antoine Ouest, Montréal (Québec) H2Y 3X7.# zoran-ethics-guard
Moteur de règles éthiques (policies YAML), explications &amp; veto.
