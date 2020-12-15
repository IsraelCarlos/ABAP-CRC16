# ABAP-CRC16
Calculation of the Cyclic Redundancy Check(CRC) CRC-16/CCITT-FALSE in SAP ABAP.

Main Class: ``` zcl_crc_16 ```

```
DATA: lv_crc(4).
lv_crc = zcl_crc_16=>calc( lv_payload ).
```

It is an ABAP class, to calculate the Cyclic Redundancy Check (CRC), following the CRC-16 / CCITT-FALSE algorithm, within SAP systems.

Initial Value: FFFF -> 0000FFFF (ABAP)

Polynomial:    0121 -> 00000121 (ABAP)

- CALC

Import -> I_PAYLOAD (String you want to calculate the CRC)

Return -> R_CRC16 (CRC character in CHAR characters)

- CRC16_MAP:

Maps in a static table the hexadecimal values based on Polynomial 0121, to be used in the calculation.

# Português:

Cálculo da Verificação de Redundância Cíclica (CRC) CRC-16 / CCITT-FALSE no SAP ABAP.

Se trata de uma classe ABAP, para calcular Cyclic Redundancy Check (CRC), seguindo o algoritmo CRC-16/CCITT-FALSE, dentro de sistemas SAP.

Valor Inicial: FFFF -> 0000FFFF (ABAP)

Polinomial:  0121 -> 00000121 (ABAP)

Métodos:
- CALC
Importar -> I_PAYLOAD 	(String que deseja calcular o CRC)

Retorno -> R_CRC16		(CRC calculado em caracteres CHAR)

- CRC16_MAP:

Mapeia em uma tabela estática os valores hexadecimais baseados no Polinomial 0121, para ser usado no cálculo.
