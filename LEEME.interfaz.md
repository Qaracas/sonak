# Interfaz de programación

<table>
<tr>
<th align="left">
jsonLstm
</th>
</tr>
<tr>
<td>
<pre>

**function jsonLstm(json, lista)**

Trasforma una cadena de texto en formato JSON en una lista multidimensional jasonizada
(en adelante nombrada como lista MJ).

**Argumentos:**
   json  - Puntero a cadena de texto en formato JSON.
   lista - Lista MJ.
</pre>
</td>
</tr>
<tr>
<th align="left">
lstmJson
</th>
</tr>
<tr>
<td>
<pre>

**function lstmJson(lista, json)**

Trasforma una lista MJ en una cadena de texto en formato JSON.

**Argumentos:**
    json  - Puntero a cadena de texto en formato JSON.
    lista - Lista MJ.
</pre>
</td>
</tr>
<tr>
<th align="left">
pinta
</th>
</tr>
<tr>
<td>
<pre>

**function pinta(lista, frmt)**

Pinta por pantalla una lista multidimensional

**Argumentos:**
    lista - Lista MJ.
    frmt  - Formato de representación. Por ejemplo: "%s ,"
</pre>
</td>
</tr>
<tr>
<th align="left">
trae
</th>
</tr>
<tr>
<td>
<pre>

**function trae(lista, elmnt)**

Busca un elemento localizado dentro de una lista MJ y devuelve su valor.

**Argumentos:**
    lista - Lista MJ.
    elmnt - Elemento a buscar en formato "a.b.c".
    
**Resultado:**
    - Si el elemento existe en la lista devuelve su valor y, ademas,
      pone RFUNC["trae"] a 1.
    - Si no existe el elemento devuelve "" y, además, pone RFUNC["trae"] a 0.
</pre>
</td>
</tr>
<tr>
<th align="left">
quita
</th>
</tr>
<tr>
<td>
<pre>

**function quita(lista, elmnt)**

Elimina elementos de una lista multidimensional jasonizada.

**Argumentos:**
    lista - Lista MJ.
    elmnt - Elemento a aliminar en formato "a.b.c".
    
**Resultado:**
    - Si el elemento existe en la lista lo elimina y devuelve su posición.
      Ademas, pone RFUNC["quita"] a 1.
    - Si no existe el elemento devuelve 0 y, además, pone RFUNC["quita"] a 0.
</pre>
</td>
</tr>
<tr>
<th align="left">
pon
</th>
</tr>
<tr>
<td>
<pre>

**function pon(lista, elmnt, valor)**

Añade un nuevo elemento a la lista MJ o modifica el valor de uno ya existente.

**Argumentos:**
    lista - Lista MJ.
    elmnt - Elemento para añadir/modificar en formato "a.b.c".
    valor - Valor del nuevo elemento o nuevo valor para el elemento ya existente.

**Resultado:**
    - Devuelve la posición del nuevo elemento la posición del que se haya
      modificado en caso de que existiese. 
</pre>
</td>
</tr>
<tr>
<th align="left">
pon
</th>
</tr>
<tr>
<td>
<pre>

**function sangra(json)**

Pinta por pantalla el texto en formato JSON que se le pasa como argumento, sangrando líneas para facilitar su lectura.

**Argumentos:**
    json  - Puntero a cadena de texto en formato JSON.

**Resultado:**
    - Nada.
</pre>
</td>
</tr>
</table>