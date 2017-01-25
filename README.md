# Codificacion-Huffman
 Ejecución: <br /> <br />
            Comprimir:    java PlantillaCodificacionHuffman -c filePathIn filePathOut  <br />
            Decomprimir:  java PlantillaCodificacionHuffman -d filePathIn filePathOut  <br />
  
 Utilidad:  <br /> <br /> Permite la compresión/descompresión usando el algoritmo de Huffman <br />
 de un archivo de entrada hacia un archivo de salida. 

Algoritmo de compresión de datos sin pérdida.
Codificación entrópica. Conocimiento previo de la probabilidad
de ocurrencia de los símbolos que aparecerán en la trama. Se 
emplean secuencias de bits de longitud variable, de modo que 
los símbolos más frecuentes tendrán secuencias más cortas.<br />
“Prefix-free codes”, libre de prefijos, (y libre de ambigüedad) la 
secuencia de bits que representa un símbolo nunca es un prefijo 
de otra secuencia que represente cualquier otro símbolo: <br />
{110A , 0B, 10C, 111D} <-> códigos de longitud variable libre de prefijos <br />
{110A , 0B, 11C, 1D} <-> códigos de longitud variable con prefijos <br />
{1010A, 1011B, 1100C,1101D} <-> códigos de longitud fija <br />
El algoritmo de Huffman produce códigos de longitud variable y 
prefix free, garantizando el menor tamaño promedio de salida 
en el proceso de codificación, cuando las frecuencias actuales de 
los símbolos se corresponden con las utilizadas al crear el código. 
