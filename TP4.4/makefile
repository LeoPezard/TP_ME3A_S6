# Nom du fichier Markdown et PDF
FILE=2025-03-04-Gr2-B07_FANGET-PEZARD_Compte-rendu_4-4-ST

# Commande pour générer le PDF
rapport: $(FILE).md
	pandoc -f markdown -o $(FILE).pdf -N --toc $(FILE).md

# Commande pour surveiller les modifications
watch:
	while true; do \
		inotifywait -e modify $(FILE).md && make rapport; \
	done
