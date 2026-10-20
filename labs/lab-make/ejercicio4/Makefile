# Nombre del ejecutable final
PROGRAMA := programa

# Compilador y flags
CC     := gcc
CFLAGS := -Wall

SRCS := main.c operaciones.c
OBJS := $(SRCS:.c=.o)

# Regla principal
all: $(PROGRAMA)

# Regla para linkear los objetos y generar el ejecutable
# TODO 3: Completá el comando de linkeo
#         Usá $(CC), la variable automática $^ (todos los prerequisitos)
#         y el flag -o $(PROGRAMA)
$(PROGRAMA): $(OBJS)
	$(CC) $^ -o $(PROGRAMA)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Regla para limpiar archivos generados
clean:
	rm -f $(PROGRAMA) $(OBJS)

.PHONY: all clean
