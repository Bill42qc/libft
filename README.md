Libft

Libft est une bibliothèque de fonctions en C qui fournit des implémentations de fonctions standard du langage C ainsi que des fonctions supplémentaires utiles. Cette bibliothèque est conçue pour être utilisée dans le cadre des projets de l'école 42 et peut être étendue avec de nouvelles fonctions au fil du temps.
Fonctionnalités

    Fonctions standard : Implémentation de fonctions standard du langage C (ex. strlen, strcpy, atoi, etc.).
    Fonctions supplémentaires : Fonctions supplémentaires utiles pour la manipulation de chaînes, de listes chaînées, etc.
    Makefile : Makefile inclus pour faciliter la compilation et l'exécution des tests.
    Documentation : Commentaires détaillés pour chaque fonction pour faciliter la compréhension et l'utilisation.

Prérequis

    GCC (ou tout autre compilateur C compatible)
    Make

Installation

    Clonez le dépôt :

bash

git clone https://github.com/Bill42qc/libft.git

    Accédez au répertoire du projet :

bash

cd libft

    Compilez la bibliothèque :

bash

make

Utilisation

Pour utiliser la bibliothèque libft dans vos projets, vous pouvez inclure le fichier libft.a généré dans vos Makefiles et utiliser les fonctions fournies comme vous le feriez avec les fonctions standard du langage C.

Exemple de Makefile :

make

NAME = mon_projet

SRCS = main.c \
       ...

OBJS = $(SRCS:.c=.o)

all: $(NAME)

$(NAME): $(OBJS)
    gcc $(OBJS) -L. -lft -o $(NAME)

%.o: %.c
    gcc -c $

%.c

libft.a: $(OBJS)
ar rcs libft.a $(OBJS)

clean:
rm -f $(OBJS)

fclean: clean
rm -f $(NAME) libft.a

re: fclean all

.PHONY: all clean fclean re

yaml


## Documentation

La documentation complète des fonctions est disponible dans le fichier `libft.h`. Vous pouvez également consulter les commentaires détaillés dans les fichiers source de chaque fonction pour obtenir des informations sur leur utilisation et leur comportement.

## Contribution

Les contributions sont les bienvenues ! Pour des modifications majeures, veuillez ouvrir une issue pour discuter des changements proposés.

## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

---

Pour toute question ou préoccupation, n'hésitez pas à ouvrir une issue ou à contacter [votre-email@example.com](mailto:votre-email@example.com).
