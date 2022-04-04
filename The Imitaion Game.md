```py
from enigma.machine import EnigmaMachine

machine = EnigmaMachine.from_key_sheet(
    rotors="II IV V",
    reflector="B",
    ring_settings="B U L",
    plugboard_settings="AV BS CG DL FU HZ IN KM OW RX",
)

machine.set_display("WXC")
msg_key = machine.process_text("KCH")
machine.set_display(msg_key)
plaintext = machine.process_text("RFMNWZUMLEHFAAASRIDYGDADUBKFBJYAQXYKCE")
print("[+] Flag: " + plaintext)
```

```bash
$ python3 enigma.py
> FLAGTHISISASECRETMESSAGEFROMALANTURING
```
