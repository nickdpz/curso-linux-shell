# Course Programming With Shell ✅
Recursos de curso de programación en linea de comandos de platzi

## Acciones más utilizadas

- Asignar permisos de ejecución
```bash
chmod +x scritp.sh
./scritp.sh 1
```

- Capturar información del usuario
```bash
read -p "Ingresar una opción:" option
```

- Validar expresiones regulares

```bash
#!/bin/bash
expresionRegular1=^[a-zA-Z]$
expresionRegular2=^[0-9]$
if [[ $1 =~ $expresionRegular1 ]]; then
 echo "Valid regex 1"
elif [[ $1 =~ $expresionRegular2 ]]; then
 echo "Valid regex 2"
else
 echo "Invalid regex"
fi

```

- Expresiones condicionales con numeros

```bash
# !/bin/bash
edad=0
read -p "Ingrese su edad:" edad
echo -e "\nExpresiones Condicionales con números"
if [ $edad -lt 10 ]; then
    echo "La persona es un niño o niña"
elif [ $edad -ge 10 ] && [ $edad -le 17 ]; then #Mayor o igual - Menor o igual
    echo "La persona se trata de un adolescente"
else
    echo "La persona es mayor de edad"
fi
```

- 
```bash
$
```
