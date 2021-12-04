# Programming With Shell ✅
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

- Sentencia Case or Switch
```bash
case $opcion in
    "A") echo -e "\nOperación Guardar Arhivo";;
    "B") echo "Operación Eliminar Archivo";;
    [C-E]) echo "No esta implementada la operación";;
    "*") "Opción Incorrecta"
esac    
```

- Verificar si un archivo existe en la carpeta del script
```bash
echo -e "\nExpresiones Condicionales con archivos"
if [ -d $pathArchivo ]; then
    echo "El directorio $pathArchivo existe"
else 
    echo "El directorio $pathArchivo no existe"
fi    
```

- Iterar todos lo archivos de ls con for

```bash
for fil in $(ls)
do
    echo "Nombre archivo:$fil"
done
```

- Iterar con while

```bash
while [ $numero -ne 10 ]
do
    echo "Imprimiendo $numero veces"
    numero=$(( numero + 1 ))
done
```


- Iterar con while

```bash
while [ $numero -ne 10 ]
do
    echo "Imprimiendo $numero veces"
    numero=$(( numero + 1 ))
done
```

- Escribir en un archivo sin necesidad de abrir editor

```bash
cat <<EOM >>$1 #Nombre de archivo
$2
EOM
```

