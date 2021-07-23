# Ethereum Solidity

Aprendiendo solidity a través de Remix Ide. 

Remix es un IDE web que te permite compilar smart contracts y deployarlos a las distintas redes. Tiene una blockchain local llamada Javascript VM que permite deployar y testear contratos.

También te permite interactuar con ellos cuando los deployas


## Tipo de funciones.

**Pure or view functions.** 
Sólo devuelven un valor, están leyendo una propiedad o bien devolviendo un valor. **No cuestan GAS** porque no realizan ningún tipo de transacción.

**GAS Spending functions**
Cómo realizan una transacción (la crean) utilizan GAS y necesitan ser aprobadas. (Firmadas por una private key)

**Payable functions**
Las funciones payable permiten recibir ETH en el contrato.

## Tipo de variables

uint256 - Unsigned int de 256 bit.

## Declaración de funciones

```
function <funtion_name>(<parameter>)<modifier> returns (type) {}
```

Si al final de la función utilizamos el modificador `view`, estaremos prometiendo que no modifica el ESTADO del contrato. Por lo cual es **completamente gratis.**

````
function get() public view returns(uint64){}
`````

## Eventos

Los eventos pueden ser emitidos desde un contrato, para que aplicaciones clientes puedan escucharlos desde la blockchain sin mucho costo.

`````
event sent()
`````



