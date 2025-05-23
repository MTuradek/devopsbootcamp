# devopsbootcamp

# ssh and git configuration
1. New ssh key
```bash
ssh-keygen -t rsa -b 4096 -C "PLACEHOLDER" -f ~/.ssh/PLACEHOLDER
```
2. vim ./ssh/config
```bash
# Konfiguracja dla prywatnego konta GitHub
Host github.com-PLACEHOLDER
   HostName github.com
   User PLACEHOLDER
   IdentityFile ~/.ssh/PLACEHOLDER
   IdentitiesOnly yes
```
3. Clone the repository
```bash
git clone git@github-PLACEHOLDER:MTuradek/devopsbootcamp.git
```
4. Turn off signature verification
```bash
git config --local commit.gpgSign false
git config --local --get commit.gpgSign
```
