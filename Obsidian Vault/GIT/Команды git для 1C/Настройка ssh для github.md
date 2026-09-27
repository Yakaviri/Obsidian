	ls -la ~/.ssh
# Генерация ключа
	
	ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
# Запустить SSH-агент (в фоновом режиме)
	
	eval "$(ssh-agent -s)"
# Добавить ваш ключ (подставьте правильное имя файла)
	ssh-add ~/.ssh/id_ed25519

# Проверим что ключ загружен
	
	ssh-add -l
