# Infrastruttura per i servizi di CSUnibo

Raccolta di _task_ _Ansible_ per configurare l'infrastruttura dietro ai servizi di CSUnibo.

I dettagli sull'uso sono disponibili sulla wiki di CSUnibo alla pagina <https://csunibo.github.io/wiki/infrastruttura/automazione/index.html>.


## Come usare i task

I task sono scritti per essere usati con _Ansible_ in modalità _playbook_.

### Setup per tutti gli host

```bash
ansible-playbook install.yaml
```

### Setup per un singolo host

```bash
ansible-playbook install.yaml -l <nome_host>

# Esempio per il solo host dynamik
ansible-playbook install.yaml -l dynamik
```

Gli host sono definiti nel file `hosts`.
