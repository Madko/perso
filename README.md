Personnalisation post-install via Ansible
=========================================

Exemple de personnalisation possible via ansible, en se basant sur le script
bash de kikinovak.

# Pre-requis

Avoir le paquet ansible installé

# Lancement

Pour lancer le playbook global :

```
ansible-playbook -i inventory.txt setup.yml
```

La configuration des variables se fait dans `group_vars/machines.yml`.

L'inventaire par défaut `inventory.txt` contient la machine locale.
Il est possible de taper sur des machines distantes en les ajoutant dans
l'inventaire.

# TODO

Pour yum.conf passer par lineinfile plutôt qu'un template.

Définir les repos yum par le module yum_repository.

etc
