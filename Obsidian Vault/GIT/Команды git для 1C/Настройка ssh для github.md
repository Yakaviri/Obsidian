ls -la ~/.ssh #проверкаКлючейSSH

# генерация ключа
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
# Запустить SSH-агент (в фоновом режиме)
eval "$(ssh-agent -s)"
# Добавить ваш приватный ключ в агент
# Если вы использовали RSA:
ssh-add ~/.ssh/id_rsa