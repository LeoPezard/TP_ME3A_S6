# Nom du fichier Markdown et PDF
FILE=test

# Commande pour générer le PDF
rapport: $(FILE).md
	pandoc -f markdown -o $(FILE).pdf -N $(FILE).md

# Commande pour surveiller les modifications
watch:
	while true; do \
		inotifywait -e modify $(FILE).md && make rapport; \
	done
