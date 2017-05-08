---
title: Install
subtitle: Install fcu-ansible
date: 2017-05-09
tags: false
---

## Dependencies

Please take care theses dependencies are installed in your system

- python >= 2.7  
- virtualenv  
- pip  

## Install

```bash
git clone https://github.com/delaballe/fcu-ansible.git
cd fcu-ansible
virtualenv .
. ./bin/activate
pip install -r requirement-pip

cat <<'EOF' >> config/outscale.ini
[default]
region = <YOUR OUTSCALE API REGION>
aws_access_key_id = <YOUR OUTSCALE API ACCESS KEY ID>
aws_secret_access_key =  <YOUR OUTSCALE API ACCESS KEY>
EOF
```

And voilà !!! you're ready to play provision & deploy in the Outscale Cloud Platform using Ansible.
