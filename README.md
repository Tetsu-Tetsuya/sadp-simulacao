# SADP: simulação da comunicação RS485 / Modbus-RTU

Notebook que simula a comunicação entre o controlador (NUCLEO-G0B1RE, mestre Modbus) e os sensores ultrassônicos DYP-A02YY4W-V2 (escravos) em um tronco RS485 do SADP.

Ele estima o tempo de ciclo de leitura e o que pode dar errado no barramento: endereços repetidos, colisões e sensores que não respondem. Também traz o procedimento de endereçamento dos sensores, com uma versão para a bancada.

Os números são estimativas para orientar os testes de bancada, e não resultados de medição.

## Como rodar

Requer Python 3 com `ipykernel` e `matplotlib`. A versão para a bancada (seção 8.1) também usa `pyserial`.

```
pip install ipykernel matplotlib pyserial
```

Abra o `simulacao_comunicacao_SADP.ipynb` no VS Code ou no Jupyter e rode todas as células.
