# 🧊 Snow Crash – Projet Cybersécurité (École 42)

Projet de groupe réalisé avec [Malo Lefort](https://github.com/Malolfrt)

## 📌 Description

**Snow Crash** est un projet d’initiation à la cybersécurité proposé par l’école 42. Il prend la forme d’un wargame dans lequel chaque niveau présente une faille système permettant de passer à l’utilisateur suivant, jusqu’au niveau final.

Le but est d’identifier et d’exploiter des vulnérabilités locales (droits Unix, variables d’environnement, buffer overflow, etc.) afin d’escalader les privilèges sur une machine Linux.

---

## 🎯 Objectifs pédagogiques

- Comprendre les mécanismes de sécurité de base sous Linux.
- Apprendre à utiliser les outils d’analyse système (`ltrace`, `strace`, `gdb`, `find`, etc.).
- Identifier et exploiter des failles classiques (SUID, mauvaise configuration, injections, etc.).
- Automatiser certaines étapes de reconnaissance et d’exploitation.
- Se sensibiliser aux erreurs de sécurité courantes dans les environnements Unix.

---

## ⚙️ Environnement

- Système Linux distant (via SSH)
- 15 utilisateurs (`level0` → `level14`)
- Un mot de passe à découvrir par niveau
- Aucun droit root
- Terminal uniquement

---

## 🧩 Types de failles abordées

- level00 : Déchiffrage code caesar
- level01 : /etc/passwd attack - John The Ripper
- level02 : Analyse de flux TCP sur un fichier pcap - Wireshark
- level03 : Modification du PATH - binaire appel 'system'
- level04 : Exploit script perl
- level05 : cron execute tous les binaires d'un dossier
- level06 : Faille modifier "e" des REGEX php
- level07 : Injection par une varible d'environnement
- level08 : Bypass d'un check dans le code par un lien symbolique
- level09 : Reverse de hash
- level10 : Race condition entre access et open
- level11 : Faille via io.popen dans un script lua
- level12 : Faille via un subshell dans un script perl
- level13 : Modifier valeur de retour d'une fonction avec GDB
- level14 : Exploiter getflag

---

## 👨‍💻 Auteur

Projet réalisé dans le cadre du cursus cybersécurité de l’[École 42](https://42.fr/).

