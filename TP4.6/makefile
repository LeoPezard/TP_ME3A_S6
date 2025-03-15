# Nom du fichier Markdown et PDF
FILE=2025-18-03-Gr2-B07_FANGET-PEZARD_Compte-rendu_4-6-SP

# Commande pour générer le PDF
rapport: $(FILE).md
	pandoc -f markdown -o $(FILE).pdf -N $(FILE).md

# Commande pour surveiller les modifications
watch:
	while true; do \
		inotifywait -e modify $(FILE).md && make rapport; \
	done
