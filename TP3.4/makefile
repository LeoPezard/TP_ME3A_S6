# Nom du fichier Markdown et PDF
FILE=2025-29-04-Gr2-B07_FANGET-PEZARD_Compte-rendu_3-4-PAC

# Commande pour générer le PDF
rapport: $(FILE).md
	pandoc -f markdown -o $(FILE).pdf -N $(FILE).md

# Commande pour surveiller les modifications
watch:
	while true; do \
		inotifywait -e modify $(FILE).md && make rapport; \
	done

final: $(FILE).md
	pandoc -f markdown -o $(FILE).pdf \
	--pdf-engine=xelatex \
	-N --toc \
	--include-before-body=page_de_garde.tex \
	$(FILE).md