# network-printer
Setup network printer using ansible (install printer-driver-gutenprint drivers https://gimp-print.sourceforge.io/p_Supported_Printers.php)

## Install dependencies

```bash
python3 -m venv ./venv
source ./venv/bin/activate
pip3 install -r requirements.txt
```

## Run ansible

```
source ./venv/bin/activate
ansible-playbook -i hosts main.yml
```